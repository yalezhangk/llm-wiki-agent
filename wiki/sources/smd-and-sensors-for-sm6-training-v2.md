---
title: "SMD and Sensors for SM6 training v2"
type: source
tags: [smd, sm6, sensors, training, digitalization, monitoring]
date: 2018-10-01
source_file: raw/MVP/SM6/SMD and Sensors for SM6 training v2.pptx
---

## Summary
这份 `31` 页英文培训稿把 `SMD` 从目录中的一个缩写选项推进成可实施的站室级监测设备对象。它围绕 `SMD V3` 功能、`TH110`/`CL110` 传感器、配对配置流程以及 `V4 / V4.1 / V5` 版本路线展开，同时把资料边界明确停留在 `2018.10` 培训与 roadmap 阶段，而不是正式产品目录或当前量产清单。

## Key Claims
- 封面标题为 `SMD & Sensors presentation`，副标题写明 `Substation Monitoring Device – TH110 – CL110`，作者 `Paolo TARDITO`，时间为 `October 2018`。
- 议程显示这份资料主要覆盖 `SMD Introduction`、`SMD V3 functions`、`TH110 / CL110`、配对配置步骤和 `SMD V4` 后续功能。
- `SMD` 被描述为面向配电站室的状态监测设备，价值叙事围绕 `24/7` 监测、即时告警、减少非计划停机和从 time-based maintenance 转向 condition-based maintenance。
- 架构页给出 `SMD` 的输入来源包括 `zigbee` 传感器、`PT100`、`DI` 和继电器信息；输出去向包括 local lights、Local HMI、Nearby HMI、`Modbus TCP` 以及发往 `Facility Expert` 的 `SMS`。
- `SMD V3` 功能页把能力列成 thermal monitoring、environmental monitoring、dry transformer monitoring、CB monitoring、substation alarming、local and remote monitoring、nearby control。
- 热监测页把对象写成 cable、busbar、CB、withdrawable connections 和 transformer connection，并强调采用 innovative wireless sensor。
- 热算法页给出 `Standard Monitoring`、`Advanced Monitoring`、phase comparison、discrepancy monitoring，以及基于电流、柜体额定电流和热极限的 real-time threshold。
- 干式变压器监测通过 `PT100` 监测绕组；断路器监测则基于 relay 信息判断操作机构和主回路健康。
- 远程告警页提到 `Facility Hero` mobile application、mobile or emails alarm notification、`SMS`，以及接入 `Scada` 或 service platform。
- `TH110` 被定位为紧凑型无线温升传感器，用于 critical points；`CL110` 被定位为环境监测传感器，标注 `IP54`、indoor applications、battery powered 和 `life expectation >15 years`。
- 配对配置部分区分 `Level 1.1` 与 `Level 1.2`：前者用 `Thermal Connect App`、`NFC tag`、传感器位置定义和 `Android telephone`；后者强调逐只传感器通电配对、本地保存 ID/position/channel 和在 SMD software 中建立项目。
- `SMD V4` 标注 `release in November 2018`，新增 batch pairing、easy configuration、channel automatic generation、`Easergy P3 and P5 compatibility` 和新的 `Modbus mapping for new relays`。
- `SMD V4.1` 标注 `release January 2019`，新增 threshold easier configuration、copy/paste cubicle、change cubicle position in SLD、export/import cubicle as template 和 cubicle library。
- `SMD V5` 被写成 `release end of April` 的 roadmap，计划补充 oil transformer monitoring、ANSI adaptations、`CL110 in free location`、wireless sensor signal status、busbar/double busbar monitoring 和 double cubicle。
- `Wireless sensors roadmap for 2019` 中还把 partial discharges sensor 列为“next”方向，并说明 ambient air PD 与 humidity、condensation、pollution 相关，因此它应视为规划项，而不是这份资料时点的既有标配。

## Key Quotes
> "SMD & Sensors presentation" — 封面标题

> "Substation Monitoring Device – TH110 – CL110" — 设备与传感器关系

## Connections
- [[SMD]] — 本文档把它从缩写选项展开为独立监测设备对象。
- [[SM6]] — 文件名表明培训语境面向 SM6 路线。
- [[数字化中压运维]] — 资料把监测、告警、远程接入和版本迭代放在同一运维链条中。
- [[温度智能监测]] — `TH110` 和热算法是主体内容之一。
- [[局部放电监测]] — `partial discharges sensor` 在 2019 roadmap 中被提为下一步方向。
- [[施耐德电气]] — `SMD`、`Facility Hero`、`Facility Expert` 和 `Easergy P3/P5` 均处于施耐德命名体系中。

## Contradictions
- 与《SM6 7.2~24kV 空气绝缘环网柜》来源页不冲突，但角色不同：后者偏产品谱系与监测对象说明，这份培训稿偏 `SMD` 软件/传感器实施与版本路线。
- 需要显式保留时间边界：`V4 / V4.1 / V5`、`partial discharges sensor`、`CL110 in free location`、double busbar 和 double cubicle 都在 roadmap 或培训稿阶段出现，不能直接写成当时已正式量产或已成为所有产品线标配。
