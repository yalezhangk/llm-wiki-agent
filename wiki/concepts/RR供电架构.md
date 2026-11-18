---
title: "RR供电架构"
type: concept
tags: [power-architecture, redundancy, data-center]
sources: [large-aidc-power-architecture-2n-tiered-redundancy-green-power]
last_updated: 2026-11-18
---

## Summary
RR（Redundant Redundancy，后备式冗余）供电架构是一种通过公共备用链实现冗余的模式。多套主用电力链分别带载，再共同配置一套备用链。以4+1 RR为例，四套主用系统各带一个负荷块，第五套在故障时接管其中一套，理论容量利用率可以达到80%。其关键在于公共备用母线、转换开关和切换控制必须可靠。

## Key Details
- **结构**：多套主用链+一套公共备用链。
- **利用率**：理论容量利用率可达80%。
- **适用场景**：具备恢复能力的训练机房等可中断负荷。
- **对比**：相比2N和DR，RR通过公共备用提高设备利用率，但依赖切换控制的可靠性。

## Related
- [[AIDC供电架构]]
- [[2N供电架构]]
- [[DR供电架构]]