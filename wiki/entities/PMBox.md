---
title: "PMBox"
type: entity
tags: [product, edge-control, predictive-maintenance, asset-management]
sources: [smart-hvx-product-pmb-introduction, dnf7-indoor-ac-metal-enclosed-switchgear-2025-4-10]
last_updated: 2026-06-04
---

## Summary
[[PMBox]] 是施耐德在 [[EcoStruxure]] Power 架构下的边缘控制层产品，资料称其部署在配电现场，通过集成互联互通层设备信息进行数据建模与分析。相较于专门面向 [[SmartHVX]] 的 [[PMBEasy]]，PMBox 的范围更偏站室级资产管理、状态监测和预测性维护。

## Key Details
- 文档把 PMBox 称为“主动运维专家”，强调优化配电资产全生命周期管理。
- 核心能力分为资产管理、状态监测和预测性维护三类。
- 状态监测覆盖电气参量、设备状态参量、元件状态、环境温湿度、微机保护信息和历史数据追溯。
- 预测性维护包括基于负载电流的温升算法、[[局部放电监测]]/分析、分合闸线圈、储能电气寿命预估和设备整体健康状态管理。
- 界面能力包括首页关键运维信息视图、间隔分页、智能断路器分页和历史数据查询。
- 应用架构中，PMBox 可通过 Ethernet、Modbus、hard wire 和 wireless 等方式接入智能网关、采集器、保护装置、局放监测、Smart HVX 与温湿度传感器。
- DNF7 样本把 PMBox 放入 [[DNF7]] 智能化方案，作为面向中压智能配电和一线运维人员的主动运维专家。

## Related
- [[EcoStruxure]]
- [[主动运维]]
- [[数字化中压运维]]
- [[DNF7]]
- [[SmartHVX]]
- [[PMBEasy]]
- [[局部放电监测]]
- [[Link150]]
- [[ZBRN32]]
- [[BMM]]
