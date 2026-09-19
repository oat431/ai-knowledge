---
title: "Practitioner Notes"
note_type: pillar-overview
pillar: 08
tags: [ai, vault, practitioner, adr, evals, postmortems, overview]
status: living
---

# 08 Practitioner Notes

> **Positioning:** YOUR working knowledge. First-hand case studies, ADRs, eval results, postmortems. No external source — only your real systems.

## What This Pillar Covers

| # | Folder | Focus |
|---|---|---|
| 01 | `01_ADRs/` | Architecture decision records for every consequential AI choice |
| 02 | `02_Eval_Suites/` | Actual eval designs with golden sets + results |
| 03 | `03_Postmortems/` | Production model failures, abuse incidents, cost overruns |
| 04 | `04_Tooling_Reviews/` | Current-state reviews of frameworks, re-verified before citing |

## The Rule

> A practitioner note is only trustworthy if it has a real system behind it. Don't write "how to build a RAG system" as a practitioner note until you've *built and shipped one*. Use pillars 01–07 for theory; use pillar 08 for war stories.

## ADR Template

Use the ADR template from `swe-knowledge/document-template/`. Every consequential AI decision (pattern, model, provider, fine-tune) gets a decision record with:
- Context
- Decision
- Alternatives considered + why rejected
- Consequences (cost, latency, failure modes)
- Eval evidence

## Sources

- First-hand only. Cross-link to pillars 01–07 for the theory behind each decision.

## Related

- [[README]] — [[04_Applied_AI_Engineering/00_overview]]
