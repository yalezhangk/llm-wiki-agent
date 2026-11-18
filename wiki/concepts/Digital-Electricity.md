---
title: "Digital Electricity (数字电力)"
type: concept
tags: [data-center, hvdc, digital-electricity, safety, power-distribution]
sources: [four-level-distribution-digital-electricity-data-center]
last_updated: 2026-11-18
---
## Key Details
- **定义**：Digital Electricity是一种融合实时故障管控与柔性数字化配电的技术，由VoltServer公司提出。
- **核心机制**：
  - **分组式电力传输**：将电力分割为多组智能管控的电能“数据包”，每组数据包在输送至负载前都会完成安全校验。
  - **故障管控**：一旦检测到线路故障、电弧、人体误触等异常，系统将在毫秒级切断电力传输，从根源消除失控电弧、触电等重大安全风险。
  - **数字化管控**：所有回路均数字化管控，任何异常都能提前识别并处置，避免故障进一步扩大。
- **优势**：
  - **安全性**：解决传统高压直流在高压工况下安全性不足、运维难度高的问题。
  - **能效**：大幅减少交直流反复转换环节，降低电能损耗。
  - **空间优化**：可采用轻量化通信线缆铺设，线缆能够与通信线路共用桥架、走线通道，减少机房专门用于布线的空间。
  - **灵活性**：部署、扩容、改造流程简便安全，无需大规模土建施工或冗余预留建设。
- **应用场景**：集装箱式数据中心、预制模块化数据中心、边缘数据中心。

## 关联页面
- [[800V-HVDC]]：Digital Electricity与800V HVDC架构互补，解决安全设计难题。
- [[Sidecar]]：Digital Electricity的轻量化线缆和紧凑设计可能与Sidecar边柜的部署理念有相似之处。