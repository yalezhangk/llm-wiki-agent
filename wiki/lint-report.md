# Wiki Lint Report — 2026-06-05

Scanned 77 wiki pages (78 including health-report.md).

## 执行说明

- **Pre-flight health:** 通过（零问题）
- **确定性检查:** 通过 `tools/lint.py` 及手动交叉验证
- **语义检查:** 由独立代理手工完成（litellm 未配置模型 provider）
- **图谱感知检查:** 跳过（需先运行 `build graph` 生成 `graph.json`）

---

## 结构性检查

### Orphan Pages（27 页 — 无入链）

全部为 `wiki/sources/` 下的源页面。来源页面通过 `wiki/index.md`、`wiki/log.md` 和 YAML frontmatter 中的 `sources:` 字段可发现，严重性较低。

```
wiki/sources/3-smart-hvx-intelligent-medium-voltage-circuit-breaker-solution-overview-single-page.md
wiki/sources/dnf7-indoor-ac-metal-enclosed-switchgear-2025-4-10.md
wiki/sources/gha-gas-insulated-switchgear-presentation-vers-06-englisch.md
wiki/sources/gha-nrjcat18789en-0318.md
wiki/sources/gm-airset-medium-voltage-primary-gas-insulated-switchgear-v1-1.md
wiki/sources/gma-air-c4c-digital-implement-20191204.md
wiki/sources/gma-medium-voltage-primary-gas-insulated-switchgear-v1-5.md
wiki/sources/gma-nrjed311328en-1017.md
wiki/sources/hvx-manual.md
wiki/sources/mvnex-medium-voltage-metal-clad-switchgear.md
wiki/sources/pix-50ka-catalogue-en.md
wiki/sources/pix-catalogue-indoor-ac-metal-enclosed-switchgear.md
wiki/sources/pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision.md
wiki/sources/pix500-catalogue-armored-metal-enclosed-switchgear.md
wiki/sources/pix550-catalogue.md
wiki/sources/pmb-easy-johnson-v1.md
wiki/sources/q320500-ksga-09-2015-wsg-enterprise-standard.md
wiki/sources/qavxm-031-2024-wsg-enterprise-standard.md
wiki/sources/smart-hvx-product-introduction-v3-4.md
wiki/sources/smart-hvx-product-pmb-introduction.md
wiki/sources/wi-g-railway-gas-insulated-switchgear-operation-instructions.md
wiki/sources/wig-high-speed-rail-smart-switchgear-jiaoda-yunda-protection-pasific-window.md
wiki/sources/wsg-12-40-5kv-ac-metal-enclosed-gas-insulated-switchgear-catalog-2024.md
wiki/sources/wsg-2014-06-27-product-presentation.md
wiki/sources/wsg-40-5kv-gas-insulated-switchgear-image.md
wiki/sources/wsg-gas-insulated-metal-enclosed-switchgear-operation-instructions.md
wiki/sources/wsg-wig-smart-switchgear-2019.md
```

### Broken Wikilinks（0 处）

✅ 无断链 — 所有 `[[链接]]` 都有对应页面。

### Missing Entity Pages（0 个）

✅ 无高频（≥3 次）提及但缺少独立页面的实体名。

### Sparse Pages — 低出链密度（1 页）

| Page | Outbound Links |
|---|---|
| `wiki/health-report.md` | 0 |

仅 `health-report.md` 不满足 ≥2 出链的密度预算。该页面为自动生成的报告，可接受。

---

## 语义检查

### 矛盾

#### 1. PIX550 "最小" vs PIX500 真正最小（⚠️ 建议修复）

- **PIX.md:** "PIX550 是 PIX 旗下尺寸最小的 12kV 中置式金属封闭开关设备"
- **PIX500 source page:** "最新加入 PIX 产品家族的尺寸最小的空气绝缘中压成套开关设备"
- **事实:** PIX500 柜宽 **500mm**，PIX550 柜宽 **550mm**，PIX500 客观上更小。
- **原因:** PIX550 可能是"最小中置式/可抽出式"，PIX500 是"最小固定式"。两页面互不引用对方的"最小"声明导致冲突。PIX550.md 虽描述了与 PIX500 的结构差异，但未限定"最小"的修饰范围。

#### 2. PIX550/MVnex550、PIX500/MVnex500 规格完全重叠，无区分（🔴 重要）

| 维度 | MVnex 550 | PIX550 | MVnex 500 | PIX500 |
|------|-----------|--------|-----------|--------|
| 电压 | 12kV | 12kV | 12kV | 12kV |
| 电流 | ≤1250A | ≤1250A | ≤1250A | ≤1250A |
| 短路 | ≤31.5kA | ≤31.5kA | ≤31.5kA | ≤31.5kA |
| 柜宽 | 550mm | 550mm | 500mm | 500mm |
| 断路器 | HVX 固封 | HVX 手车 | HVX 固封+固定 | HVX 固封+固定 |

四个实体页面 (MVnex, PIX, PIX550, PIX500) 互不交叉引用。overview.md 称"不是冲突关系，而是同属空气绝缘/金属铠装方向下不同参数段和应用场景的产品分支"，但规格完全相同时"参数段"说法不成立。**wiki 未解释这是同一 OEM 平台的不同品牌/渠道命名，还是确有工程差异。**

#### 3. ILIS 仅出现在 2010 PPT — 2018 目录未确认（⚠️）

- **ILIS.md** 仅依赖 `gha-gas-insulated-switchgear-presentation-vers-06-englisch`（2010 年 PPT）
- **GHA 2018 catalog** 提到 VAMP arc mitigation 和 Easergy P3 作为电弧保护方案，完全未提及 ILIS
- wiki 未标记"ILIS 可能已被 VAMP 弧光保护替代"的风险

