---
title: NIST 风险管理框架 RMF
date: 2025-04-20T20:44:21+08:00
tags: []
series: []
featured: false
summary: "NIST 风险管理框架 RMF 是一种基于风险的结构化方法，用于管理网络安全威胁并确保符合安全要求。它被与政府系统合作的美国联邦机构和组织广泛使用。RMF 提供了一个七步流程（准备、分类、选择、实施、评估、授权和监控），用于将安全和风险管理集成到组织的系统开发生命周期中。"
code: utf-8
---


## 风险术语及相关概念

CISSP 相关的风险术语和概念，本章节内容来源于《CISSP官方学习手册第9版》，精选其中的重点字段和概念，详细内容请参考相关文章。

- **资产**：资产可以是业务流程或任务中使用到的任何事物。如果组织以来于某个人、某个位置或者某样事物，那这就是资产，不管其是有形的还是无形的。
- **威胁**：任何可能发生的、对组织或特定资产造成不良或非预期结果的潜在事件。
- **脆弱性**：资产中的弱点，是防护措施或控制措施的弱点。
- **暴露**：暴露是指威胁导致资产受到破坏的可能性。
- **风险**：威胁利用脆弱性对资产造成损害的可能性和严重程度。
- **风险框架**：关于如何评估、解决和监控风险的指南或方法。
- **风险管理**：风险管理过程包括识别可能造成数据损坏或泄露的因素，根据数据价值和控制措施的成本评估这些因素，并实施具有成本效益的解决方案来减轻或者降低风险。

**风险管理的整体过程用于制定和实施信息安全策略，这些策略旨在支持组织使命**。首次执行风险管理的结果是制定安全策略的依据；随着内部和外部条件的变化，后续的风险管理事件用于改进和维持组织的安全基础设施。**风险管理的主要目标**是将风险降低至可接受的水平。

风险管理是由**风险分析/评估**和**风险响应**这两个基本要素组成。**风险分析**是检查环境中的风险，评估每个威胁事件发生的可能性和实际发生后造成的损失，并评估各种风险控制措施的成本。这个结果可用于对风险优先级的关键级别进行排序。**风险响应**包括使用成本/收益分析的方式评估风险控制措施、防护措施和安全控制，根据其他条件、关注事项、优先事项和资源调整评估结果，并向高层建议响应方案。根据管理决策和指导，部署方案。

与风险管理相关的一个概念是**风险意识**，风险意识是为提高组织内部风险认知而开展的工作。风险意识有助于组织了解遵守安全策略的重要性以及安全失效的后果。

**安全治理**是与支持、评估、定义和指导组织安全工作相关的实践集合。**安全治理旨在将组织内所使用的安全流程和基础设施与从外部来源获得的知识和见解进行比对。** 安全治理通常是较严格和高层次的内容。最终，安全治理指实施安全解决方案以及与之紧密关联的管理方法。安全治理直接监督并涉及所有级别的安全。

## RMF 概述

