# 贡献流程<a name="ZH-CN_TOPIC_0000001052970939"></a>

## 环境准备<a name="section124971410183614"></a>

-   针对Git的安装、环境配置及使用方法，请参考GitCode帮助中心的Git知识大全：[https://docs.gitcode.com/docs/help/home/general-reference/git](https://docs.gitcode.com/docs/help/home/general-reference/git)
-   注册SSH公钥，请参考GitCode帮助中心的公钥管理：[https://docs.gitcode.com/docs/help/home/user_center/security_management/ssh](https://docs.gitcode.com/docs/help/home/user_center/security_management/ssh)
-   在开展GitCode的工作流之前，您需要先在Cangjie的代码托管平台上找到您感兴趣的Repository。

## 代码下载<a name="section6125202333611"></a>

### 从云上Fork代码分支<a name="section8365811818"></a>

1.  找到并打开对应Repository的首页。
2.  点击右上角的 Fork 按钮，按照指引，建立一个属于**个人**的云上Fork分支。

###  把Fork仓下载到本地<a name="section49051646201819"></a>

请按照以下的过程将Repository内的代码下载到您的在计算机上：

1.  **创建本地工作目录**：

    您需要创建本地工作目录，以便于本地代码的查找和管理

    ```
    mkdir ${your_working_dir}
    ```

2.  **复制远程仓库到本地**
    1.  **切换到本地路径**

        ```
        mkdir -p ${your_working_dir}
        cd ${your_working_dir}
        ```

    2.  **复制远程仓库到本地**
        -   您可以在仓库页面内复制远程仓库的拷贝地址，得到`$remote\_link`：

            **图 1**  复制远程仓库
            
            ![image.png](https://raw.gitcode.com/user-images/assets/3162607/83364454-06ef-4f0c-a991-45855679528c/image.png 'image.png')

        -   在本地电脑执行拷贝命令：

            ```
            git clone $remote_link
            ```

### 代码提交\(git clone场景\)<a name="section669715742719"></a>

1.  **拉分支**

    更新您的本地分支

    ```
    git remote add origin $remote_link
    git fetch origin
    git checkout master  
    git pull --rebase 
    ```

    基于远端master分支拉取本地调试分支

    ```
    git branch myfeature origin/master
    git checkout myfeature  
    ```

    然后在myfeature分支上编辑和修改代码。

2. **在本地工作目录提交变更**

   ```
   git add xxx
   git commit -sm  "feat: xxx"  // 提交信息包含signoff邮箱
   ```
   您可能会在前次提交的基础上，继续编辑构建并测试更多内容，可以使用commit --amend继续添加提交。
   提交信息采用 [Conventional Commits（约定式提交规范）](https://www.conventionalcommits.org/zh-hans/v1.0.0/)，一个复杂点的 commit 格式参考如下：
   ```
   feat: add some new features

   Add xx feature for xxx, it can xxxx.

   Add xx feature for xxx, it can xxxx.

   Refs: #12

   Assisted-by: Opencode
   Signed-off-by: xxx <xxx@xxx.com>
   ```
   
   更多 commit 风格信息参考[Conventional Commits（约定式提交规范）](https://www.conventionalcommits.org/zh-hans/v1.0.0/)。

   在仓颉社区的开源代码贡献规范中，如果您使用了 AI 工具辅助编写代码，须在 commit 末尾强制标注 `Assisted-by` 标签以明确 AI 的辅助贡献。格式如下：

   ```
   Assisted-by: <AI工具名称>   # 例如：Assisted-by: Opencode
   Signed-off-by: xxx <xxx@xxx.com>
   ```

   > **注意**：人类开发者必须对 AI 生成的每一行代码进行审查，确保其在功能、安全和许可证（License）合规上完全符合规范。若代码部署后出现漏洞或版权纠纷，最终责任由提供 `Signed-off-by` 的人类提交者承担。

3.  **将变更推送到您的远端目录**

    准备进行审查（或只是建立工作的异地备份）时，将分支推到您的fork仓库:

    ```
    git push -f origin myfeature
    ```

## Pull Request与门禁操作<a name="section28261522124316"></a>

### 完整流程概览

<img src="image/贡献总览.png" alt="贡献总览" style="zoom:75%;" />

### 关键步骤说明

1. **基础准备**

- Fork 目标仓库，拉取至本地。
- 基于仓库dev分支开发，代码修改完成后提交到 Fork 仓。
- 仓库列表：
    - https://gitcode.com/Cangjie/cangjie_compiler    # 仓颉编译器仓库
    - https://gitcode.com/Cangjie/cangjie_runtime     # 仓颉运行时&标准库仓库
    - https://gitcode.com/Cangjie/cangjie_tools       # 仓颉工具链仓库
    - https://gitcode.com/Cangjie/cangjie_stdx        # 仓颉扩展库仓库
    - https://gitcode.com/Cangjie/llvm-project        # LLVM项目仓库（仓颉依赖）
    - https://gitcode.com/Cangjie/cangjie_test        # 仓颉测试用例仓库
    - https://gitcode.com/Cangjie/cangjie_test_framework  # 仓颉测试框架仓库

2. **Issue创建**

- 创建 Issue：在任意仓库创建 Issue 即可，请务必按照模板认真填写，必填项不要为空。

3. **PR创建**

- 创建 PR：
    - 单仓修改：从个人仓库分支向目标仓库 dev 分支创建 PR。
    - 多仓修改：为涉及的每个仓库分别创建 PR。
  
  - **重要提示**：
    - PR 都有模板，请务必按照模板认真填写，必填项不要为空。
    - 根据PR 模板中要求，在对应位置附上 Issue 链接可以自动关联 Issue，不需要再额外手动设置关联。
   
- **PR创建成功通知**：

    当您成功创建 Pull Request（PR）后，系统会自动回复以下通知信息：

    ```
    PR创建成功通知 | 感谢您的贡献 🎉
    
    您好！系统已检测到您成功创建 Pull Request（PR），感谢您对项目的支持与参与！以下几点需要您着重关注：
    
    一、PR必须关联Issue ❗
    
    触发门禁检查的必要步骤：在PR描述框输入Issue完整链接，完成Issue关联。
    
    请注意，一个 Issue 不能同时关联同一 base 仓库内的多个开启状态的 PR
    
    二、门禁触发规则 🔧
    
    门禁类型判定：由Issue关联的PR所属代码仓数量决定
    
    关联多个代码仓PR：触发「多仓联合门禁」
    
    关联单个代码仓PR：触发「单仓门禁」
    
    启动指令与检查范围：需主动回复指令：
    
    回复 "start build"：执行Cangjie的主要基础检查，包含commit格式检查、静态告警分析、多平台构建、测试等
    
    关联同一issue的多个PR，仅需在任意一个PR里回复触发一次门禁，该PR门禁通过后，所有PR都会添加Label和测试人
    
    每个pr只能同时运行一条CI流水线，如需重新启动，请先关闭运行中的，再评论触发门禁
    
    Markdown修改仅触发文档类构建测试门禁，不会触发Cangjie的编译测试门禁
    
    commit 信息格式请遵循：Conventional Commits 规范
    
    请保证每一条 commit 都已添加 Signed-Off-By 信息
    
    三、合入条件 ⚠️
    
    满足最低评审人数，且评审问题需全部解决；
    
    禁止合入本人创建的PR，需由其他协作者操作；
    
    合并前确保关联流水线任务运行成功（build-test-passed）。
    
    四、合并PR ✅
    
    回复 "start merge"，CI流水线会自动检查所有关联PR的状态，若所有PR都满足合并条件，则将会同时合并所有PR。若存在不满足合并条件的PR，则不会合并任何PR。
    
    五、补充说明 📢
    
    详细仓颉贡献流程：贡献流程(Cangjie Community Contribution)
    
    门禁结果将自动评论至关联的所有PR，敬请留意。
    ```

4. **PR关联操作**

- **关联方式**：
    - 在 PR 描述根据模板要求输入 Issue 完整链接，完成 Issue 关联（推荐方式，可自动关联）。
    
- **关联规则**：
    - 多仓修改时，多个仓的所有 PR 需关联同一个 Issue。
    - 请注意，一个 Issue 不能同时关联同一 base 仓库内的多个开启状态的 PR。

  <img src="image/relate_pr.png" alt="relate_pr" style="zoom:80%;" />

5. **门禁触发**

- **门禁类型判定**：
    - 由 Issue 关联的 PR 所属代码仓数量决定：
        - 关联多个代码仓 PR：触发「多仓联合门禁」
        - 关联单个代码仓 PR：触发「单仓门禁」
    - 多仓联合门禁：关联同一个 Issue 的 PR 会联合构建，如 cangjie_compiler、cangjie_runtime、cangjie_test 三个仓的三个 PR 关联了同一个 Issue，那么在运行门禁时，它们会进行联合构建和测试。
    
- **触发方式**：
    - 在任意关联 PR 的评论区回复指令：
        - 回复 "**start build**"：执行 Cangjie 的主要基础检查，包含 commit 格式检查、静态告警分析、多平台构建、测试等（推荐）
        - （内测中）回复 "**start full build**"：启动更全面的检查，耗时更长
    
      <img src="image/start_build.png" alt="start_build" style="zoom:75%;" />
    
- **触发规则**：
    - 关联同一 issue 的多个 PR，仅需在任意一个 PR 里回复触发一次门禁，该 PR 门禁通过后，所有 PR 都会添加 Label 和测试人。
    - 每个 PR 只能同时运行一条 CI 流水线，如需重新启动，请先关闭运行中的，再评论触发门禁。
    - 创建 PR、更新代码、重新打开 PR，系统**不会**自动触发门禁，需要重新回复触发 CI 门禁。
    - Markdown 修改仅触发文档类构建测试门禁，不会触发 Cangjie 的编译测试门禁。
    
      <img src="image/sync_build.png" alt="sync_build" style="zoom:75%;" />
    
- **门禁检查内容**：
    - Commit 格式检查（需遵循 Conventional Commits 规范）
    - 静态告警分析（Codecheck）
    - Linux/Windows/Mac 平台的构建和 HLT、LLT 测试
    - 请保证每一条 commit 都已添加 Signed-Off-By 信息

6. **PR检视**

- **检视要求**：
    - 满足最低评审人数要求，2个评审人，1个审查人以及必要的 codeowners 成员，codeowners成员和审查人设置为合并计数：如果 codeowners 中有 commtter 成员，则该成员通过后无需额外的审查人。
    - 评审问题需全部解决，评审问题无特殊情况外需要评论作者自行确认后解决，请勿代他人解决。
    - Committer 检视时除业务逻辑外必须关注以下内容：
        - PR 内容是否符合要求
        - Issue 内容是否完整
        - Commit log 内容是否规范
        - Commit 拆分是否合理
        - 版权信息是否符合要求
        - 代码变更是否有必要的 UT、LLT 或其他测试覆盖，测试是否能够验证变更行为

以上内容不符合要求时，不应该给予通过。为了检视效率，代码检视时建议优先选择 codeowner 成员，参考仓库中 .gitcode 文件夹下 CODEOWNERS 文件，其次优先同模块和本领域 committer 进行检视。

7. **PR合入**

- **合入条件**：
    - 所有关联 PR 的门禁检查结果为 "成功"（build-test-passed）。
    - 满足最低评审人数要求，且评审问题需全部解决。
    - 禁止合入本人创建的 PR，需由其他协作者操作。

- **合入方式**：
    - 回复 "**start merge**"，CI 流水线会自动检查所有关联 PR 的状态。
    - 若所有 PR 都满足合并条件，则将会同时合并所有 PR。
    - 若存在不满足合并条件的 PR，则不会合并任何 PR，并回复不满足条件的 PR。

​	<img src="image/pr_success.png" alt="pr_success" style="zoom:75%;" />

<img src="image/build_job.png" alt="build_job"/>

## 测试用例贡献指南

为了使代码修改能够被持续验证，涉及功能、缺陷修复或行为变化时，贡献者应同步补充或更新有效的测试用例。根据修改所属仓库，测试用例分为编译器仓库的 UT（Unit Test）和测试仓库的 LLT（Low Level Test）。新增用例应覆盖本次修改的关键路径、边界条件和异常路径，避免只增加无法复现问题或只验证实现细节的用例。

不同代码仓库对应的测试补充位置如下：

- 修改 `cangjie_compiler` 仓库代码时，按照[“cangjie_compiler 仓库的 UT 用例”](#section_compiler_ut)一节的说明，在 `cangjie_compiler/unittests` 对应模块中增加 UT 用例；同时，涉及编译器端到端行为时，也应按照[“cangjie_test 仓库的 LLT 用例”](#section_llt)一节的说明，在 `cangjie_test/testsuites/LLT/compiler` 对应模块中增加 LLT 用例。
- 修改 `cangjie_tools`、`cangjie_runtime`、`llvm-project` 或 `cangjie-stdx` 仓库代码时，按照[“cangjie_test 仓库的 LLT 用例”](#section_llt)一节的说明，在 `cangjie_test/testsuites/LLT` 下与被测功能对应的 `Tools`、`Runtime`、`API` 或其他模块目录中增加端到端用例。
- 如果同一功能修改涉及多个仓库，应根据各仓库的职责分别补充对应测试，并为相关仓库分别创建 PR，使用同一个 Issue 关联这些 PR。测试用例所在仓库为 [cangjie_test](https://gitcode.com/Cangjie/cangjie_test)，测试执行框架为 [cangjie_test_framework](https://gitcode.com/Cangjie/cangjie_test_framework)。

### cangjie_compiler 仓库的 UT 用例<a name="section_compiler_ut"></a>

如果修改的是 [cangjie_compiler](https://gitcode.com/Cangjie/cangjie_compiler) 仓库代码，必要时应在同一个 PR 中增加或更新 UT 用例。UT 用例位于仓库根目录的 `unittests` 目录下，按被测模块放置，例如：

- `unittests/Parse`：语法解析相关用例；
- `unittests/Sema`：语义分析相关用例；
- `unittests/AST`、`unittests/CHIR`、`unittests/CodeGen`：对应的数据结构、CHIR 和代码生成相关用例；
- `unittests/Driver`、`unittests/Frontend`、`unittests/Modules`：驱动、前端和模块相关用例。

请根据修改代码的归属选择已有的模块目录；如果确实没有合适的目录，再与维护者确认后新增目录。编写用例时应优先复用该模块已有的测试辅助代码、断言和命名方式，并在相应目录的 `CMakeLists.txt` 中注册新增的测试源文件（如该目录的构建规则需要注册）。测试应独立、可重复，不依赖开发者本地的临时文件、网络服务或未声明的环境变量；涉及错误诊断时，同时验证错误类型和关键诊断信息。

编译器 UT 使用 GoogleTest（GTest）。新增 C++ 测试通常使用 `TEST`/`TEST_F` 等宏编写，并在对应模块的 `CMakeLists.txt` 中创建测试目标，链接 `GTest::gtest` 和 `GTest::gtest_main`，再通过 `add_test` 注册到 CTest。可参考 [GoogleTest Primer](https://google.github.io/googletest/primer.html) 了解测试、断言和测试夹具的基本用法；仓库中已有模块的 `CMakeLists.txt` 可作为注册方式示例。

在 Linux 环境下，可参考以下方式构建并执行 UT（具体编译参数和平台要求以仓库 README 及构建脚本为准）：

```shell
cd cangjie_compiler
python3 build.py build
python3 build.py test
```

`unittests` 在正常构建时默认参与构建，`python3 build.py test` 会执行已构建的单元测试。提交前应确认新增用例已被构建系统发现，并保留本地构建和测试结果；需要了解其他构建选项时，可执行 `python3 build.py --help`。

### cangjie_test 仓库的 LLT 用例<a name="section_llt"></a>

LLT 总体使用 [cangjie_test_framework](https://gitcode.com/Cangjie/cangjie_test_framework) 运行，测试用例维护在 [cangjie_test/testsuites/LLT](https://gitcode.com/Cangjie/cangjie_test/tree/main/testsuites/LLT)。LLT 是按模块组织的端到端测试，新增用例应放入与被测功能对应的目录，而不是随意放在公共目录中。当前主要目录映射如下：

- `testsuites/LLT/compiler`：编译器功能，例如 `Parser`、`Lexer`、`Sema`、`Frontend`、`CHIR`、`CodegenCJNative`、`Driver`、`Macro`、`Modules`、`IncrementalCompilation` 等；
- `testsuites/LLT/Runtime`：运行时功能；
- `testsuites/LLT/API`：标准库、扩展库及 API 相关功能；
- `testsuites/LLT/Tools`：`cjpm`、`cjfmt`、`cjlint`、`cjdb`、`cjprof`、`cjcov` 等工具功能。

例如，编译器 Parser 的用例应放在 `testsuites/LLT/compiler/Parser` 下，并可继续按语法主题建立子目录；工具链用例应放在 `testsuites/LLT/Tools` 下对应工具目录。提交前请检查对应模块是否已有相近用例，优先在原目录补充，避免重复覆盖相同场景。

#### LLT 用例编写要求

1. 先明确用例目的和预期结果：一个用例重点验证一个行为或一组紧密相关的行为，名称和目录应能反映测试场景。
2. 复用同模块已有用例的格式。通常在 `.cj` 文件头部声明版权信息、`LEVEL` 和 `EXEC`，并使用 `SCAN` 或比较文件等机制描述预期输出；正向用例验证程序结果，负向用例验证错误类别、位置及关键诊断信息。
3. 端到端用例应覆盖真实用户路径（例如源文件编译、运行或工具命令执行），同时保持输入、依赖和输出稳定。不要把偶然的绝对路径、时间戳、机器相关信息或未稳定排序的完整输出写入期望结果；必要时使用框架提供的比较方式过滤非确定性内容。
4. 对缺陷修复至少增加一个能够在修复前失败、修复后通过的回归用例；对跨平台功能，应根据适用平台增加条件或选择对应配置，不能把平台专属行为写成所有平台都必须通过的结果。
5. 如果新增用例需要额外配置、测试数据或环境变量，应同步更新对应模块的配置/说明，并在 PR 中说明依赖和验证命令。不要通过永久屏蔽或放宽断言来隐藏失败。

#### LLT 用例运行

运行框架前请按照 [cangjie_compiler 独立构建指导](https://gitcode.com/Cangjie/cangjie_compiler/blob/dev/doc/Standalone_Build_Guide.md) 或对应平台的构建文档准备仓颉工具链及测试依赖，并确保 LLVM、JDK、OpenSSL 3、Python 3 的 `pexpect` 和 `fasteners` 等平台所需工具可用。Linux x86_64 下可参考以下命令运行单个 LLT 用例（将路径替换为实际用例）：

```shell
cd <workspace>
python3 cangjie_test_framework/main.py \
  --test_cfg=cangjie_test/testsuites/LLT/configs/cjnative/cjnative_test.cfg \
  --verbose \
  cangjie_test/testsuites/LLT/compiler/Parser/function/return.cj
```

运行 LLT 测试套中的全部用例，可使用测试列表进行筛选并设置并发数和超时时间：

```shell
python3 cangjie_test_framework/main.py \
  --test_cfg=cangjie_test/testsuites/LLT/configs/cjnative/cjnative_test.cfg \
  --test_list=cangjie_test/testsuites/LLT/cjnative_testlist \
  -pFAIL -j20 --timeout=180 \
  cangjie_test/testsuites/LLT/
```

也可以将 `cangjie_test/testsuites/LLT/configs/cjnative/cjnative_test.cfg` 复制为 `testsuites/LLT/test.cfg`，确认配置中的 `[root] path` 指向测试仓库根目录后，按框架 README 的方式运行已配置的测试套。不同操作系统或架构应选择对应的配置文件和测试列表；提交前至少执行新增用例，并根据改动范围执行对应模块或完整 LLT 测试。

#### 提交前检查

- 用例已放在正确的 UT/LLT 模块目录，并已加入必要的构建规则或测试列表；
- 用例在本地实际执行通过，失败用例没有被静默跳过、永久屏蔽或修改为无效断言；
- 代码、UT 和 LLT 的行为预期一致，测试结果具有稳定性和可重复性；
- PR 描述中列出新增/更新的用例、执行的命令、测试环境及结果；
- 若代码和测试分属多个仓库，使用同一个 Issue 关联各仓库 PR，并按照本文件前述多仓门禁流程触发联合构建和测试。

## 版本变化说明<a name="section_version_changelog"></a>

### 版本历史

本文档记录了仓颉社区贡献流程的版本更新历史，便于贡献者了解流程的变化。

---

#### 2026-06-22

**变更内容**：
- 新增 AI 辅助编码贡献规范：明确使用 AI 工具辅助编写代码时须在 commit 末尾标注 `Assisted-by` 标签，并强调人类开发者对 AI 生成代码的审查责任

---

#### 2025-12-29

**变更内容**：
- 明确 Issue 创建规则：补充说明不要重复创建多个相同 Issue，多个目标分支的 PR 可以同时使用一个 Issue 触发门禁
- 新增版本变化说明章节，用于记录文档和流程的重要变更历史

---

#### 2025-12-24

**变更内容**：
- 新增 sync 标签使用规则：明确从其他分支 cherry-pick 的同步改动需要关联 sync 标签
- 优化 PR Label 关联说明的结构和表述

---

#### 2025-12-23

**变更内容**：
- 完善 Issue 创建时的 Label 关联规则说明，明确缺陷类和需求类 Issue 的版本号 Label 关联要求
- 优化 PR 创建重要提示，要求变更内容描述信息充分详细，并提供必要的编译和自验证结果
- 简化门禁触发规则描述，移除冗余的门禁类型判定说明
- 优化 PR 关联规则表述，明确同一仓库内同一目标合入分支的限制

---

**注意**：版本变化说明将在此处持续更新，记录每次重要的流程变更和文档更新。
