会议：TPC Team-例会-2026-09-21

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

| 序号 | 议题名称                | 议题内容                                   | 汇报人 |
| ---- | ----------------------- | ------------------------------------------ | ------ |
| 1    | TPC项目创建申请规则修改 | 修改 TPC 项目创建申请规则                   | 方维   |
| 2    | 历史申请项目进展        | 通报历史申请项目的建仓与代码提交进展        | 方维   |
| 3    | Cangjie-TPC组织建仓评审 | 评审 Cangjie-TPC 组织新库创建申请            | 赵丹荣 |

## 会议纪要(Minutes of Meeting)

**议题1、TPC项目创建申请规则修改**

汇报人：方维/fangwei51@h-partners.com

会议结论：

1、源代码从必传改为非必传；

2、申请信息必须包含开源 license，增加 License 信息；

3、源码可以参考 templete 模板。

**议题2、历史申请项目进展**

汇报人：方维/fangwei51@h-partners.com

会议结论：

1、bgfx4cj、xretry、xlsx4cj、amqp、cgit、zookeeper_client、config_io、markit、cjqt6、doclint、esclient、exec4cj、cangjie-mcp-tools、cangjie-deveco-code-plugin 共14个库已完成创建和代码提交。

2、剩余30个库已完成建仓，等待第一次提交代码。

3、xos、codec、codec_json、codec_macro、codec_msgpack、fecha4cj 共7个库待优化。

4、8个库不通过。

遗留问题：

1、跟进剩余30个库提交第一版代码。责任人：赵丹荣、闭环时间：2026-09-28

**议题3、Cangjie-TPC组织建仓评审**

汇报人：赵丹荣/Leporide

会议结论：

1、本周共收到 TinyColor、dd-plist、xslt_processor_cj、@nutpi/calendar-tool、url_parse、three.cj 共6个库申请，评审结论如下：

| 申请时间 | 仓库名 | 作者 | 工作单位 | 仓库链接 | 仓库简介 | License | 评审时间 | 申请结论 | 备注 |
| -------- | ------ | ---- | -------- | -------- | -------- | ------- | -------- | -------- | ---- |
| 2026/9/14 | TinyColor | 王舒凡 | 南京大学 | https://github.com/bgrins/TinyColor | TinyColor 是面向仓颉语言的颜色操作与转换库，支持 Hex、RGB/RGBA、HSL/HSLA 等多种输入格式。 | MIT License | 2026/9/21 | 比赛 |  |
| 2026/9/14 | dd-plist | 黄博远 | 南京大学 | https://github.com/3breadt/dd-plist | dd-plist 是纯仓颉实现的 Apple property list 解析与生成库，覆盖 XML、Binary、ASCII 三种格式。 | Daniel Dreibrodt | 2026/9/21 | 比赛 | 添加license 名称，当前license和MIT License一样 |
| 2026/9/14 | xslt_processor_cj | 汪翰元 | 南京大学 | https://github.com/DesignLiquido/xslt-processor | xslt_processor_cj 是基于仓颉标准库实现的 XML、XPath 与 XSLT 处理库。 | GNU 3 | 2026/9/21 | 比赛 | 已有开发者申请建仓通过序号26 |
| 2026/9/14 | @nutpi/calendar-tool | 吉天祎 | 南京大学 | https://gitcode.com/Elmejorjugador/cangjie_base_calendar-tool | @nutpi/calendar-tool 是历法转换工具，实现公历、农历、儒略历与格里历之间的精确换算。 |  | 2026/9/21 | 比赛 | 空仓库 |
| 2026/9/14 | url_parse | 施佳凡 | 南京大学 | https://github.com/unshiftio/url-parse | url_parse 是轻量级 URL 解析与结构化处理工具库，对标 JavaScript url_parse。 | MIT License | 2026/9/21 | 比赛 | 已有开发者申请建仓通过序号21 |
| 2026/9/14 | three.cj | 饶子俊 | 二十四维（杭州）互联网有限责任公司 | https://github.com/YQ-RZJ/three.cj | three.cj 是使用仓颉语言实现的 3D 引擎运行时，提供三维渲染、音频、物理、脚本等能力。 | Apache License 2.0 | 2026/9/21 | 计划建仓 |  |

2、除 three.cj 计划建仓通过以外，其余 5 个库（TinyColor、dd-plist、xslt_processor_cj、@nutpi/calendar-tool、url_parse）在比赛和共建活动阶段，待活动结束后重新评估，由赵丹荣和开发者沟通。

遗留问题：

1、跟进 TinyColor、dd-plist、xslt_processor_cj、@nutpi/calendar-tool、url_parse 5 个库，待比赛和共建活动结束后重新评估。责任人：赵丹荣、闭环时间：待活动结束