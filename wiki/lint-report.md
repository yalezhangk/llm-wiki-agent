# Wiki Lint Report — 2026-06-23

Scanned 142 wiki pages.

## 执行说明

- **执行方式:** Codex agent 直接执行语义 lint，未调用 `tools/llm_config.py`。
- **外部 LLM 消耗:** 无 DeepSeek API 消耗。
- **结构信号来源:** 复核 `tools.lint` 的确定性检查结果，并读取 `wiki/index.md`、`wiki/overview.md`、`graph/graph.json`、`graph/graph-report.md` 及高风险页面。
- **报告范围:** `68` 个 source、`43` 个 entity、`28` 个 concept、`1` 个 synthesis。

---

## Structural Issues

### Broken Wikilinks

未发现断链。

### Missing Entity Pages

未发现高频提及但缺失独立页面的实体。

### Orphan Pages

发现 `53` 个 orphan pages。主要集中在 `wiki/sources/` 下的来源页，另有 `wiki/health-report.md` 与一个 synthesis 页面。

这些 orphan 并不等同于内容不可发现，因为来源页仍可通过 `wiki/index.md`、`wiki/log.md` 和相关实体/概念页的 `sources:` frontmatter 间接发现；但从 wikilink 图谱角度看，反向链接不足，会削弱图谱导航和社区连接。

高优先级处理建议：

- 从相关 entity / concept 页补充到关键 source 页的反向 `[[wikilinks]]`。
- 对 synthesis 页面增加来自 index、overview 或相关实体页的入口。
- `health-report.md` 属自动报告，可接受低链接密度，也可从 `wiki/index.md` 的 Reports 区保留入口。

### Sparse Pages

仅发现 `1` 个低出链页面：

| Page | Outbound Links |
|---|---:|
| `wiki/health-report.md` | 0 |

---

## Graph-Aware Issues

当前图谱文件与 wiki 页面规模不一致：

- 当前 wiki 页面数：`142`
- `graph/graph-report.md` 记录节点数：`78`
- `graph/graph.json` 的 `built` 时间：`2026-06-10`

因此，本轮不应把现有 graph-aware 报告当作当前全量事实。建议重新运行 graph workflow，并保存新的 graph report。

建议命令：

```powershell
& '.venv\Scripts\python.exe' -X utf8 tools\build_graph.py --report --save
```

如需打开可视化，再运行：

```powershell
& '.venv\Scripts\python.exe' -X utf8 tools\build_graph.py --open
```

---

## Semantic Issues

### Smart HVX 可靠性口径不一致

`smart-hvx-product-introduction-v3-4.md` 已标出同一资料中存在两类表述：

- `可靠性提高 1 倍`
- `可靠性高出 50%`

这不是可以直接合并的同义表达。建议继续作为开放核对点，后续引用时标注具体页面或避免给出统一数值。

### WIG / WSG 通信规约疑似笔误

多个 WIG / WSG 相关来源中出现 `IEC61580`，结合上下文很可能是 `IEC 61850` 的误写。

受影响页面包括：

- `wiki/sources/wig-high-speed-rail-smart-switchgear-jiaoda-yunda-protection-pasific-window.md`
- `wiki/sources/wsg-wig-smart-switchgear-2019.md`

建议保持现有“疑似笔误”处理，不要自动替换原文；工程引用时回到原图纸或通信清单核对。

### WS-G 参数版本口径并存

WS-G 当前同时存在以下口径：

- 早期材料 / 操作说明书：`2500A / 31.5kA`
- 2024 企业标准和产品目录：`3150A / 40kA`
- 图片页或特定应用：`4000A` 双母线

当前 wiki 将其解释为版本、配置或项目应用口径差异，是合理处理。后续工程引用必须带来源版本，避免把宣传页或旧说明书参数覆盖到正式目录。

### WS-G 气体年泄漏率差异

`wsg-feature-highlights-image.md` 给出 `<0.01%/年`，明显严于标准/目录中常见的 `<0.1%/年`。

建议保留为宣传页单独说法；正式参数引用优先采用企业标准或产品目录。

### BLink 峰值电流差异

GHA 旧 PPT 与 2018 catalog 对 BLink 峰值电流存在差异：

- 旧 PPT：`104kA`
- 2018 catalog：`100kA`

当前 `overview.md` 已记录该差异。后续引用应优先使用正式 catalog 或具体项目订货文件。

### SM6 分类边界

SM6 页面中“空气绝缘柜体”和 `SF6` 密闭开关间隔并存。当前 wiki 对其边界处理基本正确：SM6 可归入空气绝缘开关设备叙事，但不应被写成纯空气绝缘、完全无气体介质的路线，也不应直接并入 RM6 / FBX 这类紧凑气体绝缘 RMU 口径。

---

## Data Gaps

当前最值得补充或核对的材料：

- Smart HVX 可靠性提升数值的原始页或正式发布口径。
- WIG / WSG 中 `IEC61580` 的原始图纸和通信清单。
- WS-G 不同年份目录、企业标准和项目图片页之间的适用边界。
- BLink 在 GHA 不同资料版本中的正式型式试验参数。
- PIX / MVnex 小型化分支之间的品牌、平台和工程差异边界。

---

## Conclusion

当前 wiki 内容质量总体可用。主要冲突大多已被整理为“版本差异”“资料层级差异”或“待核对点”，未发现新的严重语义矛盾。

优先维护事项：

1. 重建并保存当前全量 graph report。
2. 为关键 source 页面补充来自 entity / concept 页的反向链接，减少 orphan source。
3. 对 Smart HVX、WS-G、WIG/WSG 通信规约、BLink 等开放核对点保留明确版本标注。
