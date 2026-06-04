---
title: "PIX 50kA Catalogue EN"
type: source
tags: [pix, air-insulated-switchgear, metal-clad-switchgear, medium-voltage]
date: 2019-01-01
source_file: raw/MVE/PIX/PIX 50kA Catalogue_EN.pdf
---

## Summary
这份英文目录介绍了 [[PIX]] 空气绝缘中压开关柜，定位为 17.5kV、50kA、4000A 的高性能 [[金属铠装开关设备]]，并采用 [[HVX]] embedded pole 真空断路器。它把 PIX 放在重工业、油气、矿业、发电和船舶等高要求场景中，补充了当前 wiki 在 [[MVnex]] 之外的高短路开断能力空气绝缘开关柜路线。

## Key Claims
- [[PIX]] 是施耐德电气的空气绝缘开关柜，目录封面给出的能力口径为 17.5kV、50kA、4000A，并配置 [[HVX]] embedded pole。
- PIX 高压部分通过金属隔板分成母线室、电缆室和开关设备室，符合 IEC 62271-200 的 LSC2B-PM 运行连续性和隔板类别。
- 技术参数覆盖 12kV 和 17.5kV，额定短路开断电流为 50kA，额定短路持续时间 3s，最大母线额定电流 4000A。
- [[内部电弧防护]] 口径为 IAC AFLR 50kA/1s，可通过弧光检测与快速跳闸限制内部电弧影响。
- 功能单元包括进线/馈线 F、母线分段 BS、母线提升 BR、母线计量与接地 BME，以及带接触器馈线 FC。
- 保护、监测和控制方案包括 Easergy P5/P3/MiCOM 保护继电器、VAMP 弧光保护、Easergy TH110 温度监测和 Easergy CL110 环境监测。
- PIX 可作为 EcoStruxure-ready 方案的一部分，支持 nearby control、substation monitoring、SCADA/Services 远程监测、云端应用和移动报警。

## Key Quotes
> "Air insulated switchgear 17.5 kV-50 kA-4000 A with HVX embedded pole" — 封面能力描述

> "Protection against internal arc according to the latest IAC test AFLR, 50 kA, 1s" — 安全能力描述

## Connections
- [[PIX]] — 文档核心产品对象。
- [[金属铠装开关设备]] — PIX 采用金属隔板、抽出式主开关设备和 LSC2B-PM 隔室结构。
- [[空气绝缘开关设备]] — PIX 属于空气绝缘中压开关柜路线。
- [[HVX]] — PIX 的主断路器平台为 HVX embedded pole。
- [[内部电弧防护]] — PIX 把 IAC AFLR 50kA/1s 作为安全卖点，并可叠加弧光保护。
- [[温度智能监测]] — TH110 被用于连续监测现场连接点温度。
- [[数字化中压运维]] — PIX 目录将保护继电器、传感器、SMD、HMI、SCADA、云应用和移动报警纳入数字化运维链路。
- [[EcoStruxure]] — 目录把 PIX 相关 connected products 放在 EcoStruxure-ready 方案下。

## Contradictions
- 未发现与 [[MVnex]] 的直接冲突；PIX 应作为更高短路能力的 17.5kV/50kA 空气绝缘开关柜路线理解，而 MVnex 当前资料主要覆盖 12kV、最高 40kA。
- 目录文本中出现 “IEC 62217-200” 表述，结合上下文和后续章节应为 IEC 62271-200，入库时按明显排版/OCR 错误处理。
