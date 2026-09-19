---
title: "Context and Prompt Engineering"
note_type: sub-area-overview
pillar: 04
sub_area: 02
tags: [ai, applied-ai, context-engineering, prompt-engineering, overview]
status: living
source: Prompt Engineering for Generative AI (Phoenix & Taylor), Karpathy on Context Engineering
---

# 04.02 Context and Prompt Engineering

> **Positioning:** Managing the *entire informational environment* the model sees — not just phrasing the instruction nicely. "Context engineering" superseded "prompt engineering" as the dominant frame in 2026 (Karpathy).

## Why This Matters

The prompt is the *least* of your problems. The hard engineering is **what is in the context window and how it's curated**: RAG retrieval quality, context-window budgeting, tool-result compression, conversation memory.

> **The model's ceiling is set by what it can see, not how you ask.**

## Topics (planned)

| # | Topic | Focus |
|---|---|---|
| 01 | `01_Prompt_Design_Principles.md` | System/user message design, instruction hierarchy |
| 02 | `02_Context_Window_Management.md` | Budgeting, trimming, compression, token economics |
| 03 | `03_Dynamic_Context_Assembly.md` | Composing retrieved docs + tool results + history |
| 04 | `04_Prompt_Templates_and_Versioning.md` | Templating, version control for prompts |
| 05 | `05_Few_Shot_and_Chain_of_Thought.md` | When examples help, when CoT helps, when they don't |
| 06 | `06_Context_vs_Prompt_Engineering.md` | The paradigm shift — what changed in 2026 |

## Key Principles

- Stop optimizing wording; start curating context
- Context window is a budget — every token has a cost (latency + $)
- Tool results that persist across turns must be compressed, not re-fetched
- Few-shot helps calibration; CoT helps reasoning; both can hurt if misapplied
- Prompt templates are code — version them, test them, review them

## Thai Speaker Traps

⚠️ "Context engineering" ไม่ใช่แค่การเขียน prompt ให้สวย — หมายถึงการคัดสรรสิ่งที่ใส่เข้า context window ทั้งหมด
⚠️ "Alignment" (in ML context) ≠ การจัดตำแหน่ง = การทำให้โมเดลเชื่อฟัง/ปลอดภัย (see [[03_Foundation_Models_and_LLMs/00_overview]])

## Seed File

- [[11_Prompt_Engineering_and_Security]] — broad survey (copied from swe-knowledge)

## Sources

- [[10_Source_Index]]

## Related

- [[04_Applied_AI_Engineering/00_overview]] — [[01_LLM_Application_Patterns/00_overview]] — [[03_Evaluation_and_Observability/00_overview]]
