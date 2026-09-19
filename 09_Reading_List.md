---
title: "AI Engineering Vault — Reading List"
note_type: reading-list
tags: [ai, vault, reading-list, sources, evergreen]
status: living
---

# AI Engineering Vault — Reading List

> Canonical sources to build this vault from. Tiered by priority. Full annotated version: `oralita_md/personal/ai/ai-engineering-reading-list.md`.
> Sources web-verified 2026-09-19.

## Tier 0 — Anchor Books (start here)

- **AI Engineering: Building Applications with Foundation Models** — Chip Huyen (O'Reilly, 2025) → pillars 04, 05, 06
- **Hands-On Large Language Models** — Jay Alammar & Maarten Grootendorst (O'Reilly) → pillars 03, 04
- **Designing Machine Learning Systems** — Chip Huyen (O'Reilly) → pillar 05
- **Build a Large Language Model (From Scratch)** — Sebastian Raschka → pillar 03 (deep)
- **LLM Engineer's Handbook** — Paul Iusztin & Maxime Labonne → pillars 04, 05
- **Prompt Engineering for Generative AI** — James Phoenix & Mike Taylor (O'Reilly) → pillar 04/02

**Minimum viable set:** Chip Huyen *AI Engineering* + Jay Alammar *Hands-On LLMs*. Seeds 70% of the applied vault.

## Tier 1 — Foundations & Core ML (slow churn)

- **Mathematics for Machine Learning** — Deisenroth, Faisal, Ong (Cambridge, free: mml-book.github.io) → pillar 01
- **Understanding Deep Learning** — Simon Prince (MIT Press, 2024) → pillar 02
- **Deep Learning** — Goodfellow, Bengio, Courville (MIT Press) → pillar 02 (reference)
- **Pattern Recognition and Machine Learning** — Christopher Bishop → pillar 02 (theory)
- **An Introduction to Statistical Learning (ISLR)** — James, Witten, Hastie, Tibshirani (free PDF) → pillar 02

## Tier 2 — Foundation Models & LLMs (medium churn)

- **The Illustrated Transformer** — Jay Alammar (blog) → pillar 03
- **LLM Course** — Maxime Labonne (free, GitHub) → pillars 03, 04
- **Hugging Face NLP Course** (free) → pillar 03
- **OpenAI / Anthropic / Google model docs** (official) → pillars 03, 04
- **Sebastian Raschka's magazine** (Substack) → pillars 03, 06
- **arXiv** (cs.CL, cs.LG, cs.AI) → pillar 03

## Tier 3 — Applied AI (fast churn — web-verify per citation)

- **OWASP Top 10 for LLM Applications (2025)** → pillar 04/04
- **Anthropic: Building Effective Agents** (engineering blog) → pillars 04/01, 04/07
- **Karpathy on Context Engineering** (X/posts) → pillar 04/02
- **promptfoo / DeepEval / Inspect / LangSmith / Braintrust** docs → pillar 04/03
- **Chip Huyen's blog** (chiphuyen.com) → pillars 04, 05
- **Eugene Yan's blog** (eugeneyan.com) → pillars 04, 05
- **Hamel Husain's blog** → pillar 04/03

## Tier 4 — AI Ops & MLOps

- **Designing ML Systems** — Chip Huyen → pillar 05 (also Tier 0)
- **LLM Engineer's Handbook** — Iusztin & Labonne → pillar 05 (also Tier 0)
- **vLLM / SGLang / TensorRT-LLM docs** → pillar 05/02
- **W&B / MLflow / DVC docs** → pillar 05/03
- **Google SRE Book** → pillar 05/04

## Tier 5 — Governance

- **NIST AI Risk Management Framework (AI RMF)** → pillar 06/01
- **ISO/IEC 42001:2023** → pillar 06/01
- **EU AI Act** → pillar 06/04
- **Model Cards for Model Reporting** — Mitchell et al. (paper) → pillar 06/03
- **Co-Intelligence** — Ethan Mollick → pillar 06 (stakeholder comms)

## Tier 6 — Specialized (on demand)

- **Speech and Language Processing** — Jurafsky & Martin (free online) → pillar 07/01
- **Deep Learning for Computer Vision** — PyImageSearch → pillar 07/02
- **AudioCraft/MusicGen + ESPnet docs** → pillar 07/03
- **LLaVA + CLIP papers** → pillar 07/04

## Reading Order (applied-first, recommended)

```
Tier 0: AI Engineering (Huyen) → Hands-On LLMs (Alammar)
   ↓  build pillar 04
Tier 3: OWASP LLM Top 10 → Anthropic agents → Hamel Husain evals
   ↓  ship safely
Tier 0: Designing ML Systems → LLM Engineer's Handbook
   ↓  operate it (pillar 05)
Tier 2: Illustrated Transformer → HF NLP → Labonne course
   ↓  understand bridge layer (pillar 03)
Tier 1: ISLR → MML book (selective) → Understanding DL (selective)
   ↓  foundations on demand
Tier 5: NIST AI RMF → EU AI Act → model cards
   ↓  govern (pillar 06)
Tier 7: your own ADRs, evals, postmortems — ongoing
```

## Related

- [[10_Source_Index]] — verification log
- [[00_Vault_Overview]]
