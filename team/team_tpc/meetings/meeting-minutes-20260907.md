会议：TPC Team-例会-2026-09-07

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

| 序号 | 议题名称                | 议题内容                              | 汇报人 |
| ---- | ----------------------- | ------------------------------------- | ------ |
| 1    | Cangjie-TPC组织建仓评审 | 评审 Cangjie-TPC 组织新库创建申请      | 赵丹荣 |
| 2    | 已创建仓库审核          | 审核已申请仓库的建仓情况              | 方维   |

## 会议纪要(Minutes of Meeting)

**议题1、Cangjie-TPC组织建仓评审**

汇报人：赵丹荣/Leporide

会议结论：

1、以下 14 个库计划建仓（2026-09-07），各库备注要求如下：

| 仓库名 | 作者 | 仓库链接 | 简介 | License | 备注 |
| ------ | ---- | -------- | ---- | ------- | ---- |
| quality-plugin | 孟飞 | https://gitcode.com/koolib/quality-plugin | quality-plugin 是一款专为 DevEco Studio 和 IntelliJ IDEA 设计的插件，用于扫描和评估仓颉项目的代码质量。 | Apache License 2.0 | 适配6.1.1和7.0版本插件；package 不使用huawei |
| buffer4cj | 李佩 | https://gitcode.com/koolib/buffer4cj | buffer4cj 是一个使用仓颉语言实现的二进制数据缓冲区库，支持多种编码的读写、搜索、比较等操作，提供与 Node.js Buffer 兼容的 API 设计。 | MIT License | 添加Test文件夹 |
| avro4cj | 陈文龙 | https://gitcode.com/koolib/avro4cj | avro4cj 是 Apache Avro 数据序列化系统的仓颉语言实现，使仓颉应用能够与 Hadoop/Kafka 等主流大数据基础设施原生集成。 | Apache License 2.0 | 添加DT用例；文档check |
| throttledebounce4cj | 李佩 | https://gitcode.com/koolib/throttledebounce4cj | throttledebounce4cj 是一个节流和防抖的函数库。 | Apache License 2.0 | 添加Test文件夹 |
| sanitizeHtml4cj | 蔡钊 | https://gitcode.com/koolib/sanitizeHtml4cj | sanitizeHtml4cj 是基于仓颉语言开发的 HTML 清理工具库，通过白名单机制移除危险的 HTML 标签和属性，有效防止 XSS 攻击。 | MIT License | 计划建仓 |
| image_edit_cj | 陈文龙 | https://gitcode.com/koolib/image_edit_cj | image_edit_cj 是仓颉语言图片编辑库，提供图片裁剪、旋转、缩放、翻转等几何变换和色彩调整能力。 | Apache License 2.0 | 增加6.1.1_compli分支；增加DT用例 |
| image_cropper_cj | 赵家辉 | https://gitcode.com/koolib/image_cropper_cj | image_cropper_cj 是基于仓颉语言开发的 HarmonyOS 图片裁剪组件，支持自由及固定宽高比裁剪、捏合缩放、拖动定位、旋转、镜像等。 | Apache License 2.0 | 添加DT用例 |
| jmespath4cj | 刘婷 | https://gitcode.com/koolib/jmespath4cj | JMESPath4cj 是一个用于 Cangjie 语言的 JMESPath 表达式解析库，提供完整的 JMESPath 实现。 | Apache License 2.0 | 删除其他分支 |
| validator4cj | 张宇飞 | https://gitcode.com/koolib/validator4cj | validator4cj 提供了数据验证功能。 | Apache License 2.0 | 升级到1.1.3；只上传develop分支 |
| box2d4cj | 李艳情 | https://gitcode.com/koolib/box2d4cj | box2d4cj 是一个用仓颉语言实现的 2D 刚体物理引擎，是对著名 Box2D 物理引擎的高质量移植。 | Apache License 2.0 | 增加中文文档；ReadMe中文；仓库模板修改 |
| epub4cj | 孟飞 | https://gitcode.com/koolib/epub4cj | epub4cj 是一个用仓颉语言编写的 EPUB 电子书格式解析库，支持 EPUB 2 和 EPUB 3 标准。 | Apache License 2.0 | 增加中文文档；ReadMe中文；仓库模板修改 |
| mail4cj | 李佩 | https://gitcode.com/koolib/mail4cj | mail4cj 是一个用于在仓颉应用程序中发送、接收和处理电子邮件的库。 | Apache License 2.0 | 增加中文文档；ReadMe中文；仓库模板修改 |
| quality-tool | 李艳情 | https://gitcode.com/koolib/qualitytool | quality-tool 是一个仓颉项目质量评分工具，对仓颉项目进行多维度的质量扫描和评分，生成 Markdown 格式的质量报告。 | Apache License 2.0 | ReadME修改兼容版本；增加文档 |
| lz4cj | 李佩 | https://gitcode.com/koolib/lz4cj | lz4cj 是一个使用仓颉语言实现的 LZ4 压缩/解压缩库。 | Apache License 2.0 | 添加Test文件夹 |

遗留问题：

1、跟进各仓库按备注要求完成整改后建仓。责任人：赵丹荣、闭环时间：2026-09-14

**议题2、已创建仓库审核**

汇报人：方维/fangwei51@h-partners.com

会议结论：

1、bgfx4cj、xretry、codec、codec_json、codec_macro、codec_msgpack、fecha4cj、log4cj-OH、color-picker-cj、jsoup4cj、jfreechart4cj、gcoord4cj、sqlite_cj、xlsx4cj、Silo-Project、juuid、amqp、xslt_processor_cj、Cangjie-SunCalc、CangjieEmbeddedHAL、cgit、zookeeper_client、config_io、crc-cj、cryptoprimitives4cj、hud4cj、markit、cjqt6 已完成沟通。

2、bgfx4cj、xretry、log4cj-OH、jsoup4cj、amqp、cgit、zookeeper_client、config_io、markit、cjqt6 已完成项目创建流程。

3、color-picker-cj、jfreechart4cj、gcoord4cj、xlsx4cj、Silo-Project、xslt_processor_cj、hud4cj 已创建仓库但尚未提交代码，需跟进开发者尽快提交第一版代码。

遗留问题：

1、跟进已创建仓库但未提交代码的仓库（color-picker-cj、jfreechart4cj、gcoord4cj、xlsx4cj、Silo-Project、xslt_processor_cj、hud4cj），督促开发者尽快提交第一版代码。责任人：赵丹荣、闭环时间：2026-09-14