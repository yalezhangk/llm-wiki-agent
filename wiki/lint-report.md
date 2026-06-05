# Wiki Lint Report — 2026-06-04

Scanned 67 wiki pages.

## Execution Notes

- Pre-flight `health` passed before lint.
- Deterministic lint checks completed locally with `tools/lint.py`.
- Semantic lint through `litellm` did not complete because no local provider/model is configured for the default model `claude-3-5-sonnet-latest`.
- Manual semantic review was performed by the agent using the current wiki pages.
- Graph-aware checks were skipped because `graph/graph.json` does not exist yet.

## Structural Issues

### Orphan Pages

19 orphan pages were found. All are source pages under `wiki/sources/`, not entity or concept pages.

- `wiki/sources/3-smart-hvx-intelligent-medium-voltage-circuit-breaker-solution-overview-single-page.md`
- `wiki/sources/dnf7-indoor-ac-metal-enclosed-switchgear-2025-4-10.md`
- `wiki/sources/gha-gas-insulated-switchgear-presentation-vers-06-englisch.md`
- `wiki/sources/gha-nrjcat18789en-0318.md`
- `wiki/sources/gm-airset-medium-voltage-primary-gas-insulated-switchgear-v1-1.md`
- `wiki/sources/gma-air-c4c-digital-implement-20191204.md`
- `wiki/sources/gma-medium-voltage-primary-gas-insulated-switchgear-v1-5.md`
- `wiki/sources/gma-nrjed311328en-1017.md`
- `wiki/sources/hvx-manual.md`
- `wiki/sources/mvnex-medium-voltage-metal-clad-switchgear.md`
- `wiki/sources/pix-50ka-catalogue-en.md`
- `wiki/sources/pix-catalogue-indoor-ac-metal-enclosed-switchgear.md`
- `wiki/sources/pix-indoor-ac-metal-enclosed-switchgear-v8-breaker-parameter-revision.md`
- `wiki/sources/pix500-catalogue-armored-metal-enclosed-switchgear.md`
- `wiki/sources/pix550-catalogue.md`
- `wiki/sources/pmb-easy-johnson-v1.md`
- `wiki/sources/smart-hvx-product-introduction-v3-4.md`
- `wiki/sources/smart-hvx-product-pmb-introduction.md`
- `wiki/sources/wig-high-speed-rail-smart-switchgear-jiaoda-yunda-protection-pasific-window.md`

These are currently treated as low severity because source pages are discoverable through `wiki/index.md`, `wiki/log.md`, and frontmatter `sources:` fields, even when no page body links back to them.

### Broken Wikilinks

No broken wikilinks found.

### Missing Entity Pages

No entity-like wikilinks were found 3 or more times without a corresponding page.

### Sparse Pages

No pages have fewer than 2 outbound wikilinks.

## Graph-Aware Issues

Graph-aware checks were skipped because `graph/graph.json` is not present.

Suggested next step: run `build graph` or `tools/build_graph.py` when graph-level checks are needed.

## Semantic Review

### Contradictions / Version Differences

- `Smart HVX` reliability wording remains the main promotional metric inconsistency: most sources say reliability is improved by 1x, while `Smart HVX 产品介绍 V3.4` also says reliability is 50% higher. This is already marked in `overview.md`, `SmartHVX.md`, and the related source page.
- `BLink` peak-current wording differs between GHA sources: the older PPT states 104kA peak current, while the 2018 GHA catalog states 100kA peak current. The catalog should be preferred for general ratings, but project/order documents should be checked before engineering use.
- `WIG` uses `IEC61580` in system-diagram protocol labels while the narrative and industry context point to IEC 61850. Treat this as a likely typo until checked against original engineering drawings or device communication lists.
- `GMA` and `PIX` parameter differences appear to be version/market/application-scope differences rather than confirmed contradictions. Examples include GMA Chinese 2023 vs English 2017 current ranges, and PIX English high-performance catalog vs Chinese broader family catalogs.

### Stale Content

- No stale entity or concept page was found that directly conflicts with a newer source.
- GHA pages were recently updated to prefer the 2018 formal catalog for general ratings while preserving older PPT-only notes such as `ILIS`.

### Data Gaps & Suggested Sources

- Smart HVX promotional metrics need source evidence: reliability-improvement baseline, maintenance-efficiency calculation boundary, and cost-reduction assumptions.
- GHA B-link 100kA vs 104kA should be verified with a more specific technical manual, type-test certificate, or ordering document.
- WIG IEC61580 vs IEC 61850 should be checked against original project drawings, communication protocol lists, or equipment manuals.
- Full GHA engineering selection still needs project-specific configuration data for cable connector combinations, room planning, and local standard variants.

### Concepts Needing More Depth

- `IVIS` is newly created and adequate for catalog-level description, but would benefit from an operating/manual source if voltage testing workflow becomes important.
- `ILIS` currently depends on the older GHA PPT only; if later GHA documents omit the name, the wiki should decide whether to keep `ILIS` as a legacy/option term or merge its content into broader arc-fault mitigation.

## Summary

The wiki is structurally healthy: no broken links, no missing entity pages, no sparse pages, and all source pages are indexed and logged. The remaining work is mostly semantic governance: preserve known version differences, verify promotional claims, and build the graph when graph-aware lint is needed.