#### 4. BLink 峰值电流差：104kA vs 100kA（已标注）

- BLink.md 和 overview.md 已记录，但未给出推荐值（对工程设计有实际影响的 4% 偏差）

#### 5. Smart HVX 可靠性倍数仍未解决（已标注）

- SmartHVX.md 记录 V3.4 同时出现"提高 1 倍"和"高出 50%"
- 后续 ingest 更多来源后仍未推进结论

---

### 陈旧内容

#### 1. `entities/千里眼.md` — 严重过时（🔴）

- **last_updated:** 2026-06-03，仅 2 个 Smart HVX 来源
- 后续 PIX V8、DNF7、Smart MVnex、WSG-WIG 均引用千里眼作为远程运维平台
- 千里眼已从"Smart HVX 的云端显示"扩展为施耐德中压产品家族的通用资产顾问平台

#### 2. `entities/PMBEasy.md` — 缺少跨产品线引用

- **last_updated:** 2026-06-03，仅有 Smart HVX 相关来源
- PIX V8 和 SmartPIX.md 都提到 PMB/PMB Easy 是 Smart PIX 的组件，页面未反映

#### 3. `entities/DNF7.md` — 单一来源未更新

- 仅 1 个来源，后续 ingests 的 WSG/GHA（同为 40.5kV 开关柜品类）无交叉引用

#### 4. `concepts/测温技术对比.md` — 局限于 Smart HVX 视角

- 仅 1 个来源 (Smart HVX V3.4)。WSG-WIG、GMA Air C4C 等来源讨论了 TH110、CL110、RFID/Zigbee、光纤等不同测温方案但未整合

#### 5. `concepts/ILIS.md` — 单一来源，未与 VAMP 弧光保护关联

- 仅 2010 PPT。PIX 和 GHA 2018 目录均提到 VAMP 弧光保护，页面未做对比

#### 6. `entities/GMA.md` — sources 包含非 GMA 来源

- sources 列表包含 `gha-gas-insulated-switchgear-presentation-vers-06-englisch`（实为跨产品线参考，非 GMA 数据来源）

---

### 数据缺口

#### 1. PIX vs MVnex：何时选择哪个？没有解释

- 规格高度重叠，但 wiki 无页面解释市场划分
- **建议来源:** 施耐德中压配电产品选型指南、区域产品目录（中国 vs 国际）

#### 2. Smart PIX vs Smart MVnex：同一方案还是不同的？

- 两者能力清单几乎一致（TH110、P3/VAMP、PMB/PMB Easy、千里眼）
- **建议来源:** 施耐德智能化解决方案对照表

#### 3. ILIS 是否仍在产？可否替换为 VAMP？

- **建议来源:** 当前 GHA 产品目录、报价软件选项、生命周期状态公告

#### 4. GHA vs WS-G：同达 40.5kV 气体绝缘，各自定位？

- 两个实体页独立存在，无对比维度
- **建议来源:** 施耐德全球 GIS 产品组合手册

#### 5. SF6 监管合规路线图

- PIX500 和 GM AirSeT 宣传"无 SF6"，但大量产品仍用 SF6。无相关法规讨论
- **建议来源:** 施耐德可持续发展报告、EU F-Gas 法规影响分析

#### 6. 缺少产品型号对照表

- 面对 GMA/GMAirSeT/GHA/WSG/WIG/PIX/PIX550/PIX500/MVnex/DNF7，无任何矩阵对比
- **建议:** 创建 `wiki/syntheses/product-comparison.md`

---

### 需要深化的概念

#### `entities/SmartPIX.md` — 单来源、薄

- 仅 28 行（vs SmartHVX.md 35 行、6 个来源）。Smart PIX 的 PMB Easy/千里眼链路是否与 Smart HVX 共享相同软硬件栈？未说明。

#### `concepts/ILIS.md` — 技术深度不足

- 仅 23 行，无原理说明，未与 VAMP 弧光保护（5-7ms、过流闭锁）做对比

#### `entities/MVnex.md` — 缺少与 PIX 的直接对比

- 尽管与 PIX 在 550/500 规格上完全相同，仅轻轻带过，未做任何对比说明

#### `concepts/BLink.md` — 跨产品线通用性未确认

- BLink 同时出现在 GHA 和 WS-G 中，这是否是施耐德 GIS 的统一母线连接方案？wiki 未回答

#### `entities/EcoStruxure.md` — 仍为简介

- 30 行，未按三层架构（互联互通/边缘控制/应用分析）展开具体产品和它们的关系

---

## 图谱感知检查

跳过。运行 `build graph` 后重新 lint 以启用。

---

## 建议优先修复

| 优先级 | 问题 | 修复方式 |
|--------|------|----------|
| 🔴 高 | PIX vs MVnex 规格重叠未澄清 | 在 overview/PIX/MVnex 页面添加显式说明 |
| 🔴 高 | 千里眼.md 过时 | 更新以反映跨产品线平台角色 |
| ⚠️ 中 | PIX550/PIX500 "最小"矛盾 | 添加限定词明确范围 |
| ⚠️ 中 | ILIS 单一来源风险 | 标注"仅 2010 PPT，后续目录未确认" |
| ⚠️ 中 | PMBEasy.md 缺跨线引用 | 补充 Smart PIX 引用 |
| 💡 低 | 缺少产品对照表 | 创建 `wiki/syntheses/product-comparison.md` |
| 💡 低 | SF6 合规路线图 | 寻源 EU F-Gas 法规文档 |
