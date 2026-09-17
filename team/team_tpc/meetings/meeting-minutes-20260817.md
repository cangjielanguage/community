会议：TPC Team-例会-2026-08-17

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
| 1    | Cangjie-TPC组织建仓评审      | 评审 Cangjie-TPC 组织新库创建申请         | 方维   |
| 2    | Cangjie-SIG组织建仓模板评审  | 评审 Cangjie-SIG 组织建仓模板             | 赵丹荣 |
| 3    | Cangjie-TPC组织分支管理评审  | 评审 Cangjie-TPC 组织仓库分支管理要求     | 方维   |

## 会议纪要(Minutes of Meeting)

**议题1、Cangjie-TPC组织建仓评审**

汇报人：方维/fangwei51@h-partners.com

会议结论：
1、对本次 10 个建仓申请逐库评审，其中 3 个申请通过、1 个升级到 1.1.3 后通过、若干需补充资料/待下周重新评审，详见下表：

| 仓库名称            | 作者   | 简介                                                         | 决策                                                         |
| ------------------- | ------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Cangjie-SunCalc     | 符继东 | 基于仓颉语言的太阳与月亮位置计算库，算法移植自 mourner/suncalc | 待提交源码后，下周重新评审：1、压缩包内无源码；2、版本升级，53.4 版本太老，升级到 1.1.3 |
| fraction_js         | 付一   | 面向仓颉的有理数运算工具库，对标 JS 生态 Fraction.js         | 待提交源码后，下周重新评审：1、压缩包内无源码；2、版本升级到 1.1.3 |
| CangjieEmbeddedHAL  | 符继东 | 仓颉嵌入式硬件抽象层（HAL），统一 GPIO/UART/SPI/I2C/PWM/ADC 等外设接口 | 压缩包内无源码，需补充提交源码                               |
| cgit                | 高阳   | 基于仓颉的 Git 实现库，对标 JGit-6.8.0-m2                   | 申请通过；1、说明 zlib4cj 来源；2、建议升级到 1.1.3          |
| zookeeper_client    | 高阳   | ZooKeeper Cangjie SDK，支持节点操作、ACL、Watcher 等         | 申请通过；1、缺少 license                                    |
| config_io           | 周佳锐 | 借助仓颉宏能力简化配置文件读写/加密/校验/监听操作            | 申请通过                                                     |
| crc-cj              | 赵梓博 | 面向仓颉生态的原生 CRC 校验库，支持 CRC-8 至 CRC-64          | 缺少 test，下周重新评审                                      |
| cryptoprimitives4cj | 杨志盛 | 仓颉生态密码学原语库，提供 MD5/SHA/SM3 等摘要                | 升级到 1.1.3 后申请通过                                      |
| hud4cj              | 赵仟亿 | 基于鸿蒙 ArkUI 的通用 HUD 组件库仓颉版本                     | 等 cj-awesome 活动结束，不用单独上 Cangjie-TPC 评审          |
| markit              | 孙岱岳 | 仓颉 Markdown 解析、文档站生成、PDF/Typst 输出等全链路工具链 | 申请通过                                                     |

遗留问题：
1、Cangjie-SunCalc、fraction_js 提交源码并升级版本后，下周重新评审。责任人：符继东/付一、闭环时间：2026-08-24
2、CangjieEmbeddedHAL 补充提交源码。责任人：符继东、闭环时间：2026-08-24
3、cgit 说明 zlib4cj 来源并建议升级到 1.1.3。责任人：高阳、闭环时间：2026-08-24
4、zookeeper_client 补齐 license。责任人：高阳、闭环时间：2026-08-24
5、crc-cj 补齐测试用例后，下周重新评审。责任人：赵梓博、闭环时间：2026-08-24
6、cryptoprimitives4cj 升级到 1.1.3 后建仓。责任人：杨志盛、闭环时间：2026-08-24
7、hud4cj 待 cj-awesome 活动结束后再处理，不单独上 Cangjie-TPC 评审。责任人：方维
8、以上建仓申请决策的落实跟进。责任人：方维/fangwei51@h-partners.com、闭环时间：2026-08-24

**议题2、Cangjie-SIG组织建仓模板评审**

汇报人：方维/fangwei51@h-partners.com

会议结论：
1、在 cangjie-sig 组织新建 TPC-resource 仓库，承载 Cangjie-SIG 组织建仓模板及组织资源；
2、Cangjie-SIG 组织建仓申请按模板与流程进行审核和管理。

遗留问题：
1、完成 cangjie-sig/TPC-resource 仓库创建与建仓模板整理。责任人：赵丹荣、闭环时间：2026-08-24

**议题3、Cangjie-TPC组织分支管理评审**

汇报人：方维/fangwei51@h-partners.com

会议结论：
1、分支管理：develop、main 分支保留；
2、保留 cjc 相关分支：cjc_1.1.3、cjc_1.1.0；
3、ohcangjie 项目版本仅保留 IDE 5.1.1、6.1.1、6.1.1_compatibility，其余小版本归档：

   - 纯仓颉分支：markdown4cj_cangjie-plugin-5.1.1、markdown4cj_cangjie-plugin-6.1.1_compatibility；
   - 互操作分支：markdown4cj_hybrid_cangjie-plugin-5.1.1；
   - 定制分支：avif-ffi_hybrid-cangjie-plugin-5.1.1_xc；


遗留问题：
1、按分支管理要求完成相关仓库分支的梳理与归档。责任人：方维/fangwei51@h-partners.com、闭环时间：2026-08-24