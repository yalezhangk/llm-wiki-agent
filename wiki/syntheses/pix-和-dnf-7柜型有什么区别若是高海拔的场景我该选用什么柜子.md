---
title: "PIX 和 DNF 7柜型有什么区别？若是高海拔的场景我该选用什么柜子？"
type: synthesis
tags: []
sources:
  - "overview.md"
  - "entities/PIX.md"
relevant_pages:
  - "overview.md"
  - "entities/PIX.md"
source_chat_id: "19"
source_question_message_id: 37
source_assistant_message_id: 38
last_updated: 2026-11-18
---
## PIX 与 DNF7 的核心区别

两者同属施耐德电气的**户内交流空气绝缘金属封闭开关设备**，都采用四隔室结构、LSC2B 运行连续性、PM 级金属隔板，且都可以配装 [[HVX]] 真空断路器，但在电压等级、电流/短路参数、产品族宽度和典型应用场景上存在明显分层。[[entities/PIX|PIX]]

| 维度 | PIX | DNF7 |
|---|---|---|
| **额定电压** | 7.2 / 12 / 24 kV（英文目录另见 17.5 kV） | 36 / 40.5 kV |
| **额定电流** | 630 A ~ 4000 A；PIX-Gen 可达 5000 A / 6300 A | 2500 A（2011 目录）→ 3150 A（后续版本） |
| **短路开断** | 20 kA ~ 50 kA；PIX-Gen 63 kA | 31.5 kA |
| **内部电弧（IAC）** | AFLR 50 kA/1 s（7.2/12 kV）；AFLR 40 kA/1 s（24 kV） | AFLR 31.5 kA/1 s |
| **断路器选项** | HVX、VAH、CVX（接触器-熔断器组合） | HVX 真空断路器 或 FP SF₆ 断路器 |
| **柜宽** | 500 mm（PIX500）/ 550 mm（PIX550）/ 标准柜 | 1200 mm / 1400 mm |
| **子产品族** | PIX-12kV、PIX-24kV、PIX-M、PIX-Gen、PIX550、PIX500、Smart PIX | 标准型、Middle Rolling / Floor Rolling 抽出式 |
| **典型应用** | 公共/工业中压配电、重工业、油气、采矿、发电、船舶、数据中心、商业建筑 | 40.5 kV 工业配电、石化、冶金、风电升压站、轨道交通 |
| **数字化层** | Smart PIX：PMB/PMB Easy、无线测温、局放、一键顺控、剩余电寿命、视频、弧光、环境温湿度 | 2025 版接入 EcoStruxure、PMBox、PMB Easy、千里眼资产顾问 |

简言之，**PIX 覆盖 7.2~24 kV（英文 17.5 kV）的宽电压、大电流（最高 6300 A / 63 kA）场景，产品族更宽、小型化分支更多；DNF7 则锁定 36/40.5 kV 高电压等级，电流和短路参数相对收敛，但多了 FP SF₆ 断路器选项和 KYN28/KYN61 结构体系。** 两者不是替代关系，而是同一空气绝缘技术路线下不同电压/电流段的产品分支。[[overview|Overview]]

## 高海拔场景的选型建议

在已入库的 wiki 资料中，**PIX 和 DNF7 的现有页面均未给出明确的高海拔额定值**，因此不能仅凭这两条产品线直接判定高海拔适用性。wiki 中明确标注了高海拔能力的主要是以下产品：

- **WSG（气体绝缘金属封闭开关设备）**：2024 企业标准将特殊使用海拔提高到 **5500 m**，2014 演示稿中特殊型为 4000 m，2018 目录常规口径为 1000 m。[[overview|Overview]]
- **Premset（屏蔽式固体绝缘开关设备）**：2020 目录明确列出 **5000 m** 海拔边界。[[overview|Overview]]
- **FLUSARC（40.5 kV SF₆ 绝缘中压开关柜）**：最大海拔 **2000 m**。[[overview|Overview]]

因此，如果项目海拔超过常规 1000 m：

1. **40.5 kV 等级、海拔 ≤ 5500 m**：优先考虑 **WSG** 气体绝缘路线，其 2024 标准已覆盖 5500 m，且 SF₆ 密封气室结构天然适合高海拔（气压降低对气体绝缘的影响小于空气绝缘）。[[overview|Overview]]
2. **12/24 kV 等级、海拔 ≤ 5000 m**：可考虑 **Premset** 屏蔽式固体绝缘路线，固体绝缘不受海拔气压变化影响，2020 目录已给出 5000 m 边界。[[overview|Overview]]
3. **若必须使用 PIX 或 DNF7**：wiki 现有资料未提供高海拔额定值，需要向施耐德项目团队确认具体型号的降容系数和海拔修正要求，不能直接按常规 1000 m 参数选型。[[entities/PIX|PIX]]

> **提示**：高海拔场景下空气绝缘设备的绝缘强度会随气压下降而降低，气体绝缘（WSG/GHA）和固体绝缘（Premset）路线在工程上通常更具优势。最终选型应结合具体海拔、电压等级、短路电流和当地标准，以正式产品目录和订货文件为准。[[overview|Overview]]
