会议：TPC Team-例会-2026-09-14

## 参会人员 (Attendance)

| 姓名   | 账号                              |
| ------ | --------------------------------- |
| 方维   | [wayne29](https://gitcode.com/wayne29) |
| 夏松   | [xdst](https://gitcode.com/xdst) |
| 任义   | [renyi43](https://gitcode.com/renyi43) |
| 虞嘉豪 | [ChaosJohn](https://gitcode.com/ChaosJohn) |
| 王焱济 | [cangjie-wangyanji](https://gitcode.com/cangjie-wangyanji) |
| 赵丹荣 | [Leporide](https://gitcode.com/Leporide) |

## 议题(Agenda)

| 序号 | 议题名称               | 议题内容                                  | 汇报人 |
| ---- | ---------------------- | ----------------------------------------- | ------ |
| 1    | 历史申请项目进展       | 跟进历史申请项目的评审进展与建仓情况      | 赵丹荣 |
| 2    | Cangjie-TPC组织建仓评审 | 评审 Cangjie-TPC 组织新库创建申请        | 方维 |
| 3    | 已创建仓库更名评审     | 评审已创建仓库的更名申请                  | 赵丹荣 |

## 会议纪要(Minutes of Meeting)

**议题1、历史申请项目进展**

汇报人：赵丹荣/Leporide

会议结论：

1、本周历史申请项目评审进展如下：历史申请项目中有以下 11 个库已完成建仓（2026-09-13）：

| 仓库名 | 作者 | 仓库链接 | License | 建仓日期 |
| ------ | ---- | -------- | ------- | -------- |
| quality-plugin | 孟飞 | https://gitcode.com/Cangjie-TPC/quality-plugin | Apache License 2.0 | 2026-09-13 |
| buffer4cj | 李佩 | https://gitcode.com/Cangjie-TPC/buffer4cj | MIT License | 2026-09-13 |
| avro4cj | 陈文龙 | https://gitcode.com/Cangjie-TPC/avro4cj | Apache License 2.0 | 2026-09-13 |
| throttledebounce4cj | 李佩 | https://gitcode.com/Cangjie-TPC/throttledebounce4cj | Apache License 2.0 | 2026-09-13 |
| sanitizeHtml4cj | 蔡钊 | https://gitcode.com/Cangjie-TPC/sanitizeHtml4cj | MIT License | 2026-09-13 |
| image_edit_cj | 陈文龙 | https://gitcode.com/Cangjie-TPC/image_edit_cj | Apache License 2.0 | 2026-09-13 |
| image_cropper_cj | 赵家辉 | https://gitcode.com/org/Cangjie-TPC/image_cropper_cj | Apache License 2.0 | 2026-09-13 |
| jmespath4cj | 刘婷 | https://gitcode.com/Cangjie-TPC/jmespath4cj | Apache License 2.0 | 2026-09-13 |
| validator4cj | 张宇飞 | https://gitcode.com/Cangjie-TPC/validator4cj | Apache License 2.0 | 2026-09-13 |
| box2d4cj | 李艳情 | https://gitcode.com/Cangjie-TPC/box2d4cj | Apache License 2.0 | 2026-09-13 |
| epub4cj | 孟飞 | https://gitcode.com/Cangjie-TPC/epub4cj | Apache License 2.0 | 2026-09-13 |

遗留问题：

1、本周完成第一次代码提交，责任人：各仓库负责人；闭环时间：2026/9/18

**议题2、Cangjie-TPC组织建仓评审**

汇报人：赵丹荣/Leporide

会议结论：
1、本周申请项目评审进展如下：

| 仓库名 | 作者 | 单位 | 仓库链接 | 简介 | License | 评审结论 | 备注 |
| ------ | ---- | ---- | -------- | ---- | ------- | -------- | ---- |
| esclient | 高阳 | 普元信息股份有限公司 |  | Elasticsearch 的仓颉客户端实现, 由普元信息技术股份有限公司开发实现并提供支持, 参考Java实现 co.elastic.clients:elasticsearch-java:8.14.1 | Apache License 2.0 | 计划建仓 |  |
| exec4cj | 罗昌灏 | 湖南大学 |  | Commons-Exec 参考 Apache Commons Exec，是一个基于仓颉语言实现的外部进程执行与管理库。<br/>该库提供了灵活、安全、跨平台的进程执行接口，能够方便地在应用程序中启动和控制系统命令或外部程序，封装了底层进程管理逻辑，提供更高级别的 API，使开发者能够更方便地进行命令执行、流重定向、超时监控及异步控制。 |  | 计划建仓 | 当前cjc编译版本0.45.2，后续需要社区更新到最新1.1.3版本 |
| fastjson2-cangjie | 李伟彬 |  | https://gitee.com/fuquxiaoguang/fastjson2-cangjie | fastjson2-cangjie 是阿里巴巴高性能 JSON 库 fastjson2 的仓颉（Cangjie）语言移植版 | LGPL-3.0 | 待优化 | 1.缺少README.OpenSource文本文件；2.cjpm中organization = "alibaba"，alibaba不合适；3.上游 https://github1s.com/alibaba/fastjson2/ 的 license 是 Apache License 2.0，移植后使用 LGPL-3.0 需澄清，该协议会污染源码；4.参考模板 https://gitcode.com/Cangjie-TPC/TPC-Resource/tree/main/template 修改代码路径，增加test文件夹 |
| Cliver4cj | 郭天悦 | 编程语言实验室-布尔研究所 | https://github.com/BinaRoy/CJCliver | Cliver（Cangjie Package CLI Driver Generator）是一个面向仓颉语言的软件包 CLI 驱动生成工具。它能够解析目标仓颉包公开 API，并自动生成可执行的 CLI Driver，使原本需要通过仓颉代码集成和调用的 Package API，被直接通过命令行调用。 | Apache License 2.0 | 计划建仓 |  |
| parser-html-json | 黄博远 | 南京大学 | https://github.com/1623311678/html-parser-server | parser-html-json 是纯仓颉实现的 HTML 解析库，对外提供两个顶层函数：getHtmlJson 将 HTML 字符串解析为 JSON 树字符串，getClassStyleJson 从 style 标签中提取 CSS 类样式并返回「类名—样式声明」映射。 | MIT License | 待优化 | 1.参考模板 https://gitcode.com/Cangjie-TPC/TPC-Resource/tree/main/template 修改代码路径，增加test文件夹；2.Licence 需修改为标准MIT，不需要体现上游仓库 |
| cangjie-mcp-tools | 李磊 | 华为 | https://gitcode.com/lilei-ide/tools/tree/main/mcp/cangjie_lsp_mcp | 构建仓颉专属插件，将LSP等底层能力转化为MCP工具集，并打通DevEco Code/OpenCode与仓颉鸿蒙应用开发的端到端链路，实现从自然语言到仓颉应用生成的自动化闭环。 | MIT License | 计划建仓 | 源码仓缺少License |
| cangjie-deveco-code-plugin | 李磊 | 华为 | https://gitcode.com/lilei-ide/tools/tree/main/plugins/deveco_code_cangjie/cangjie-plugin | 构建仓颉专属插件，将LSP等底层能力转化为MCP工具集，并打通DevEco Code/OpenCode与仓颉鸿蒙应用开发的端到端链路，实现从自然语言到仓颉应用生成的自动化闭环。 | MIT License | 计划建仓 | 源码仓缺少License |

遗留问题：

1、fastjson2-cangjie 按备注完成优化（补齐 README.OpenSource、修正 cjpm organization、澄清 License、按模板调整代码路径并增加 test 文件夹）。责任人：李伟彬、闭环时间：待定

2、parser-html-json 按模板调整代码路径并增加 test 文件夹，License 修改为标准 MIT。责任人：黄博远、闭环时间：待定

3、cangjie-mcp-tools、cangjie-deveco-code-plugin 源码仓补充 License 后建仓。责任人：李磊、闭环时间：待定

**议题3、已创建仓库更名评审**

汇报人：方维/fangwei51@h-partners.com

会议结论：

1、已创建仓库更名评审结果如下：

| 序号 | 申请时间 | 原仓库名      | 仓库地址                                      | 新仓库名称 | 新仓库地址                                   | 评审时间 | 申请结论 | 备注         |
| ---- | -------- | ------------- | --------------------------------------------- | ---------- | -------------------------------------------- | -------- | -------- | ------------ |
| 1    | 2026-09-11 | cjc-hotfix-plugin | https://gitcode.com/Cangjie-TPC/cjc-hotfix-plugin | hotfix_tools | https://gitcode.com/Cangjie-TPC/hotfix_tools | 2026-09-14 | 通过 | 缺少License |
| 2 | 2026-09-11 | sqlite_cj |  | sqlite-ffi |  | 2026-09-14 | 通过 |  |

遗留问题：

1、hotfix_tools 需补充 License。责任人：赵丹荣；待确认、闭环时间：待定