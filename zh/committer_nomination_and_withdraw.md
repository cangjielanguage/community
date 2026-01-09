## 完整的Committer推举/退出以及添加/删除Committer权限的完整流程如下：

![Committer推举/退出流程](./figures/committer_change_flow.png)

### 1. 推举/退出Committer邮件模板：

- 邮件标题：[VOTING] New Committer [Approver/Reviewer] Nonimation xxx / Withdrawal Committer [Approver/Reviewer] xxx

- 邮件正文
  #### 1.1 概述：

  **推举概述示例：**
  ```
  xxx_Team的Committer gitcode_id (email address) 提名 gitcode_id (email address) 为 repository_address仓的社区Committer。
  xxx 个人贡献的简要一句话介绍。请大家回复邮件投票，赞成请回复 +1，不赞成请回复 -1 及不赞成原因。
  ```

  **退出概述示例：**
  ```
  由于工作变动，申请退出 xxx 仓库committer
  ```

  #### 1.2 贡献举证：

  - **PR 贡献**（实质代码贡献的链接）：
    - [PR 1](https://gitcode.com/Cangjie/community/pull/1)
    - [PR 2](https://gitcode.com/Cangjie/community/pull/2)
    - ...

  - **PR 有效检视** (参与仓颉语言社区代码有效评论意见的链接)：
    - [Review 1](https://gitcode.com/Cangjie/community/pull/1)
    - [Review 2](https://gitcode.com/Cangjie/community/pull/2)
    - ...

  - **参与XXX社区推广**：
    - [文章链接](https://mp.weixin.qq.com/s/zLNukoY1iDKCbOHuVI0D8w)

  - **参与技术峰会**：
    202x年 参加仓颉语言开发者大会、仓颉语言技术峰会、开放原子全球开源峰会的 **《XXX议题》**

### 2. 收到公示邮件后，回复相关信息到pmc邮件列表

- 邮件标题格式：Information confirm // [New Committer] Welcoming to become committer of Cangjie xxxTeam project : xxx

- 邮件正文：
```
  1. Cangjie xxxTeam Repository:
    - [Repository 1](https://gitcode.com/Cangjie/community/tree/main/team/team_tools)
    - ...

  2. My name: [中文名拼音全拼/Chinese romanization]
  3. gitcode id url: [gitcode id的链接](https://gitcode.com/xxx)
  4. gitcode id associated email: [个人企业邮箱/Enterprise Email], 若是个人贡献者可以填写自己关联gitcode的个人邮箱

  ```

### 3. 在Team管理平台提交committer新增/退出申请

1. 用gitcode帐号登录仓库管理平台：[仓管理](待定)
2. 仓路径筛选自己需要申请的仓库;
3. 在弹出的“仓信息修改”中填写：
    - **Committer列表**：输入自己的 gitcode帐号（为了社区沟通和开发者沟通，要求关联邮箱公开可获取）
    - **会议记录**：填写dev 邮件公示的会议纪要链接，例如 [会议纪要链接](待定)
