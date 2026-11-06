---
title: 成熟度评估
description: Apache HugeGraph 社区成熟度模型评估
weight: 50
---

# Apache HugeGraph 成熟度评估

本成熟度模型旨在以简明、高层次的方式描述 Apache 项目的运作方式，并提供一个基础评估框架供项目进行自我评估。

更多背景说明请参阅 [Apache 项目成熟度模型](https://community.apache.org/apache-way/apache-project-maturity-model.html)。

## 当前评估状态

初步评估已完成。

## 成熟度模型评估明细

以下表格依据 [Apache 成熟度模型](https://community.apache.org/apache-way/apache-project-maturity-model.html)填写，欢迎导师（Mentors）与社区成员审阅、讨论并协助完善。

### 代码（CODE）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **CD10** | 项目向公众免费产出并分发开源软件。 | **是（YES）** 项目源代码基于 `Apache License 2.0` 协议开源发布。 |
| **CD20** | 任何人都可以便捷地发现并访问项目代码。 | **是（YES）** [官方网站](https://hugegraph.apache.org/cn/)包含指向 [GitHub 代码仓库](https://github.com/apache/hugegraph)的公开链接。 |
| **CD30** | 任何人都可以使用标准的通用工具，以可复现的方式构建代码。 | **是（YES）** Apache HugeGraph 提供了[快速入门文档](https://hugegraph.apache.org/cn/docs/quickstart/hugegraph/hugegraph-server/)，详细说明如何编译与构建源码。 |
| **CD40** | 项目代码的完整历史记录可通过版本控制系统获取，允许任何人重现任意已发布版本。 | **是（YES）** 项目使用 Git 进行版本控制，任何人都可以通过提交历史（commit logs）与每个发布版本的标签（tags）查看完整历史。 |
| **CD50** | 版本控制系统基于对提交者（Committer）的强身份认证，可靠地记录每一行代码的来源。当第三方贡献代码时，提交信息同样提供可靠的来源信息。 | **是（YES）** 项目使用由 Apache Infra 托管的 GitHub 仓库，确保每一行代码均可追溯至对应 Committer；第三方贡献严格遵循[贡献指南](https://hugegraph.apache.org/cn/docs/contribution-guidelines/)通过 Pull Request 审阅合入。 |

### 许可证与版权（LICENSE）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **LC10** | 已发布的代码采用 Apache License 2.0 协议授权。 | **是（YES）** 源码仓库中包含 [LICENSE](https://github.com/apache/hugegraph/blob/master/LICENSE) 文件；所有源码文件均包含 APLv2 许可证头，并在构建阶段由 Apache Rat 插件自动校验。 |
| **LC20** | 项目代码的必需依赖库不会产生比 Apache 许可证更严格的限制。 | **是（YES）** 所有第三方依赖均已完成许可证核查，不存在比 Apache License 2.0 更严格的附加限制。 |
| **LC30** | LC20 中提及的依赖库均作为开源软件公开可得。 | **是（YES）** 相关依赖库均可在公共 Maven 仓库中获取。 |
| **LC40** | 提交者（Committers）均受个人贡献者许可协议（"Apache iCLA"）约束，明确规定可提交的代码范围以及如何标识非本人原创的代码。 | **是（YES）** 所有 Committer 均已在 ASF 签署并备案 iCLA。 |
| **LC50** | 项目清晰定义并记录其产出的所有内容的版权归属。 | **是（YES）** 源码文件头部的版权声明与仓库根目录下的 NOTICE 文件对此进行了明确记录。 |

### 发布管理（Releases）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **RE10** | 发布产物包含源代码，并采用预期可长期读取的标准开放归档格式进行分发。 | **是（YES）** 源码发布包通过 [dist.apache.org](https://dist.apache.org/repos/dist/release/hugegraph/) 分发，并可在官网[下载页面](https://hugegraph.apache.org/cn/docs/download/download/)获取。 |
| **RE20** | 项目的项目管理委员会（PMC，见 CS10）批准每一次软件发布，使该发布成为基金会的正式行为。 | **是（YES）** 所有版本发布均在 `dev@hugegraph.apache.org` 邮件列表上由 PMC 投票表决通过。 |
| **RE30** | 发布包均附带数字签名和/或哈希摘要，供任何人可靠地校验下载归档的完整性。 | **是（YES）** 所有发布版本均由发布经理（Release Manager）签名并附带校验和，可通过 [KEYS](https://downloads.apache.org/hugegraph/KEYS) 文件进行验签。 |
| **RE40** | 项目可以在源码之外同时分发便利性二进制包（convenience binaries），但它们不属于 Apache 正式发布物，且不附带任何担保。 | **是（YES）** 项目提供便利性二进制包供用户快速体验，但仅源码归档包构成 Apache 官方正式发布。 |
| **RE50** | 项目记录了可重复执行的发布流程，使新加入的成员也能够独立生成发布所需的完整产物集合。 | **是（YES）** 项目的完整发布流程已记录在 [ASF Release Guidance V2.0](https://github.com/apache/hugegraph/wiki/ASF-Release-Guidance-V2.0) 指南中。 |

### 质量保障（Quality）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **QU10** | 项目对自身代码质量保持公开与诚实。只要清晰沟通，不同模块处于不同质量与成熟度阶段是自然且可接受的。 | **是（YES）** 鼓励用户在 GitHub 上[报告问题（Issues）](https://github.com/apache/hugegraph/issues)，所有技术讨论均公开透明。 |
| **QU20** | 项目将产出安全的软件置于极高优先级。 | **是（YES）** 所有报告的安全问题均按高优先级响应与处理。 |
| **QU30** | 项目提供文档完备、安全且私密的安全漏洞报告渠道，以及明确记录的响应流程。 | **是（YES）** 官方网站提供专门的[安全页面](https://hugegraph.apache.org/cn/docs/guides/security/)，说明安全漏洞的私密报告方式与响应机制。 |
| **QU40** | 项目高度重视向后兼容性，致力于记录任何不兼容变更，并提供工具与文档帮助用户平滑迁移至新特性。 | **是（YES）** 项目重视向后兼容性，任何破坏性变更均在版本发布说明（Release Notes）及文档中明确标注。 |
| **QU50** | 项目努力及时响应已有记录的缺陷报告。 | **是（YES）** 社区积极处理 GitHub 上提交的 Issue 以及邮件列表中的用户提问。 |

### 社区建设（Community）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **CO10** | 项目拥有广为人知的官方网站首页，指向按照本成熟度模型运作所需的全部信息。 | **是（YES）** [项目官网](https://hugegraph.apache.org/cn/)作为汇聚项目核心信息的中心入口。 |
| **CO20** | 社区欢迎任何怀有善意、彼此尊重并为项目创造价值的贡献者参与贡献。 | **是（YES）** Apache HugeGraph 设有[贡献指南](https://hugegraph.apache.org/cn/docs/contribution-guidelines/)，欢迎各类有价值的社区贡献。 |
| **CO30** | 贡献涵盖源代码、文档、建设性的缺陷报告、技术讨论、推广传播以及任何能够为项目创造价值的活动。 | **是（YES）** 项目同等重视代码贡献与非代码贡献。 |
| **CO40** | 社区坚持任人唯贤（Meritocracy），随着时间推移赋予持续为项目创造价值的贡献者更多权限与责任。 | **是（YES）** 社区遵循 Apache 之道（Apache Way），持续选拔活跃贡献者成为 Committer 与 PMC 成员。 |
| **CO50** | 项目记录贡献者如何获得更多权限（如提交权限或决策权），并一致地践行这些原则。 | **是（YES）** 成为 Committer 的标准与流程已在[提交者指南](https://hugegraph.apache.org/cn/docs/contribution-guidelines/committer-guidelines/)中明确列出。 |
| **CO60** | 社区基于拥有决策权的成员（见 CS10）的共识运作。无论是否仁慈，独裁者在 Apache 项目中均不受欢迎。 | **是（YES）** 所有重大决策均通过邮件列表公开讨论并达成共识。 |
| **CO70** | 项目努力及时解答用户问题。 | **是（YES）** 社区通过 `dev@hugegraph.apache.org` 邮件列表、[GitHub Issues](https://github.com/apache/hugegraph/issues) 及 [GitHub Discussions](https://github.com/apache/hugegraph/discussions) 为用户提供支持。 |

### 共识决策（Consensus）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **CS10** | 项目维护一份公开的拥有决策权的贡献者名单。项目的项目管理委员会（PMC）由这些贡献者组成。 | **是（YES）** 项目治理与成员名单可通过 ASF 委员会公开页面查阅，参见 [委员会信息](https://projects.apache.org/committee.html?hugegraph)。 |
| **CS20** | 决策需在 PMC 成员间达成共识，并记录在项目的主通信渠道上。PMC 会充分听取社区意见，但最终决定权归属 PMC。 | **是（YES）** 所有正式决策均在 `dev@hugegraph.apache.org` 邮件列表上通过投票做出，至少需要 3 名 PMC 成员投出 `+1` 票且无否决票（veto）。 |
| **CS30** | 当仅靠讨论不足以达成一致时，项目使用有据可查的投票规则来建立共识。 | **是（YES）** 项目严格遵循标准的 ASF 投票规则。 |
| **CS40** | 在 Apache 项目中，否决权（veto）仅对代码提交有效。行使否决权的人必须按照 CS30 定义的 Apache 投票规则给出技术解释。 | **是（YES）** HugeGraph 社区严格遵守这一原则。 |
| **CS50** | 所有“重要”讨论均以书面形式在项目主通信渠道上异步进行。影响项目的线下、面对面或私下讨论也必须记录在该渠道上。 | **是（YES）** 所有重要讨论与决定均记录在公开邮件列表中，确保透明与可追溯。 |

### 独立性（Independence）

| **ID** | **评估项描述** | **当前状态** |
| -------- | --------------- | ---------- |
| **IN10** | 项目独立于任何单一企业或组织的影响。 | **是（YES）** Apache HugeGraph 的 PMC 成员与 Committers 来自 10 余家不同企业、高校与科研机构，不存在任何单一实体控制项目的情况。 |
| **IN20** | 贡献者以个人身份参与社区行动，而非代表任何企业或组织。 | **是（YES）** 所有贡献者均以个人身份服务于项目与社区，而非代表其雇主。 |
