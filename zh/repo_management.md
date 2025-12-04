# 仓颉社区代码仓管理

&nbsp;&nbsp;&nbsp;&nbsp;本文用于规范仓颉社区代码仓建立和管理活动，保证开发活动有序，提升开发效率。


## 适用范围
&nbsp;&nbsp;&nbsp;&nbsp;本规范适用于仓颉社区所有原生代码仓。引入的上游社区仓库，保持和上游一致。

## 代码仓建立
&nbsp;&nbsp;&nbsp;&nbsp;代码仓必须归属于某个项目，所以建仓需要由该项目向`PMC`提交申请，`PMC`评审通过后，建立仓库。

## 代码仓毕业



## 代码仓运作

&nbsp;&nbsp;&nbsp;&nbsp;代码仓配置主要有如下四部分：基础设置、权限、仓库管理、分支管理、服务集成：

![仓库配置](pictures\仓库配置.PNG "Project Config")   

### 基础配置

#### 代码仓命名
&nbsp;&nbsp;&nbsp;&nbsp;建议代码仓采用`cangjie_`开头的方式进行命名，单词使用小写开头，单词之间采用下划线分隔；例如：仓颉跨平台互操作仓库名字为`cangjie_multiplatform_interop`

#### 其他配置
&nbsp;&nbsp;&nbsp;&nbsp;默认分支选择开发分支（默认为**main**，详细分支策略参考分支管理章节），项目模块取消勾选wiki及安全漏洞(成体系的文档应通过专门的资料代码或者资料文档仓库管理，没有明确的wiki用途使用，禁止勾选，可基于明确用途CMC评审备案后打开。漏洞通过仓颉官网专门邮件途径反馈)。

![基础配置](pictures\基础配置.PNG "Project module")    


### 角色与权限
&nbsp;&nbsp;&nbsp;&nbsp; 仓颉社区代码仓主要角色包含Developer 和 Commiter，其中Developer至少需要配置如下权限：


![Developer权限](pictures\Developer权限.PNG "Developer")   

Commiter需要配置如下权限：

![Commiter权限](pictures\Commiter权限.PNG "Commiter")   

### 仓库管理

&nbsp;&nbsp;&nbsp;&nbsp;仓颉社区采取fork开发工作流，所以仓库建议禁止开发者创建分支：

   ![仓库管理](pictures\仓库管理.png "Repo manage")   

#### 分支命名

&nbsp;&nbsp;&nbsp;&nbsp;分支命名需尽量表达分支的作用；建议使用feature/bugfix/release开头，后接字母或数字。其正则表达如下：

    ^(feature|bugfix|release)/[a-z0-9.-]+$

*注*：一般情况下不允许创建单独分支，特殊情况，需`PMC`评审通过方可创建。

发布分支命名以`release`开头，后跟版本号，例如下：release/v1.0.0.

仓库默认使用dev分支做开发，main分支做版本发布，这两个分支不用遵守分支命名规则。


#### Tag命名
&nbsp;&nbsp;&nbsp;&nbsp;`Tag`和社区版本相一一对应，所以Tag号规则同版本号，其正则表达式如下：
    
    ^v(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*)(?:-([a-zA-Z0-9-]+))?$
 
格式为： v<主版本>.<次版本>.<修订版本>-先行版本号(可选)

示例： V1.2.3-alpha

例外：`stdx`为扩展库，其版本命名风格跟其他工程权限有所差异

    ^v(0|[1-9]\d*)\.(0|[1-9]\d*)\.(0|[1-9]\d*).(0|[1-9]\d*)(?:-([a-zA-Z0-9-]+))?$
 
`stdx`具有四位版本号，因此采用上述规则。

#### 提交设置

&nbsp;&nbsp;&nbsp;&nbsp;社区提交log建议采用[conventional commits 通用提交规范](https://www.conventionalcommits.org/zh-hans/v1.0.0/)


仓库检查正则配置如下：

    ^(?<type>feat|fix|docs|style|refactor|test|chore|perf|build|ci|revert)(\((?<scope>[\w\-]+)\))?!?:\s(?<description>.{1,72})$
 
仓库提交文件限制建议限制在100M以内，且禁止强制推送

 ![提交设置](pictures\提交设置.png "Request Config")  

 #### 保护分支

 &nbsp;&nbsp;&nbsp;&nbsp;建议至少将默认开发和发布分支设置为保护分支；其余请根据需要进行设置，例如可以将`LTS`版本分支设置为保护分支。

![保护分支](pictures\保护分支.png "Protect Branch")  

### Pull Request 设置

#### 合入条件
&nbsp;&nbsp;&nbsp;&nbsp;PR至少需要两个评审人评审方可合入，评审人需为项目Developer或者Commiter。检视发现的问题必须全部解决后合入，严禁未经确认直接将检视意见标记为解决。必须在流水线通过后合入。

![合入条件](pictures\合入条件.png "Merge Request")  

#### CLA协议设置

&nbsp;&nbsp;&nbsp;&nbsp;社区的仓库需要全勾选，并配置该协议。


![CLA 协议](pictures\CLA协议.png "CLA")  

##### Pull Requests 设置
&nbsp;&nbsp;&nbsp;&nbsp;禁止自提自合、且不允许强制合入. 仓颉社区采用fork工作流，所以所有MR必须通过fork方式合入。PR合并后允许继续做代码检视和评论，持续提升代码质量。

![Pull Request](pictures\PullRequests设置.png "Pull Request")  

#### Squash设置

&nbsp;&nbsp;&nbsp;&nbsp;为了保留项目的原始提交信息，建议禁止Squash合并。


![Squash](pictures\Squash合并.png "Squash")


#### PR审查设置

&nbsp;&nbsp;&nbsp;&nbsp;最小审查通过人数为1人，审查人必须为committer。

![PR审查](pictures\PR审查.png "PR")