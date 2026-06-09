---
title: "RM6-S Plus"
type: entity
tags: [product, switchgear, ring-main-unit, gas-insulated, medium-voltage]
sources: [rm6-s-rm6-s-plus-medium-voltage-distribution-gas-insulated-switchgear-catalog-2018]
last_updated: 2026-06-09
---

## Summary
[[RM6SPlus]] 是 [[施耐德电气]] `RM6-S` 路线中的升级分支，定位为 `12kV` 二次配电用、`1250A` 顶部扩展的 [[气体绝缘开关柜]] / 环网柜对象。当前知识库里它主要来自一份 `2018.10` 正式目录：核心不是运维说明，而是 `CB / B / G / CBBr / M / PT` 功能体系、`1250A / 31.5kA` 进线与母联单元、顶部扩展和固体母线拼柜边界。

## Key Details
- 目录直接把 `RM6-S Plus` 定义为 `RM6-S` 的升级版：额定电流由 `630A` 提升到 `1250A`，柜间拼接由侧部扩展改为顶部扩展。
- 主功能单元写为 `CB / B / G / CBBr / M / PT`。
- `CB` 功能单元为 `1250A 31.5kA` 真空断路器进线/出线单元，额定操作顺序为 `O - 0.3s - CO - 180s - CO`。
- `B` 功能单元为 `630A 25kA` 线路与变压器保护单元，支持快速自动重合闸顺序 `O - 0.3s - CO - 180s - CO`。
- `CBBr` 功能单元为 `1250A` 断路器母联方案，三工位隔离开关和母线提升位于同一气箱内，并可与进线柜实现机械闭锁。
- `G` 为 `1250A` 隔离柜，接地开关可选，并可与进线断路器柜闭锁，避免带负载开合隔离开关。
- `PT` 功能单元带三工位隔离开关，可位于母线任何位置，包括边柜和中间柜。
- 顶部拼柜可采用特定固体母线装置实现，不需要现场气体处理，也不需要为扩展额外预留安装空间。
- 目录把 `Sepam40` 作为 `CB` 进线柜标准配置，把 `Sepam20` 作为 `B` 出线柜标准配置。

## Related
- [[施耐德电气]]
- [[RM6]]
- [[RM6S]]
- [[气体绝缘开关柜]]
- [[ALink]]
