会议：TPC Team-例会-2026-08-31

## 参会人员 (Attendance)

| 姓名   | 账号                              |
| ------ | --------------------------------- |
| 夏松   | [xdst](https://gitcode.com/xdst) |
| 王焱济 | [cangjie-wangyanji](https://gitcode.com/cangjie-wangyanji) |
| 方维   | [wayne29](https://gitcode.com/wayne29) |
| 赵丹荣 | [Leporide](https://gitcode.com/Leporide) |
| 虞嘉豪 | [ChaosJohn](https://gitcode.com/ChaosJohn) |
| 任义   | [renyi43](https://gitcode.com/renyi43)  |

## 议题(Agenda)

| 序号 | 议题名称                     | 议题内容                                 | 汇报人 |
| ---- | ---------------------------- | ---------------------------------------- | ------ |
| 1    | Cangjie-TPC组织建仓评审      | 评审 Cangjie-TPC 组织新库创建申请         | 赵丹荣 |
| 2    | 已创建仓库审核               | 审核已申请仓库的建仓情况                 | 方维   |

## 会议纪要(Minutes of Meeting)

**议题1、Cangjie-TPC组织建仓评审**

汇报人：方维/fangwei51@h-partners.com

会议结论：
1、doclint（工具仓）建仓申请计划建仓，需完成以下事项后建仓：
   - 补充 license；
   - 仓库网址 https://gitcode.com/cjse/doclint 打不开（尚未公开），需公开后复核；
   - 删除 .trae 文件夹；
   - 待确认是否需走开源流程。

遗留问题：
1、doclint 补充 license、删除 .trae 文件夹、公开仓库并确认开源流程后建仓。责任人：赵丹荣、闭环时间：2026-09-07

**议题2、已创建仓库审核**

汇报人：方维/fangwei51@h-partners.com

| 仓库名        | 作者        | 仓库链接                                                     | 简介                                                         | 仓颉linces | 决策     | 备注                                                         |
| ------------- | ----------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ---------- | -------- | ------------------------------------------------------------ |
| codec         | 陈皓珲      | https://gitcode.com/m0_74475107/codec                        | codec  是仓颉编程语言的序列化/反序列化核心库，提供格式无关的序列化抽象。 | Apache-2.0 | 计划建仓 | 和开发者沟通 codec、codec_json、codec_macro、codec_msgpack 4 个仓库需先沟通确认是否可合并建仓 |
| codec_json    | 陈皓珲      | https://gitcode.com/m0_74475107/codec_json                   | codec_json 是基于 codec  框架的 JSON 格式实现库，为仓颉生态提供高性能、功能完整的 JSON 序列化能力。 | Apache-2.0 | 计划建仓 | 和开发者沟通 codec、codec_json、codec_macro、codec_msgpack 4 个仓库需先沟通确认是否可合并建仓 |
| codec_macro   | 陈皓珲      | https://gitcode.com/m0_74475107/codec_macro                  | codec_macro 是 codec  序列化框架的编译时代码生成组件，通过 @Codec 和 @Field 宏自动为数据结构生成高效的序列化/反序列化代码，实现零成本抽象。 | Apache-2.0 | 计划建仓 | 和开发者沟通 codec、codec_json、codec_macro、codec_msgpack 4 个仓库需先沟通确认是否可合并建仓 |
| codec_msgpack | 陈皓珲      | https://gitcode.com/m0_74475107/codec_msgpack                | codec_msgpack 是 Codec  序列化框架的 MessagePack 格式实现，与 codec（核心抽象层）和  codec_macro（代码生成宏）紧密集成，为仓颉语言提供高性能的二进制序列化能力。 | Apache-2.0 | 计划建仓 | 和开发者沟通 codec、codec_json、codec_macro、codec_msgpack 4 个仓库需先沟通确认是否可合并建仓 |
| fecha4cj      | 田玟玟      | https://gitcode.com/MakerStudio/fecha4cj.git                 | Fecha-cj是Fecha日期库的仓颉语言移植版本，是一个轻量级日期格式化和解析库。 | MIT        | 待优化   | 库的想法不错，建议增加cangjie通用版本分支                    |
| sqlite_cj     | 高亲豹      | https://gitcode.com/gqb6666/sqlite_cj                        | sqlite_cj 是一个为仓颉语言提供的  SQLite3 数据库封装库。     | MIT        | 待优化   | 开发者反馈 建议优化库名  增加ffi，体现封装                   |
| titlebar      | 周可心      | https://gitee.com/smarthane/titlebar                         | titlebar  旨在提供统一、易用、可扩展的页面顶部标题栏能力。   | Apache-2.0 | 不通过   | 需发邮件通知开发者，待整改完成后重新申请                     |
| url-parse     | 周可心      | https://gitcode.com/CPF-ApplicationTPC/openharmony_tpc_samples/tree/master/url_parse | url-parse提供将URL字符串解析为解析为机构化对象的能力，并支持相对路径解析、查询参数以及百分号编码/解码 | Apache-2.0 | 计划建仓 |                                                              |
| mdurl         | 周可心      | https://gitcode.com/openharmony-tpc/openharmony_tpc_samples/tree/master/mdurl | mdurl 是一个基于仓颉 1.1.0  编写的轻量级 URL 解析与百分号编解码工具库，完全手工实现，不依赖任何正则表达式或第三方库。 | Apache-2.0 | 计划建仓 |                                                              |
| juuid         | hw076035933 | https://gitcode.com/gcw_z3acR2wn/Cangjie-KU                  | 仓颉语言 UUID 生成库，支持  v1/v3/v4/v5/v7 五种版本，严格符合 RFC 4122/RFC 9562 标准。 | Apache-2.0 | 计划建仓 | 改名为 uuid_lite，和TPC/uuid4cj库区别                        |
| cjvalidator   | hw076035933 | https://gitcode.com/gcw_z3acR2wn/Cangjie-KU                  | 仓颉语言数据验证库，提供 193+  内置验证规则，覆盖 8 大类别，支持链式构建器、跨字段校验、自定义规则扩展和多语言错误消息。 | Apache-2.0 | 计划建仓 | 和开发者沟通 cjvalidator 改名后                              |

会议结论：

1、和开发者沟通 codec、codec_json、codec_macro、codec_msgpack 4 个仓库需先沟通确认是否可合并建仓。责任人：赵丹荣、闭环时间：2026-09-07

2、url_parse、mdurl 两个仓库都保留，计划建仓；责任人：赵丹荣、闭环时间：2026-09-07

3、和开发者沟通，cjuuid 改名为 uuid_lite  计划建仓，和开发者沟通 cjvalidator 改名、与 validator4cj 区分后  计划建仓；责任人：赵丹荣、闭环时间：2026-09-07

4、titlebar 非鸿蒙工程、无 demo 效果，不通过，需发邮件通知开发者，待整改完成后重新申请；责任人：赵丹荣、闭环时间：2026-09-07

5、titlebar-cj 计划建仓；责任人：赵丹荣、闭环时间：2026-09-07

6、已创建仓库，和开发者沟通，尽快提交第一版代码， 责任人：赵丹荣、闭环时间：2026-09-07