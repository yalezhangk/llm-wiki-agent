---
title: "DR供电架构"
type: concept
tags: [power-architecture, redundancy, data-center]
sources: [large-aidc-power-architecture-2n-tiered-redundancy-green-power]
last_updated: 2026-11-18
---

## Summary
DR（Distributed Redundancy，分布式冗余）供电架构是一种通过多套电力链交叉供电实现冗余的模式。三套或更多电力链正常共同带载，并通过交叉供电互相备份。任何一套退出后，负荷分配到剩余系统。DR没有固定闲置的备用链，理论容量利用率高于2N，但交叉配电、负荷均衡和故障转移逻辑更复杂。

## Key Details
- **结构**：三套或更多电力链交叉供电，无固定闲置备用链。
- **利用率**：理论容量利用率高于2N。
- **适用场景**：具备恢复能力的训练机房等可中断负荷。
- **对比**：相比2N，DR通过交叉连接共享冗余，提高设备利用率，但逻辑更复杂。

## Related
- [[AIDC供电架构]]
- [[2N供电架构]]
- [[RR供电架构]]