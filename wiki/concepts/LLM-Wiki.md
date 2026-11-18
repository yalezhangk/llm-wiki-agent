---
title: "LLM-Wiki"
type: concept
tags: [knowledge-base, llm, wiki, traceability]
sources: [llm-wiki-traceable-medium-voltage-knowledge-base]
last_updated: 2026-11-18
---
## Summary
[[LLM-Wiki]] 是一种结合大语言模型（LLM）与 Wiki 结构的知识库构建方法。它旨在解决专业领域资料分散、答案与出处难以关联的问题。通过自动化流程将原始资料（如产品样本、说明书）转化为结构化的 Source、实体和概念页面，并在问答时提供带有引用溯源的回答，确保知识可浏览、可提问、可追溯。该方法参考了 Andrej Karpathy 的 LLM Wiki 构想及 SamurAIGPT/llm-wiki-agent 开源项目。

## Key Details
- **核心流程**：原始资料 → 结构化 Wiki（Source/实体/概念） → 问答与浏览。
- **追溯机制**：回答中的引用可链接至 Source 知识页，进而链接至原始文件（如 PDF），实现三级追溯。
- **适用场景**：适用于产品学习、方案比较、资料导航等场景，但关键参数和标准条款仍需核对原文。
- **系统组成**：通常包括 `llm-wiki-agent`（知识内容）、`wiki-backend`（服务编排）和 `quartz`（网站呈现）等组件。

## Related
- [[HVX]]
- [[真空灭弧室]]