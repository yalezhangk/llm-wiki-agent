---
title: "PIX和DNF7有何区别？"
type: synthesis
tags: []
sources:
  - "DNF7"
  - "PIX"
  - "PIX500"
  - "PIX550"
  - "PMBox"
  - "SmartPIX"
  - "dnf7-chinese-product-catalog-2011"
  - "dnf7-chinese-selection-manual-2017"
  - "dnf7-english-selection-manual-2017"
  - "dnf7-metal-clad-switchgear-technical-instruction-2010"
  - "pix-12kv-24kv-air-insulated-switchgear-catalog-2016"
  - "pix-50ka-catalogue-en"
  - "pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision"
  - "金属封闭开关设备"
relevant_pages:
  - "sources/dnf7-metal-clad-switchgear-technical-instruction-2010.md"
  - "sources/dnf7-chinese-product-catalog-2011.md"
  - "sources/dnf7-chinese-selection-manual-2017.md"
  - "sources/dnf7-english-selection-manual-2017.md"
  - "sources/pix-50ka-catalogue-en.md"
  - "sources/pix-12kv-24kv-air-insulated-switchgear-catalog-2016.md"
  - "entities/SmartPIX.md"
  - "entities/PIX.md"
  - "entities/DNF7.md"
  - "entities/PMBox.md"
  - "entities/PIX500.md"
  - "concepts/温度智能监测.md"
  - "sources/pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision.md"
  - "sources/rm6-sf6-insulated-ring-main-unit-and-compact-switchgear-catalog-2018.md"
  - "concepts/金属封闭开关设备.md"
source_chat_id: "97c72f8b-5a6a-4824-8406-8b4263c92e86"
source_question_message_id: 31
source_assistant_message_id: 32
last_updated: 2026-06-23
---
PIX 与 DNF7 同为施耐德电气的户内空气绝缘金属封闭开关设备，但在电压等级、短路开断能力、电流容量、柜体结构、典型应用和产品变体上存在明显分层。二者不是替代关系，而是覆盖不同中压配电场景的独立产品族。

## 电压等级与适用范围
- **PIX** 主要覆盖 7.2 kV、12 kV、17.5 kV 和 24 kV 系统，英文目录定位为 `17.5 kV‑50 kA‑4000 A` 高性能柜，中文目录覆盖 `PIX‑12kV`、`PIX‑24kV` 及发电机出口断路器方案。[[PIX]] [[pix-50ka-catalogue-en]] [[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]]
- **DNF7** 聚焦 36 kV / 40.5 kV 等级，早期英文技术说明同时给出 `36kV` 与 `40.5kV` 适用范围，后续中文样本固定为 `40.5kV` 系统，面向一次配电。[[DNF7]] [[dnf7-metal-clad-switchgear-technical-instruction-2010]]

## 额定电流与短路开断能力
- **PIX** 最大额定电流可达 **4000 A**（断路器单元），发电机出口柜 **6300 A**；额定短时耐受/开断能力最高 **50 kA**（7.2/12 kV），**63 kA**（12 kV 发电机柜），24 kV 可达 **40 kA**。[[PIX]] [[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]] [[pix-50ka-catalogue-en]]
- **DNF7** 最大母线额定电流 **3150 A**（3150 A 需强制风冷），额定短路开断/短时耐受电流为 **25 kA / 31.5 kA‑4 s**。[[DNF7]] [[dnf7-chinese-selection-manual-2017]]

## 柜体结构与外形尺寸
- **PIX** 采用金属铠装移开式结构（LSC2B‑PM），四隔室（断路器室、母线室、电缆室、继电器仪表室）；尺寸随电压‑电流等级变化：柜宽从 **550 mm（PIX550）、650 mm、800 mm、1000 mm 到 1200 mm**，深度/高度因方案不同而调整。[[PIX]] [[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]]
- **DNF7** 同样为金属铠装移开式、LSC2B‑PM，四隔室（母线室、手车室、电缆室、低压室）；标准柜宽 **1200 mm**（可选 1400 mm），高 2400 mm，深 2750 mm，加深柜最大 3400 mm。[[DNF7]] [[dnf7-chinese-selection-manual-2017]]

