---
title: "DVCAS Switchgears for Transformer Substations in Wind Farms"
type: source
tags: [dvcas, wind-farm, ring-main-unit, secondary-distribution, gas-insulated, catalog]
date: 2007-01-01
source_file: raw/二次气体绝缘开关柜/CAS&DVCAS/SCDOC-DVCAS-EN.pdf
---

## Summary
这份 `01/2007` 英文目录把 [[DVCAS]] 定位为风电场用 `36kV` 中压二次配电开关柜，面向风机箱变和集电网场景。与刚入库的 `CAS 36` 单页式目录层不同，这份资料给出了更完整的工程骨架：`36kV / 630A / 20kA`、`IP67` 高压隔室、`SF6 0.3 bar`、`I / D / 0 / T` 模块化功能，以及风机塔筒内安装、故障隔离和远方恢复供电的应用逻辑。它更像施耐德体系内一条偏风电专用的早期 RMU / GIS 分支，而不是后续 [[RM6]]、[[FBX]]、[[SM6]] 的简单前身。

## Key Claims
- 封面将产品写为 `DVCAS Switchgears for transformer substations in wind farms`，并标注 `36 kV`、`SECONDARY DISTRIBUTION SWITCHGEAR`。
- 资料把应用场景明确限定在风电场集电网与风机箱变，强调 `36 kV` 是新风电场的主导趋势，并要求设备可穿过仅 `600 mm` 宽的风机门洞。
- 目录说明 [[DVCAS]] 适用于海拔 `2000 m` 以内的风电场。
- 总参数页给出：额定频率 `50Hz`、额定电压 `36kV`、工频耐压 `70kV`、雷电冲击耐压 `170kV`、主母线额定电流 `630A`、短时耐受 `20kA / 3s`、短路开断能力 `20kA`、关合能力 `50kA peak`、内部电弧 `IAC AFL 20kA / 1s`。
- 防护等级写为高压隔室 `IP67`、低压与操作机构隔室 `IP3X`，`SF6` 在 `20℃` 下压力为 `0.3 bar`。
- 结构上每个模块单元包含金属底架、操作与继保隔室、电缆隔室，以及容纳母线与开断元件的不锈钢密封气箱；绝缘介质为 `SF6`。
- 资料将柜型功能模块写为 `D` 保护功能、`I` 进线三工位负荷开关、`0` 出线刚性提升、`T` 带接地开关的提升，并通过 `NE / LE / RE / DE` 表示左右扩展能力。
- 推荐的风电场标准功能组包括 `NE-D0`、`NE-ID0` 和 `NE-IID0`，分别对应变压器保护加出线、再加一路进线、再加两路进线。
- `D` 保护单元采用真空断路器，文中写为 `Evolis CAS`，并给出 `E2` 电寿命、`M1/2000` 机械寿命，以及 `VIP-35` 自供电继电器与 `CSH-30` 零序电流传感器。
- `I` 进线单元采用 `SF6` 自气吹灭弧的三工位开关，可选 `48Vdc` 电动操作、`230Vac` 充电整流及 `Flair` 故障指示，实现远方故障隔离和供电恢复。
- 电缆室采用符合 `EN 50181` 的 `C` 型套管，口径写为 `630A / 25kA / M16`，并支持每相两根电缆连接。
- 目录把该产品归入 MESA 路线，说明 MESA 为 Schneider Electric 成员企业，并强调其在风电场中压开关柜上的大量装机经验。

## Key Quotes
> "DVCAS switchgears can go through doors only 600 mm wide." — 风机塔筒内安装边界的直接表述。

> "These DVCAS switchgears can be installed in wind farms up to 2000 m over the sea level." — 海拔适用范围说明。

## Connections
- [[DVCAS]] — 资料核心产品对象。
- [[施耐德电气]] — 资料所属集团背景。
- [[气体绝缘开关柜]] — 资料属于 `36kV` 风电场二次配电气体绝缘路线。
- [[CAS36]] — 同目录夹中的更简版 `CAS 36` 资料，可作为相近时期的早期 RMU 命名层对照。
- [[RM6]] — 后续更通用的施耐德二次配电环网柜路线。
- [[FBX]] — 后续更标准化的二次配电 GIS / RMU 目录路线。

## Contradictions
- 与 [[CAS36]] 不构成直接冲突；更适合把两者理解为相近时期的相邻资料层：[[CAS36]] 更像简要产品叙事页，[[DVCAS]] 则是风电专用工程目录。
- 与 [[RM6]]、[[FBX]]、[[SM6]] 不应视为同一产品的简单旧版本关系；[[DVCAS]] 明显更聚焦 `36kV` 风电场集电网与箱变应用，而后者更偏通用二次配电环网柜 / RMU。
