# 仓颉PMC的责任细则

本文档旨在为仓颉语言社区提供PMC的具体角色细则。

## 一、概述

仓颉语言项目管理委员会（PMC：Project Management Committee）是仓颉项目群技术指导委员会下设组织，负责仓颉语言开源项目的管理，职责如下：

1. 负责仓颉语言项目的管理工作，包括开源社区版本规划、架构看护、特性代码开发维护、版本及补丁规划等；
2. 发布和处理仓颉语言项目的需求，为开源社区提供技术架构指导和技术决策；
3. 处理仓颉语言项目的Bug、Issue、邮件列表等渠道开发者反馈问题；
4. 负责仓颉语言PMC、Committer成员的选举和退出，制定仓颉语言项目的PMC、Committer协作机制；

## 二、仓颉语言 PMC关键角色


| 领域     | 职责定义                                                    |
| -------- | :----------------------------------------------------------- |
| PMC主席  | 负责仓颉语言PMC整体技术治理和管理；<br/>主持仓颉语言PMC、Committer新成员的选举和退出，以及社区协作机制；<br/>召集和主持PMC会议，并检查PMC会议决议的落实情况；<br/>代表PMC或委派PMC成员参与仓颉项目群周边组织会议，以及外部技术交流活动，提升社区影响力。 |
| Architecture Team | 负责仓颉语言技术架构的顶层分析、设计和关键技术识别；<br/>负责评审仓颉语言重大技术方案和技术架构变更；<br/>负责对技术争议和设计方案冲突进行裁决、对跨组件影响的技术方案进行协调。 |
| Specification Team     | 仓颉语言SPEC分析和关键技术识别，对应领域特性标准撰写及维护; <br/>负责仓颉语言SPEC设计的技术评审，技术决策以及关键技术问题解决; <br/>负责仓颉语言SPEC相关的社区需求规划和梳理对应领域的共建需求梳理; <br/>代表仓颉语言SPEC设计领域参加仓颉社区的峰会和布道。|
| Compiler Team     | 负责编译器技术领域的竞争力分析、关键技术识别与突破，主导功能分解、接口定义与维护管理，构建高性能、可扩展的编译器架构； <br/>主导系统设计方案评审与技术决策，解决关键技术问题，确保技术方案与架构的先进性与可行性； <br/>统筹代码开发、维护及质量保障，通过架构设计与代码审核，推动高质量代码合入主干； <br/>规划社区需求技术方案，梳理共建需求，推动开源社区问题闭环与技术方案落地；<br/>代表团队参与仓颉社区峰会，输出技术成果，分享编译器领域最佳实践，提升技术影响力，推动开源生态繁荣。|
|Runtime Team| 运行时技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等; <br/>负责运行时技术领域系统设计方案的技术评审，技术决策，模块关键技术问题解决; <br/>负责运行时技术领域的社区需求技术规划和梳理对应领域的共建需求梳理;<br/>代表运行时技术领域参加仓颉社区的峰会和布道。|
|Libs Team| 语言库技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等; <br/>负责语言库领域系统设计方案的技术评审，技术决策，模块关键技术问题解决; <br/>负责语言库技术领域的社区需求技术规划和梳理对应领域的共建需求梳理; <br/>代表语言库技术领域参加仓颉社区的峰会和布道。|
|Multi-platform Team| 仓颉语言跨平台能力构建分析和关键技术识别，对应领域特性标准撰写及维护; <br/>负责仓颉跨平台领域系统设计的技术评审，技术决策以及关键技术问题解决; <br/>负责仓颉跨平台领域相关的社区需求规划和梳理对应领域的共建需求梳理; <br/>代表仓颉跨平台领域参加仓颉社区的峰会和布道。|
|Tools Team| 工具链技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等; <br/>负责工具链技术领域系统设计方案的技术评审，技术决策，模块关键技术问题解决; <br/>负责工具链技术领域的社区需求技术规划和梳理对应领域的共建需求梳理; <br/>代表工具链技术领域参加仓颉社区的峰会和布道。|
|IDE Team| 仓颉IDE技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等;<br/>负责仓颉IDE技术领域系统设计方案的技术评审，技术决策，模块关键技术问题解决;<br/>负责仓颉IDE技术领域的社区需求技术规划和梳理对应领域的共建需求梳理;<br/>代表仓颉IDE技术领域参加仓颉社区的峰会和布道。|
|Security Team|安全技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等;<br/>负责安全技术领域系统设计方案的技术评审，技术决策，模块关键技术问题解决;<br/>负责安全技术领域的社区需求技术规划和梳理对应领域的共建需求梳理;<br/>代表安全技术领域参加仓颉社区的峰会和布道。|
|Release Team | 负责版本时间表制定和发布，在开发/测试周期中跟踪版本交付特性状态；<br/>组织发布相关评审，协调QA，发布工程师，技术委员会等参与发布相关会议完成版本发布评估；<br/> 负责项目交付过程的协调。|
| QA Team | QA团队的目标是负责社区开发、治理、运营等流程规范的制定和发布；<br/>制定社区奖惩机制，例行跟踪社区运营问题。|
| Test Team | 构建社区测试能力，让更多的社区开发者参与、贡献构建仓颉编程语言测试能力；<br/>根据版本计划制定测试计划、规划测试活动，看护版本关键软件包质量；<br/>参与制定、维护发布标准，参与管理发布过程，决策阻塞问题和关键缺陷的修复计划。|
|  Infrastructure Team  | 安全CICD领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等; <br/>负责CICD领域系统设计方案的技术评审，技术决策，模块关键技术问题解决; <br/>负责CICD领域的社区需求技术规划和梳理对应领域的共建需求梳理。|
| Document Team  | 文档规划和信息架构设计、文档版本生命周期管理，风格指南等质量保证和标准化规范制定、文档贡献流程建设、文档维护更新、审核文档、响应并处理社区文档问题反馈。|
|InterOp Team|  负责互操作技术领域的竞争力分析、关键技术识别与突破，主导功能分解、接口定义与维护管理，构建易用、高性能的互操作能力；<br/>主导系统设计方案评审与技术决策，解决关键技术问题，确保技术方案与架构的先进性与可行性；<br/>统筹互操作领域代码开发、维护及质量保障，通过架构设计与代码审核，推动高质量代码合入主干；<br/>规划互操作社区需求技术方案，梳理共建需求，推动开源社区问题闭环与技术方案落地；|
|TPC Team|  三方库技术领域竞争力分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码开发维护等; <br/>负责三方库领域系统设计方案的技术评审，技术决策，模块关键技术问题解决;<br/>负责三方库技术领域的社区需求技术规划和梳理对应领域的共建需求梳理;<br/>代表三方库技术领域参加仓颉社区的峰会和布道。|
|AIAgent Team|  负责仓颉面向Agent开发底座能力构建，负责仓颉面向AI Agent领域竞争力分析、关键技术识别与突破；<br/>负责仓颉面向Agent编程Agent DSL设计与实现；<br/>负责Agent开发底座功能开发与实现；<br/>负责Agent领域社区影响力建设；|



