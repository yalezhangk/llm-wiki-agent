---
title: "SMD"
type: entity
tags: [product, monitoring, digitalization, substation]
sources: [pix-50ka-catalogue-en, gha-nrjcat18789en-0318, fbx-catalogue-2020, sm6-product-introduction-and-digital-content-2019, smd-and-sensors-for-sm6-training-v2, premset-12kv-compact-modular-vacuum-switchgear-catalog-2020, rm6-set-medium-voltage-switchgear-catalog-2022, rm6-set-medium-voltage-switchgear-catalog-2025]
last_updated: 2026-06-08
---

## Summary
[[SMD]] 是施耐德资料中反复出现的站室级监测设备对象，全称 `Substation Monitoring Device`。在较早目录里它常以数字化选件名出现，而 `SMD and Sensors for SM6 training v2` 则把它展开为能接入 `TH110`、`CL110`、`PT100`、继电器和 `DI` 的监测/告警平台，并给出 `V3 -> V4 -> V4.1 -> V5` 的功能与实施路线。

## Key Details
- 培训稿明确把 `SMD` 写成 `Substation Monitoring Device`，并与 `TH110`、`CL110` 一起作为核心对象。
- 架构页显示其输入可来自 `zigbee` 传感器、`PT100`、`DI` 和 relay 信息，输出面向 local lights、Local HMI、Nearby HMI、`Modbus TCP` 和 `Facility Expert` 的 `SMS` 告警链路。
- `SMD V3` 的能力覆盖 thermal monitoring、environmental monitoring、dry transformer monitoring、CB monitoring、substation alarming、local and remote monitoring、nearby control。
- 热监测对象包括 cable、busbar、CB、withdrawable connections 和 transformer connection；环境监测对象对应 `CL110`；干式变压器监测通过 `PT100`；断路器监测则借助 relay 信息。
- 热算法页给出 `Standard Monitoring`、`Advanced Monitoring`、phase comparison、discrepancy monitoring 和基于实时负荷的 threshold 调整思路，说明 `SMD` 不只是数据转发器，也带有一定分析逻辑。
- 远程告警页补出 `Facility Hero` mobile application、email/SMS alarm notification、`Scada` 和 service platform 接口，显示其定位处于本地监测与远方运维之间。
- 配置流程区分 `Level 1.1` 与 `Level 1.2`：前者围绕 `Thermal Connect App`、`NFC tag`、`Android telephone` 和传感器位置定义；后者强调逐只配对、生成 local file 和在 SMD software 中建项目。
- 版本链在线索上较完整：`V4` 标注 `November 2018`，新增 batch pairing、automatic channel generation、`Easergy P3/P5 compatibility` 和 new relay `Modbus mapping`；`V4.1` 标注 `January 2019`，新增模板化配置与柜位复制；`V5` 则作为 `end of April` roadmap 提到 oil transformer monitoring、ANSI adaptation、double busbar 和 double cubicle。
- `partial discharges sensor` 只出现在 `Wireless sensors roadmap for 2019` 中，因此当前更适合作为规划线索记录，而不是默认写成 `SMD V3` 已成熟内建功能。
- 在产品谱系上，`SMD` 不只服务 [[SM6]]：PIX、GHA、FBX、Premset、RM6 SeT 等资料都把它列入 [[EcoStruxure]] 或数字化中压运维扩展能力，说明它是施耐德跨多条中压产品线复用的监测平台对象。

## Related
- [[施耐德电气]]
- [[数字化中压运维]]
- [[温度智能监测]]
- [[局部放电监测]]
- [[SM6]]
- [[FBX]]
- [[GHA]]
- [[Premset]]
- [[RM6SeT]]
- [[EcoStruxure]]