## 断路器方案与抽出方式
- **PIX** 以 **HVX embedded pole** 为核心，中文目录还包含 VAH、CVX 接触器‑熔断器组合电器等；整体为移开式，未特别强调中置/落地之分。[[PIX]] [[pix-50ka-catalogue-en]]
- **DNF7** 可配置 **HVX** 真空断路器或 **FP** 型 SF₆ 断路器，相同额定值下两种灭弧方式可互换；早期资料给出 **Middle Rolling** 和 **Floor Rolling** 两种抽出形式，中文手册对应 **KYN28**（中置式）和 **KYN61**（落地式）。[[DNF7]] [[dnf7-metal-clad-switchgear-technical-instruction-2010]] [[dnf7-chinese-selection-manual-2017]]

## 产品变体与应用场景
- **PIX** 族下有多个明确分支：
  - **PIX‑12kV / PIX‑24kV**：标准高性能柜；
  - **PIX‑M**：接触器柜；
  - **PIX‑Gen**：发电机出口断路器柜（至 63 kA）；
  - **PIX550**：柜宽 550 mm 小型化方案；
  - **PIX500**：500 mm 紧凑型，固定联接主回路 + 三工位开关；
  - **Smart PIX**：智能化解决方案。
  应用覆盖重工业、油气、采矿、发电、船舶、基础设施等高要求场景。[[PIX]] [[PIX500]] [[PIX550]] [[SmartPIX]]
- **DNF7** 没有明显的子产品代号，主要通过 **KYN28/KYN61** 结构区分中置/落地式；典型功能单元为进线/馈线、母线分段/隔离、母线提升、母线电压测量和计量。应用更偏向 **40.5 kV 变电站一次配电**，工业领域亦有使用，但定位不如 PIX 宽泛。[[DNF7]] [[dnf7-chinese-selection-manual-2017]]

## 数字化与智能化方案
- **PIX** 通过 **Smart PIX** 接入 EcoStruxure，具备寿命评估、风险预警、千里眼资产顾问、PMB/PMB Easy、嵌入式无线测温、局放在线监测、剩余电寿命、一键顺控、弧光保护和视频监测等能力。[[PIX]] [[SmartPIX]] [[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]]
- **DNF7** 的智能化方案涵盖温度在线监测、断路器特性监测、弧光保护、剩余电寿命评估，并以 **PMBox** 作为主动运维专家，架构偏重站室级资产管理。[[DNF7]] [[PMBox]]

## 标准与认证
- **PIX V8** 目录已引入 GB/T 3906‑2020、IEC 62271‑200:2021，并通过 Green Premium、RoHS、REACh、PCCC、中国质量认证中心产品碳足迹认证等绿色认证。[[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]]
- **DNF7** 资料亦依据 GB/T 3906 与 IEC 62271‑200 组织，但当前 wiki 未突出同等级的绿色认证层级，更侧重于结构、参数与安装交付。[[DNF7]] [[dnf7-chinese-selection-manual-2017]]

## 归纳
- **电压与容量**：PIX 覆盖 7.2 kV↔24 kV，可承载最高 63 kA / 6300 A；DNF7 只服务 36/40.5 kV，31.5 kA / 3150 A。  
- **柜体与结构多样化**：PIX 具备从 550 mm 紧凑型到 1200 mm 的宽度谱系，并有发电机专用方案；DNF7 仅有 1200/1400 mm 两档，通过中置/落地式区分布置。  
- **应用领域**：PIX 更偏向高故障水平工业、发电和海事；DNF7 主要胜任 40.5 kV 配电网的进线、母联和馈线回路。  
- **数字化**：两者均提供智能运维方案，但 Smart PIX 在边缘控制与资产健康服务上整合度更高，DNF7 则通过 PMBox 实现同类功能。

## Sources
- [[PIX]]
- [[DNF7]]
- [[pix-50ka-catalogue-en]]
- [[pix-12kv-24kv-air-insulated-switchgear-catalog-2016]]
- [[pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision]]
- [[SmartPIX]]
- [[PIX500]]
- [[PIX550]]
- [[dnf7-metal-clad-switchgear-technical-instruction-2010]]
- [[dnf7-chinese-product-catalog-2011]]
- [[dnf7-chinese-selection-manual-2017]]
- [[dnf7-english-selection-manual-2017]]
- [[PMBox]]
- [[金属封闭开关设备]]
