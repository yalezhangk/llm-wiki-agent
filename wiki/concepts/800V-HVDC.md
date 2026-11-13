---
title: "800V HVDC (高压直流)"
type: concept
tags: [ai, data-center, hvdc, voltage-standard]
sources: [ai-data-center-800v-hvdc-analysis]
last_updated: 2026-08-25
---

## Key Details
- **定义**：AI数据中心采用的标称母线电压为800V的高压直流供电架构。
- **选型逻辑**：
  - **峰值电压**：系统稳态允许最高约900V，叠加开关关断200V尖峰，峰值达1100V。
  - **器件适配**：完美匹配主流商用1200V SiC MOSFET/IGBT，留有安全裕量且成本最优。
  - **监管边界**：保持在1000V直流红线以内，按低压配电管理，避免高压运维合规成本。
- **拓扑差异**：英伟达MGX/Kyber主推两线制800V（2-wire），中点Hi-Z高阻浮空；另有三线制±400V方案。