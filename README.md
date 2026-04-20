网络安全策略/框架/标准/指南/白皮书的原创翻译

## 0 已翻译作品

| 文档 | 类型 | 说明 |
|------|------|------|
| [**NIST CSF 2.0**](https://secnotes.github.io/grc/papers/csf2.0/) | 网络安全框架 | 网络安全风险管理指南 |
| [**NIST RMF (SP 800-37)**](https://secnotes.github.io/grc/blogs/rmf/) | 风险管理框架 | [完整PDF版](attachment/NIST-800-37-RMF/NIST-SP-800-37r2-完整中文版.pdf) |
| [**NIST AI RMF**](https://secnotes.github.io/grc/papers/airmf/) | AI 风险管理 | 人工智能风险管理框架 |
| [**NIST SP 800-53**](https://secnotes.github.io/grc/ai/nist-800-53/) | 安全与隐私控制 | 安全控制措施 |
| [**NIST SP 800-57 Part 1 Rev 6**](https://secnotes.github.io/grc/translations/NIST.SP.800-57pt1r6.ipd/) | 密钥管理 | 密钥管理建议 |
| [**GDPR**](https://secnotes.github.io/grc/ai/gdpr/) | 数据保护法规 | GDPR 条款中文翻译 |
| [**OWASP MASVS v2.1.0**](https://secnotes.github.io/grc/papers/owasp-masvs/) | 移动应用安全 | 移动应用安全验证标准 |
| [**AVSS 白皮书 1.0**](https://secnotes.github.io/grc/papers/avsswhitepaper/) | 车辆安全 | 车辆安全标准 |
| [**NIST CSF、ISO 27001/2、NIST 800-53 和 SCF**](https://secnotes.github.io/grc/blogs/csf27001-80053-scf/) | 框架对比 | 框架对比分析 |



## 1 本地运行

### 安装 Hugo

需要安装 Hugo extended 版本：

```bash
# Linux (Debian/Ubuntu)
sudo apt install hugo=0.145.0-1

# 或使用 snap
sudo snap install hugo --channel=extended

# 或直接下载 deb 包
wget https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_extended_0.145.0_linux-amd64.deb
sudo dpkg -i hugo_extended_0.145.0_linux-amd64.deb
```

### 克隆项目

```bash
git clone --recurse-submodules https://github.com/secnotes/grc.git

# 如果已经克隆但缺少主题
git submodule update --init --recursive
```

### 启动服务器

```bash
cd grc
hugo server
```

访问 `http://localhost:1313/grc/` 查看效果。

### 常用命令

| 命令 | 说明 |
|------|------|
| `hugo server` | 启动开发服务器，实时预览 |
| `hugo server -D` | 包含草稿内容 |
| `hugo` | 构建静态文件到 `public/` 目录 |
| `hugo new content/papers/new-doc.md` | 创建新内容 |

## 2 贡献指南

**方式一：提交 issue**

最简单的方式是提交 issue，帮助我们一起成长！

**方式二：Pull Request**

直接在网页上提交

```
1. 需要一个 GitHub 账户
2. 直接点击 content/paper，选择编辑栏的右上角的 🖊 进行修改
3. 直接添加想要贡献的内容
4. 保存，即选择 “Propose file change”，默认会克隆本项目到你的账户
5. 选择你账号中刚刚 fork 的本项目，提交 “pull request”
```

Git 提交

```
1. 点击项目上的 fork 按钮
2. git clone https://github.com/你的账户/grc.git
3. hugo new content/* 修改本地已经拉取的分支，增加你想要修改的内容
4. git add *
5. git commit -m "添加描述"
6. git pull
7. 选择你账号中刚刚 fork 的本项目，提交 “pull request”
```

## License

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="知识共享许可协议" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />本作品采用<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">知识共享署名-相同方式共享 4.0 国际许可协议</a>进行许可。
