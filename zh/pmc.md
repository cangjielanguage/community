# 仓颉PMC的责任细则

本文档旨在为仓颉语言社区提供PMC的具体角色细则

## 一、概述

仓颉语言项目管理委员会（PMC：Project Management Committee）是仓颉项目群技术指导委员会下设组织，负责仓颉语言开源项目的管理，职责如下：

1. 负责仓颉语言项目的管理工作，包括开源社区版本规划、架构看护、特性代码开发维护、版本及补丁规划等；
2. 发布和处理仓颉语言项目的需求，为开源社区提供技术架构指导和技术决策；
3. 处理仓颉语言项目的Bug、issue、邮件列表等渠道开发者反馈问题；
4. 负责仓颉语言PMC、Committer成员的选举和退出，制定仓颉语言项目的PMC、Committer协作机制；

## 二、仓颉语言 PMC关键角色


| 领域     | 职责定义                                                     | 维护的流程和社区规则                                         |
| -------- | :----------------------------------------------------------- | ------------------------------------------------------------ |
| PMC主席  | 负责仓颉语言PMC整体技术治理和管理；<br />主持仓颉语言PMC、Committer新成员的选举和退出，以及社区协作机制；<br/>召集和主持PMC会议，并检查PMC会议决议的落实情况；<br/>代表PMC或委派PMC成员参与仓颉项目群周边组织会议，以及外部技术交流活动，提升社区影响力。 | 新技术项目引入和孵化流程；<br/>软件包选型引入和退出决策流程；<br/>仓颉语言PMC技术治理和运作规范流程；<br/>仓颉语言PMC版本GO/NO-GO决策流程。 |
| Specification Team     | 领域Team管理工作：包括跨领域间技术竞争分析和关键技术识别，Team领域间接口定义与维护跨Team间架构设计变更的评审和最终决策；<br/>负责跨Team领域间接口变更的联合评审和决策；<br/>架构设计原则制定，架构变更和看护。 | Team领域间技术孵化流程；<br/>Team领域间技术决策流程；<br/>代码仓新建、孵化、退休和毕业。 |
| Compiler/Run Time/Stand Libs/Multi-platform/Tools/IDE/Security Team     | 负责各自Team领域竞争分析和关键技术识别，功能分解分配，模块间接口定义与维护管理，对应领域特性代码仓开发维护等; <br/>负责Team领域系统设计方案的技术评审，技术决策，模块关键技术问题解决；<br/>负责各自Team领域的社区需求技术规划和梳理对应领域的共建需求梳理； <br/>代表各自Team领域参加仓颉语言相关的技术峰会和布道。| 各自Team领域间技术孵化流程；<br/>Team领域间技术决策流程；<br/>代码仓新建、孵化、退休和毕业。 |
|Release Team | 规划和计划版本的发行时间表；<br/>在开发/测试周期中跟踪（更新updates或功能feature）的开发状态；<br/>版本发布协调，参与相关组和发布相关等会议；<br/>负责项目的交付过程协调。 | 仓颉语言PMC版本发布流程；<br/>仓颉语言PMC版本发行时间表；<br/>仓颉语言PMC版本补丁发布流程和生命周期策略说明。 |
| QA Team | 负责Team项目孵化准出的质量标准制定；<br/>负责社区开发、治理、运营等流程规范的制定和发布；<br/>制定社区奖惩机制，例行跟踪社区运营问题，并定期在仓颉语言PMC例会汇报关键角色参与社区治理情况。 | Team项目孵化流程规范制定；<br/>仓颉语言PMC开发、治理和运营等流程规范制定和发布。 |
|  Infrastructure Team  | 支持仓颉语言PMC构建发布工具基础架构/发布工程的工具环境；<br/>支持仓颉语言PMC工具应用程序维护；<br/>支持仓颉语言PMC沟通交流和社区运营监控平台；<br/>制定仓颉语言PMC的基础设施发展计划。 | 构建工具使用指导；<br/>仓颉语言PMC通信使用指导。  |
| Document Team  | 支持仓颉语言PMC文档全流程管理：负责文档的创建、更新、发布及归档，确保内容准确、版本与产品同步，维护多语言文档的一致性，满足全球化需求；<br/>跨团队协作：联动各个Team，同步技术细节与功能描述，保证文档与各Team的代码一致性；<br/>用户反馈闭环：收集并分析用户反馈（如评论、搜索数据），持续优化文档质量与结构。 | 文档构建使用指导；<br/>仓颉语言PMC通信使用指导。  |
|Industry Team（待定）|  各应用厂商提出针对跨平台框架及三方库的需求，并且支持在达成一致后落入版本计划；<br/>引入更多企业资源参与到跨平台框架的实践与共建。|待定|
|Academic Team（待定）|  推动跨平台框架与三方库的技术创新与突破；<br/>引入更多高校资源参与到跨平台框架的实践与共建。|待定|
 

## 仓颉语言 PMC 成员列表
首届仓颉语言项目管理委员会（PMC）成员由华为选举并委派十二名代表和四名企业代表担当，后续成员由现任提议，通过投票决定。


| 姓名   | 账号                                  | 角色    | 领域                 |
| ------ | ------------------------------------- | ------- | ------------------- |
| 冯新宇 |                                       | PMC主席 | 总架构               |
| 冯新宇 |                                       | PMC成员 | Specification Team  |
| 涂玏   |                                       | PMC成员 | Compiler Team       |
| 傅舟   |                                       | PMC成员 | Runtime Team        |
| 查君鹏 |                                       | PMC成员 | Standard Libs Team  |
| 朱佳梦 |                                       | PMC成员 | Multi-platform Team |
| 刘天瑜 |                                       | PMC成员 | QA Team             |
| 胡晓明 | [@l3gi0n](https://gitcode.com/l3gi0n) | PMC成员 | Tools Team          |
| 周广宇 |                                       | PMC成员 | IDE Team            |
| 胡晓明 | [@l3gi0n](https://gitcode.com/l3gi0n) | PMC成员 | Security Team       |
| 朱艳婷 |                                       | PMC成员 | Document Team       |
| 麻赛军 |                                       | PMC成员 | Infrastructure Team |
| 曾维林 |                                       | PMC成员 | Release Team        |
| 待定 |                                           | PMC成员 | Industry Team        |
| 待定 |                                           | PMC成员 | Academic Team        |

# 相关管理制度

- [仓颉社区版本管理](https://gitcode.com/Cangjie/community/blob/main/zh/version_management.md)
- [提案管理](https://gitcode.com/Cangjie/community/blob/main/zh/proposal_management.md)
- [仓颉社区代码仓管理](https://gitcode.com/Cangjie/community/blob/main/zh/repo_management.md)
- [成长路径](https://gitcode.com/EricHaHaHaHa/community/blob/main/zh/promotion.md)
- [Team管理制度与操作指南](https://gitcode.com/EricHaHaHaHa/CJ_PMC_TEAM/blob/main/Team/Team_rules_and_regulations/rules_and_regulations.md)

