---
title: "Foundation Models and LLMs"
note_type: pillar-overview
pillar: 03
tags: [ai, vault, llm, foundation-models, overview]
status: living
source: Hands-On Large Language Models (Alammar & Grootendorst), The Illustrated Transformer (Alammar)
---

# 03 Foundation Models and LLMs

> **Positioning:** The bridge layer. What you're actually calling via API — transformers, pretraining, alignment, tokenization. Medium churn — re-verify quarterly.

## What This Pillar Covers

The engineering-relevant theory behind the models you use every day. You don't need to train one from scratch (that's research). You need to understand enough to reason about capabilities, limits, cost, and failure modes.

## Planned Sub-Folders

| # | Folder | Focus |
|---|---|---|
| 01 | `01_Transformer_Architecture/` | Attention, scaling laws, MoE, context length |
| 02 | `02_Pretraining_and_Alignment/` | Pretraining, SFT, RLHF/DPO, constitutional methods |
| 03 | `03_Tokenization_and_Representations/` | BPE, SentencePiece, embeddings |
| 04 | `04_Capabilities_and_Limits/` | What models can/can't do, reasoning, hallucination |
| 05 | `05_Open_vs_Closed_Weight_Ecosystem/` | Llama/Qwen/DeepSeek vs OpenAI/Anthropic/Google |

## Key Principle

> The applied pillar (04) assumes you understand *what a model is*. This pillar gives you that. If you skip it, your applied notes become copy-paste — you'll blame the model for failures that are actually context/retrieval problems.

## Build Order

1. [[01_Transformer_Architecture]] — start with Jay Alammar's *Illustrated Transformer*, then deepen
2. [[04_Capabilities_and_Limits]] — what current models do well/poorly (web-verify per model release)
3. [[03_Tokenization_and_Representations]] — embeddings, context windows
4. [[02_Pretraining_and_Alignment]] — RLHF, DPO, why alignment matters for safety
5. [[05_Open_vs_Closed_Weight_Ecosystem]] — routing decisions live here

## Sources

- [[10_Source_Index]]

## Related

- [[README]] — [[02_Core_Machine_Learning/00_overview]] — [[04_Applied_AI_Engineering/00_overview]]