[风险管理框架 RMF ](https://csrc.nist.gov/projects/risk-management/rmf-overview)是一套标准，规定了美国政府 IT 系统的架构、保护和监控方式。RMF 最初由美国国防部（DoD）开发，并于 2010 年被美国其他联邦信息系统采用。该特别出版物旨在将之前的 C&A（认证和认可） 流程转变为我们现在所知的 RMF。尽管初始版本运行良好并被联邦机构采用，但它缺乏足够的集中隐私控制措施，并且只有 6 个步骤。第二次修订版于 8 年后的 2018 年 12 月发布，在我们现在所知的 RMF 中增加了“**准备**”步骤和更多常用控制措施。如今，美国国家标准与技术研究院 (NIST) 负责维护 RMF。

NIST RMF 已取代联邦机构先前使用的风险管理认证流程，目前正用于管理联邦政府所有运营系统中的风险。虽然它是**联邦机构的强制性要求**，但它也因其能够最大限度地降低风险而被私人组织所采用。

RMF 是一个框架，也是一个将信息安全和隐私管理整合到一个大型风险管理系统中的指南或标准。RMF 主要基于[《联邦信息安全现代化法案》（FISMA）](https://www.cisa.gov/topics/cyber-threats-and-advisories/federal-information-security-modernization-act)，旨在确保联邦机构拥有一个通用的框架来有效地管理风险。FISMA 本质上确立了风险管理计划的要求，而 RMF 则是一种格式，具体规定了如何实施该计划以获得联邦政府授权。

- NIST SP 800-30，题为[《风险评估指南》](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-30r1.pdf)，概述了风险管理如何融入系统开发生命周期 (SDLC)，并描述了如何进行风险评估以及如何降低风险。
- [NIST SP 800-37](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-37r2.pdf)讨论了风险管理框架 RMF 本身，并包含我们将在本指南其余部分介绍的大部分信息。
- 最后，NIST SP 800-39，标题为[《管理信息安全风险》](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-39.pdf)，定义了对于达到 RMF 合规性至关重要的多层次、组织范围的风险管理方法。

## RMF 实施流程

NIST 风险管理框架（RMF）旨在创建一个通用框架，用于联邦机构保护信息系统。它包括一个全面、灵活、可重复且可衡量的 7 步流程。这 7 个步骤（**准备、分类、选择、实施、评估、授权和监控**）帮助组织管理信息安全和隐私风险。NIST 建立了安全控制目录 ( [SP 500-83](https://www.steeltoad.com/what-is/nist-sp-500-83/) )，用于组织制定安全和隐私计划。RMF 可以根据每个组织的具体需求进行定制。

![1](../images/1.png)

**准备（Parepare）**

- 帮助组织做好管理安全和隐私风险准备的基本活动
  - 确定风险管理的不同角色
  - 制定组织层面的战略
  - 确定风险承受能力
  - 执行组织层面的风险评估
  - 制定持续监控风险的策略
  - 确定常见的控制措施

**分类（Categorize）**

- 根据风险影响分析对信息/系统进行分类
- 确定风险对系统流程/任务对 CIA 的影响。并根据此影响提出风险管理建议。
  - 文件系统特性
  - 对系统和信息进行分类
  - 审核/批准分类

**选择（Select）**

- 根据风险评估选择一组 NIST SP 800-53 控制措施来保护系统
  - 选择安全控制基线
  - 系统特定、通用或混合的控制
  - 控制被分配给系统的特定部分
  - 制定整个系统的持续监控策略
  - 证明先前选择、分配和指定安全控制措施的安全/隐私计划已获批准

**实施（Implement）**

- 实施选定的 NIST SP 800-53 控制措施并记录其部署方式
  - 先前指定的控制措施已实施
  - 选择步骤中的安全和隐私计划已更新，以反映已实施的控制措施

**评估（Assess）**

- 评估以确定 NIST SP 800-53 控制措施是否到位、是否按预期运行并产生预期结果
  - 选择评估员/评估团队进行评估，并制定、审查和批准计划
  - 制定评估报告
  - 采取一切必要的补救措施
  - 根据评估更新安全/隐私计划
  - 制定行动计划/里程碑

**授权（Authorize）**

- 高级官员做出基于风险的决定，授权系统运行
  - 授权包（执行摘要、系统安全/隐私计划、评估报告、行动计划和里程碑）
  - 风险判定
  - 提供的风险应对措施
  - 授权被批准或拒绝

**监控（Monitor）**

- 持续监控 800-53 控制实施情况和系统风险
  - 系统受到监控，并根据选定步骤中制定的持续监控策略进行持续评估
  - 分析持续监测策略的结果
  - 确保有一个向管理层报告安全和隐私问题的框架
  - 根据持续监测结果进行持续授权

## 相关问题

### 1 RMF 真的有必要吗

在日益危险的网络环境中，国家面临的联邦信息威胁至关重要。网络世界已成为美国地缘政治敌人的新前线，而俄罗斯尤其利用了这一新的海外机遇。美国网络安全和基础设施安全局 (CISA) 表示：“随着俄罗斯不断完善和运用其间谍、影响和攻击能力，它将继续成为全球最大的网络威胁。” CISA 指出，“优先修补已知漏洞至关重要”，而这正是 RMF 的开发初衷。它能够识别潜在风险（或漏洞），并创建一种实施安全控制措施以降低这些风险的格式。

RMF 不仅对于美国控制系统和关键基础设施的防御很重要，而且也可以实现个人身份信息的保护。每位美国公民的个人信息都存储在联邦机构的多个信息系统中。如果没有适当形式的风险管理，这些个人身份信息或将面临极大的风险。

RMF 框架的重要性还在于，其概述了组织评估、持续重新评估和监控风险的形式。当公共或私人组织必须在不断变化的网络安全环境中保持良好保护环境时，识别和防御当前或未来威胁的能力至关重要。

### 2 RMF 是审计吗

RMF 主要充当评估，而非审计或评价。在流程的第 5 步和第 6 步中，RMF 使用称为“**评估和授权 (A&A)**”的流程。组织成功准备、分类系统、选择并实施控制措施后，现在必须进行评估和授权，因此该流程得名。评估是一个复杂的过程，由担任各种职务的许多高级官员监督。然而，授权主要由“授权官员”监督，他最终决定是否授权某个系统运行。他根据控制措施的有效性和合理选择，以及先前对安全和隐私问题的评估来做出此决定。

### 3 RMF 组织期望：角色和职责

- 机构负责人
- 架构师
- 安全隐私架构师
- 采购
- 通用控制提供程序
- 首席信息官
- 风险主管
- 高级机构信息安全官
- 系统管理员
- 用户
- ...

### 4 谁可以使用 RMF

RMF 最初仅供[国防部](https://www.steeltoad.com/what-is/dod/)使用。国防部比其他联邦机构更早开发并实施了该标准。然而，自 2010 年 NIST 将其作为特别出版物发布以来，所有联邦机构都必须遵守该指南并获得授权才能运行其系统。[RMF 授权](https://www.steeltoad.com/risk-management-framework/)对于拥有大量信息以及个人身份信息或政府机密信息的联邦机构尤为重要。

虽然 RMF 最初是为联邦机构设计的，但它也适用于私营部门。联邦机构和私营部门的实施流程相同，唯一的区别在于，私营部门可以自行决定是否符合 RMF 的要求并获得政府授权。

### 5 RMF vs CSF

NIST RMF 对于联邦机构来说是强制性的，并且经常用于处理敏感数据的行业，例如医疗保健、国防和金融。

NIST CSF 在私营部门得到广泛应用，并被全球公认为提高网络安全的最佳实践框架。

| **特征** | **NIST RMF**                   | **NIST CSF**               |
| -------- | ------------------------------ | -------------------------- |
| **目的**     | 确保联邦系统的合规性和安全性   | 增强所有组织的网络安全韧性 |
| **强制** | 是的，对于美国联邦机构         | 否，所有行业均自愿         |
| **重点**    | 合规驱动                       | 基于风险的灵活方法         |
| **用户**     | 政府机构、承包商和受监管行业   | 各行各业                   |
| **结构**    | 七步流程，结构化流程           | 六大核心功能，灵活可调整   |
| **采用**     | 严格按规执行                   | 适应组织需求               |
| **细节**     | 细致和系统的控制措施（800-53） | 开放和灵活的控制措施       |

NIST CSF 和 NIST RMF 均可与 ISO 27001 认证对接，ISO 27001 是国际公认的信息安全管理系统标准。ISO 27001 认证侧重于建立、实施、维护和持续改进组织的信息安全控制措施。NIST 框架可作为开发符合 ISO 27001 要求的控制措施和流程的基础。这种对接确保了全面的网络安全风险管理方法，并使组织能够展示其对国际标准和最佳实践的承诺。

<hr />
<div style="text-align: right;">
    原文：<a href="https://www.steeltoad.com/risk-management-framework">Risk Management Framework (RMF)</a><br />
    本文翻译有改动和整合
</div>