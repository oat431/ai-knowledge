---
title: "Foundations"
note_type: pillar-overview
pillar: 01
tags: [ai, vault, foundations, math, statistics, overview]
status: living
source: Mathematics for Machine Learning (Deisenroth et al.), Understanding Deep Learning (Prince)
---

# 01 Foundations

> **Positioning:** The math, statistics, optimization, and computing fundamentals that ML/AI sits on. The slowest-churning layer — textbook-grounded, safe to cite from memory.

## What This Pillar Covers

The math you actually need as an AI engineer: not 4 semesters of pure math, but the specific tools that come up when you debug a model, read a paper, or reason about why something works. Built **on demand** — deepen only the topics you hit walls on in applied work.

| Topic | File | Why it matters |
|---|---|---|
| AI Foundations (survey) | [[AI Overview]] | Bird's-eye view of the whole field — copied seed |
| Classical AI foundations | [[01_AI_Foundations]] | Search, reasoning, the pre-ML AI — seed |
| Search & CSP | [[02_Search_and_CSP]] | Constraint satisfaction still appears in planning agents — seed |
| Logic & reasoning | [[03_Logic_and_Reasoning]] | Symbolic reasoning background — seed |
| Uncertainty & decisions | [[04_Uncertainty_and_Decisions]] | Probability theory, Bayesian reasoning — seed |

## Build Strategy

**Shallow first, deepen on demand (per your D3 decision).** Each seed file starts as a concept survey. When an applied problem forces you to actually understand the math (e.g., you can't reason about embedding similarity → go to linear algebra), deepen that topic with worked examples.

> ⚠️ **Anti-pattern:** front-loading all of math before touching an API. You'll forget it without application.

## Planned Sub-Folders (on demand)

- `01_Mathematics/` — linear algebra (vectors, matrices, eigendecomposition, SVD), calculus for ML
- `02_Statistics_and_Probability/` — distributions, Bayesian thinking, sampling
- `03_Optimization/` — gradient descent, convex optimization, SGD variants
- `04_Computing_for_ML/` — tensors, autodiff, GPU memory, data structures

## Sources

- [[10_Source_Index]] — full source list with verification dates

## Related

- [[README]] — vault map
- [[02_Core_Machine_Learning/00_overview]] — what foundations enable
- `oralita_md/personal/ai/ai-engineering-reading-list.md` — Tier 1 sources
