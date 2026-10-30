# Cangjie 社区 Pull Request 评论支持命令行清单

本文列出 Cangjie 社区 Pull Request 支持的评论命令及常用标签，适用于 Cangjie 组织下接入 CI 的代码仓。命令需在 PR 会话区评论，联合提交只需在任意一个关联 PR 评论一次。

## 1. 评论命令

| 评论命令 | 是否必选 | 使用场景 | 触发角色 |
| --- | --- | --- | --- |
| `start build` | **必选** | 触发构建与测试检查：commitlint、Codecheck、OAT、PR/Issue 合规、Linux/Windows/macOS 构建与 UT/HLT/LLT，以及文档和多语言互操作检查 | PR 创建人 |
| `start merge` | **必选（合入）** | 检查并合入同一 Issue 关联的全部 PR；任一 PR 不满足条件则全部不合入 | PR 创建人 |
| `start build cov` | 条件必选 | 关联 `[feature]:` 需求类 Issue 时必选，用于检查增量代码覆盖率；非需求类 PR 可不执行 | PR 创建人 |
| `pr-issue-review` | 可选 | 复核 PR/Issue 模板遵从度及关联一致性 | PR 创建人 |

**使用说明**

- 命令需单独评论在 PR 会话区，不要发在 Issue 或代码行内评论。
- 同一 PR 同时只允许一条 CI 任务运行；需要重跑时，等待当前任务结束后重新评论。
- 代码推送后需重新执行 `start build`；需求类 PR 同时需重新执行 `start build cov`。
- `start build` 通过后，重复评论会被跳过；需要重新验证时，先推送新提交。

## 2. 标签说明

| 标签 | 含义 | 触发方式 |
| --- | --- | --- |
| `waiting-start-build` | 等待触发 CI，或 CI 失败待修改 | PR 创建、代码变更、CI 失败 |
| `CI-running` | CI 运行中 | 命令触发 CI |
| `build-test-passed` / `build-test-failed` | 构建测试通过/失败 | `start build` |
| `codecheck-passed` / `codecheck-failed` | 静态检查通过/失败 | `start build` |
| `commitlint-passed` / `commitlint-failed` | commit 规范通过/失败 | `start build` |
| `sign-off-passed` / `sign-off-failed` | Signed-off-by 检查通过/失败 | `start build` |
| `OAT-passed` / `OAT-failed` | 开源声明检查通过/失败 | `start build` |
| `cov-test-passed` / `cov-test-failed` | 增量覆盖率检查通过 | `start build cov` |
| 语义化版本标签（如 `1.2.0-alpha.12`） | 目标分支对应的版本 | PR 创建时按目标分支自动添加 |
