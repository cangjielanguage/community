# PMC例会第三次会议纪要

## 会议信息

**会议时间**: 2026-09-15

**参会人员 (Attendance)**: PMC 全体成员，列表详见 [PMC成员列表](https://gitcode.com/Cangjie/community/blob/main/cangjie_pmc/pmc.md#%E4%BB%93%E9%A2%89%E8%AF%AD%E8%A8%80-pmc-%E6%88%90%E5%91%98%E5%88%97%E8%A1%A8)

**议题**

| 序号 | 议题名称                         | 时长(分钟) | 汇报人   |
| ---- | ------------------------------- | ---------- | -------- |
| 1    | 技术课题管理方案评审                 | 30         | [胡晓明](https://gitcode.com/l3gi0n)   |
| 2    | 仓颉社区仓库管理方案评审             | 30         | [赵丹荣](https://gitcode.com/Leporide)   |
| 3    | PR/Issue/会议运营方案及工程方案评审  | 45         | [胡晓明](https://gitcode.com/l3gi0n)  |
| 4    | Cangjie Release Notes 建仓申请     | 10         | [刘军](https://gitcode.com/r4hl)     |
| 5    | cangjie_spec 建仓申请              | 10         | [傅荣枭](https://gitcode.com/RongxiaoFu)   |
| 6    | 社区问题多分支修复策略评审           | 15         | [王音强](https://gitcode.com/wyq1213)/[虞嘉豪](https://gitcode.com/ChaosJohn) |
| 7    | Cangjie STS 1.2.0 版本发布评审      | 15          | [刘军](https://gitcode.com/r4hl)     |

议题详情参见：[第三次PMC会议通知](../meeting_notices/thirdmeeting-notice.md)

## 会议纪要(Minutes of Meeting)

**议题1、技术课题管理方案评审**

汇报人：[胡晓明](https://gitcode.com/l3gi0n) 

会议结论：

1、同意当前技术课题处理流程。

2、技术课题揭榜轻流程运作，名单收集和汇总发布即可; 揭榜验收需要代码开源。

遗留问题：

1、社区组件、代码进入版本的机制和流程，以及后续的维护和演进。责任人：刘军/胡晓明；闭环时间：2026-10-15

**议题2、仓颉社区仓库管理方案评审**

汇报人：[赵丹荣](https://gitcode.com/Leporide)

会议结论：

1、整体同意建仓管理方案。

2、轻量化 cangjie-tpc 建仓流程，明确 TPC Team 管理范围和职责（评优、清退等）。

遗留问题：

1、讨论历史上的编程语言 SIG 的运作情况和后续处理策略。责任人：胡晓明/王学智；闭环时间：2026-10-15

2、刷新描述，明确组织定位与举例。责任人：赵丹荣；闭环时间：2026-10-15

3、流程发布后梳理历史代码仓的 team 归属。责任人：夏松/赵丹荣；闭环时间：2026-10-30

4、梳理轻量化 cangjie-tpc 建仓流程，不能要求先有代码再建仓。 责任人：夏松；闭环时间：2026-09-30

**议题3、PR/Issue/会议运营方案及工程方案评审**

汇报人：[胡晓明](https://gitcode.com/l3gi0n) 

会议结论：

1、不同意该方案，须对 Issue 和 PR 流程图中的各个分支流程进行计划后重新汇报。

2、须明确与社区开发者产生交互的所有节点。

**议题4、Cangjie Release Notes 建仓申请**

汇报人：[刘军](https://gitcode.com/r4hl) 

会议结论：

1、同意建仓，用于存放 release 相关的内容，仓库名称修改为 Cangjie Roadmap，并链接到社区首页显示。

**议题5、cangjie_spec 建仓申请**

汇报人：[傅荣枭](https://gitcode.com/RongxiaoFu)

会议结论：

1、同意 cangjie_spec 建仓。

2、Spec 的文本改进走仓库 Issue 流程（修 typo、改善语言表达等），但如果只是简单的改 typo 可以直接提 PR，由 Committer 检视后合入，不必关联 Issue。

3、Spec 特性提案跟随 CJEEP 流程（参见架构提案）。

遗留问题：

1、cangjie_spec 仓库使用的开源协议待与法务确认，当前考虑文档部分使用 CC-by-4.0，代码部分使用 Apache-2.0 with Runtime Library Exception。责任人：傅荣枭；闭环时间：待定

**议题6、社区问题多分支修复策略评审**

汇报人： [王音强](https://gitcode.com/wyq1213)/[虞嘉豪](https://gitcode.com/ChaosJohn)

会议结论：

1、同意采用缺陷类 Critical / Major / Minor "维护期内且受影响则默认合入"，建议类 Suggestion 历史维护版本默认不合入的问题分层原则。

2、同意安全问题统一采用"视 CVE 评分决定是否合入历史分支"的原则。

遗留问题：

1、兼容性在 LTS 和 STS 的处理原则需在架构完成决策，具体规则参照业界社区实践制定。责任人：王音强/虞嘉豪；闭环时间：待定

**议题7、Cangjie STS 1.2.0 版本发布评审**

汇报人：[刘军](https://gitcode.com/r4hl) 

会议结论：

1、同意发布 Cangjie STS 1.2.0 版本。

遗留问题：

1、修改 Release Notes 中错字、标点符号等问题。责任人：刘军；闭环时间：2026-09-16
