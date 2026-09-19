---
title: "Applied AI Engineering"
note_type: pillar-overview
pillar: 04
tags: [ai, vault, applied-ai, engineering, overview]
status: living
source: AI Engineering (Huyen), OWASP Top 10 for LLM Applications (2025)
---

# 04 Applied AI Engineering

> **Positioning:** THE applied layer. What you do every day as an AI engineer — RAG, agents, evals, guardrails, context engineering. **Fast churn — web-verify before citing in any ADR.**

## What This Pillar Covers

Eight sub-areas. The first six mirror the capability areas in the [[career-path/18_Applied_AI_Engineer/00_overview|Applied AI Engineer career path]] (role view); the last two (`06_Fine_Tuning_Strategy`, `07_Multi_Agent_and_Orchestration`) are added depth the career-path notes don't cover.

| # | Sub-area | Focus |
|---|---|---|
| 01 | [[01_LLM_Application_Patterns/00_overview\|LLM Application Patterns]] | RAG, tool use, agents, structured outputs, context injection, pattern selection |
| 02 | [[02_Context_and_Prompt_Engineering/00_overview\|Context & Prompt Engineering]] | Context engineering (superseded prompt engineering), templates, versioning |
| 03 | [[03_Evaluation_and_Observability/00_overview\|Evaluation & Observability]] | Eval suites, LLM-as-judge, regression gates, tracing, trajectory eval |
| 04 | [[04_AI_Security_and_Guardrails/00_overview\|AI Security & Guardrails]] | Prompt injection, OWASP LLM Top 10, data leakage, blast radius |
| 05 | [[05_Model_and_Inference_Operations/00_overview\|Model & Inference Operations]] | Routing, cascading, caching, cost/latency, self-hosting |
| 06 | [[06_Fine_Tuning_Strategy/00_overview\|Fine-Tuning Strategy]] | When (rarely) it's worth it; SFT vs LoRA vs RAG-first |
| 07 | [[07_Multi_Agent_and_Orchestration/00_overview\|Multi-Agent & Orchestration]] | Bounded agents, trajectory eval, vertical agents |

## Seed Files (copied from swe-knowledge)

Three broad LLM-era notes already live at this pillar's root:
- [[10_LLM_Production_Patterns]] — maps to sub-area 01
- [[11_Prompt_Engineering_and_Security]] — spans sub-areas 02 + 04
- [[13_LLM_Evaluation_and_Guardrails]] — spans sub-areas 03 + 04

These are surveys. Deepen them into the sub-area folders as you read.

## Key Principle (the honest one)

> **Q4 2026's applied AI is less about "make the model smarter" and more about engineering *around* the model's probabilistic nature:** curate its context, gate its output with evals, scope its autonomy, route it cheaply, enforce its structure, and defend against its misuse.

This is the layer where my 8 core principles bite hardest:
1. Demo quality ≠ production quality
2. Evaluation is a first-class engineering practice
3. The simplest solution that works wins
4. Models are probabilistic components — engineer around that
5. Cost and latency are features
6. Defense in depth against AI-specific threats
7. Teach the trade-offs, not the hype
8. The vault is the curriculum; the web is the changelog

## Quality Gate

Before any applied pattern ships from this pillar into production:
- [ ] ADR exists for the pattern choice (including "why not simpler/no-AI")
- [ ] Eval suite with baseline; regression gate in CI
- [ ] Failure modes designed: timeouts, malformed output, hallucination, fallbacks
- [ ] Guardrails: input/output filtering, injection defenses, least-privilege tools
- [ ] Cost & latency budget documented and monitored
- [ ] Data handling reviewed: leakage, privacy, retention
- [ ] "What happens when the model is wrong?" answered explicitly

## Sources

- [[10_Source_Index]]
- Full reading list: `oralita_md/personal/ai/ai-engineering-reading-list.md` — Tiers 0 + 3

## Related

- [[00_Vault_Overview]] — [[03_Foundation_Models_and_LLMs/00_overview]] — [[05_AI_Operations_and_MLOps/00_overview]] — [[08_Practitioner_Notes/00_overview]]
