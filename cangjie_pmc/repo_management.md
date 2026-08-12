# 仓颉社区代码仓管理条例

## 一、 总则

### **1. 目的与背景**

为规范仓颉语言社区代码仓的建立、运作及日常管理，确保开发活动的高效有序，特制定本条例。

### **2. 适用范围**

本规范适用于仓颉社区内所有原生开发的代码仓。对于引入的第三方上游社区仓库，其管理原则应与上游社区保持一致。

### **3. 组织定位与仓库归属**

仓颉社区根据仓库性质与治理层级，将代码仓统一归口至下列三个 Gitcode 组织承载，建仓申请须首先明确目标归属组织：

- **[Cangjie](https://gitcode.com/Cangjie) 组织**：承载仓颉语言项目版本相关各 Team 作业仓库、仓颉社区章程和用户论坛仓库，以及持续维护的社区运作相关仓库。
- **[Cangjie-SIG](https://gitcode.com/Cangjie-SIG) 组织**：承载非三方库项目；开放邮件申请建仓申请途径，由 TPC Team 负责审核和管理。
- **[Cangjie-TPC](https://gitcode.com/Cangjie-TPC) 组织**：承载仓颉三方库、工具等项目；开放邮件申请建仓申请途径，由 TPC Team 负责审核和管理。

## 二、 代码仓建立与准入<a id="section2"></a>

### **1. 归口管理与建仓权限**

代码仓须归属于特定项目及对应组织。建仓申请路径按目标组织分级行使用例决策权：

- **Cangjie 组织建仓**：由 PMC 决策。建仓申请应由仓库责任人（Team Leader 或 Committer）向 PMC 提交议题，由 Team Leader 申请议题，可按需触发 PMC 例会进行评审。
- **Cangjie-SIG、Cangjie-TPC 组织建仓**：由 TPC Team 决策。建仓申请由仓库责任人向 TPC Team 提交，由 TPC Team 按其建仓模板与流程进行审核和管理。

### **2. 职责明确**

建仓申请须明确仓库的责任团队（Team 或社区运营办公室）及目标归属组织，经对应权限组织评审通过后，由授权管理员在相应组织下执行建仓：

- Cangjie 组织仓库经 PMC 评审通过后，由授权管理员在 [Cangjie](https://gitcode.com/Cangjie) 组织下执行建仓。
- Cangjie-SIG、Cangjie-TPC 组织仓库经 TPC Team 决策通过后，由授权管理员分别在 [Cangjie-SIG](https://gitcode.com/Cangjie-SIG)、[Cangjie-TPC](https://gitcode.com/Cangjie-TPC) 组织下执行建仓。

### **3. 分级审批准入**

- **版本主干仓库**：凡进入仓颉语言社区版本的仓库，必须经 PMC 评审后方可建立。
- **非版本主干仓库**：不进入仓颉语言社区版本的仓库，可在 Team 评审通过后先行建立；其中 Cangjie 组织仓库须向 PMC 备案并同步，Cangjie-SIG、Cangjie-TPC 组织仓库须向 TPC Team 备案并同步。
- **授权原则**：PMC 可根据实际治理需要，在其职权范围内授权仓库评审权限；Cangjie-SIG、Cangjie-TPC 组织的仓库评审权限由 TPC Team 行使。

## 三、 代码仓变更与迁移

### **1. 仓库变更申请（新增、退休、更名及开源引入）**

- **评审**：仓库变更评审按目标归属组织分级执行：
  - Cangjie 组织仓库（含版本主干仓库及社区运作相关仓库）的新增、退休、更名或外部开源软件的引入，须提交 PMC 进行专业评审；其中版本主干仓库相关操作必须经 PMC 评审。
  - Cangjie-SIG、Cangjie-TPC 组织仓库的新增、退休、更名或外部开源软件的引入，须提交 TPC Team 进行专业评审；非版本主干仓库相关操作可在所属 Team 内部处理并按第二章规定向对应权限组织备案。

- **执行路径**：
	- **申请流程**：评审通过后，申请人须根据变更需求发起申请；其中 Cangjie 组织仓库由 Team Leader 向 PMC 申报议题，通过 PMC 会议评审后执行；Cangjie-SIG、Cangjie-TPC 组织仓库按对应组织的建仓申请模板发送邮件至 [contact@cangjie-lang.net](contact@cangjie-lang.net) 办理。
  
	- **联系渠道**：新增、退休或更名操作须统一通过联系 [contact@cangjie-lang.net](contact@cangjie-lang.net) 进行确认与后台处理。
