若github pages根路径存在问题，需要添加相对路径
```html
relativeURLs = true
```

若需保留 relativeURLs = true，需在模板中使用 absURL 函数转换链接：

```html
<a href="{{ absURL .URL }}">{{ .Name }}</a>
```

```css
style='background-image: url("{{ with .Params.image }}{{ . | absURL }}{{ else }}{{ absURL (printf "images/%d.jpg" $randomNumber) }}{{ end }}"); background-size: cover; background-position: center; background-repeat: no-repeat; width: 100%;'
```