## 仓颉语言 PMC 成员列表
首届仓颉语言项目管理委员会（PMC）成员由华为选举并委派十二名代表和四名企业代表担当，后续成员由现任提议，通过投票决定。


| 姓名   | 账号                                  | 角色    | 领域                 |
| ------ | ------------------------------------- | ------- | ------------------- |
| 冯新宇 | [@thumb](https://gitcode.com/thumb) | PMC主席 | 总架构师、Architecture Team、Specification Team |
| 董鑫 | [@seanXDO](https://gitcode.com/seanXDO) | PMC成员 | 项目代表 |
| 徐潇 | [@shawn_xuxiao](https://gitcode.com/shawn_xuxiao) | PMC成员 | 仓颉终端架构师 |
| 吴家文 | [@Timi3](https://gitcode.com/timi3) | PMC成员 | Compiler Team       |
| 傅舟   | [@binaryfz](https://gitcode.com/binaryfz) | PMC成员 | Runtime Team        |
| 查君鹏/虞嘉豪 | [@ZhaJunpeng](https://gitcode.com/zhajunpeng) / [@ChaosJohn](https://gitcode.com/ChaosJohn) | PMC成员 | Libs Team  |
| 朱凯迪 | [@Boommmmmm](https://gitcode.com/Boommmmmm) | PMC成员 | Multi-platform Team |
| 刘晓莹 | [@liuxiaoying](https://gitcode.com/gcw_soeAfXvg) | PMC成员 | QA Team |
| 刘天瑜/胡彬彬 | [@BestLeon](https://gitcode.com/bestleon) / [@Gcourage](https://gitcode.com/Gcourage) | PMC成员 | Test Team             |
| 胡晓明/张俊 | [@l3gi0n](https://gitcode.com/l3gi0n) / [@zjdd](https://gitcode.com/zjdd) | PMC成员 | Tools Team          |
| 周广宇 | [@Timzhou](https://gitcode.com/Timzhou) | PMC成员 | IDE Team            |
|李卓远/虞嘉豪 | [@zhuoyuanli](https://gitcode.com/zhuoyuanli) / [@ChaosJohn](https://gitcode.com/ChaosJohn) | PMC成员 | Security Team       |
| 朱艳婷 | [@amy_mayun](https://gitcode.com/amy_mayun) | PMC成员 | Document Team       |
| 夏松 | [@xdst ](https://gitcode.com/xdst ) | PMC成员 | TPC Team |
| 周晶 | [@zhoujing106 ](https://gitcode.com/zhoujing106) | PMC成员 | Infrastructure Team |
| 曾维林/刘军 | [@frank83](https://gitcode.com/frank83) / [@r4hl](https://gitcode.com/r4hl) | PMC成员 | Release Team        |
| 轩加振 | [@xuanjz](https://gitcode.com/xuanjz) | PMC成员 | InterOp Team       |
| 杨典 | [@ydgzb](https://gitcode.com/ydgzb) | PMC成员 |AI Agent  Team       |


# 相关管理制度

- [仓颉社区版本管理](https://gitcode.com/Cangjie/community/blob/main/cangjie_pmc/version_management.md)
- [提案管理](https://gitcode.com/Cangjie/community/blob/main/cangjie_pmc/proposal_management.md)
- [仓颉社区代码仓管理](https://gitcode.com/Cangjie/community/blob/main/cangjie_pmc/repo_management.md)
- [成长路径](https://gitcode.com/EricHaHaHaHa/community/blob/main/cangjie_pmc/promotion.md)
- [Team管理制度与操作指南](https://gitcode.com/Cangjie/community/blob/main/team/README_zh.md)

