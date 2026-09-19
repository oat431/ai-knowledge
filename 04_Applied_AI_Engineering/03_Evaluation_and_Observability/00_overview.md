---
title: "Evaluation and Observability"
note_type: sub-area-overview
pillar: 04
sub_area: 03
tags: [ai, applied-ai, evaluation, observability, eval-driven-development, overview]
status: living
source: Hamel Husain (LLM evals), DeepEval docs, Chip Huyen AI Engineering
---

# 04.03 Evaluation and Observability

> **Positioning:** Evaluation is a first-class engineering practice. Evals are the unit tests of LLM software. No AI feature merges without eval results against a baseline.

## Why This Matters

Three reasons eval-driven development (EDD) became consensus in 2026:
1. LLM outputs are probabilistic — you cannot eyeball regressions the way you do with deterministic code
2. EDD makes regressions **loud at PR time** instead of silent in production
3. The eval suite becomes the **institutional memory** of what "good" looks like

> **The eval suite *is* the deliverable — the code is secondary.**

## Topics (planned)

| # | Topic | Focus |
|---|---|---|
| 01 | `01_Evaluation_Fundamentals.md` | What to eval, golden datasets, held-out sets |
| 02 | `02_Offline_Eval_Suites.md` | Building eval sets, CI integration, regression gates |
| 03 | `03_Metrics_for_LLM_Outputs.md` | Faithfulness, relevance, groundedness, custom rubrics |
| 04 | `04_LLM_as_Judge.md` | Using LLMs to grade LLMs — biases, calibration, cost |
| 05 | `05_Trajectory_Evaluation.md` | Agent traces: every step, every tool call, cohort analysis |
| 06 | `06_Tracing_and_Observability.md` | OpenTelemetry for LLM, LangSmith, Braintrust, dashboards |
| 07 | `07_Online_Evaluation_and_Monitoring.md` | Prod monitoring, drift detection, feedback loops |
| 08 | `08_Regression_Gates.md` | CI gates that block merges on quality drop |

## Key Principles

- No AI feature ships without an eval suite + baseline
- Regression gates block merges — treat eval failures like test failures
- Trajectory eval for agents: filter by `failed agent → trajectory → step`, compare against golden trajectories
- LLM-as-judge has biases — calibrate against human labels, don't trust blindly
- Tracing is non-negotiable: if you can't see every model call + tool call, you're flying blind

## Anti-Patterns

| Anti-pattern | Why it fails |
|---|---|
| "It works on my examples" | Anecdote ≠ evidence; 5 examples prove nothing |
| Eyeballing outputs for regression | You miss subtle quality drops |
| End-to-end pass/fail only | Can't diagnose *where* the agent failed |
| LLM-as-judge without calibration | Judge model has its own biases |

## Tooling (web-verify before citing)

- **promptfoo** — CLI eval runner, good for prompt comparison
- **DeepEval** — Python eval framework, LLM-as-judge built in
- **Inspect** — UK AISI framework, strong for safety/agent evals
- **LangSmith** — LangChain ecosystem tracing + eval
- **Braintrust** — eval + experiment tracking
> All re-verify current state before recommending — fast-churn tools.

## Seed File

- [[13_LLM_Evaluation_and_Guardrails]] — broad survey (copied from swe-knowledge)

## Sources

- [[10_Source_Index]]

## Related

- [[04_Applied_AI_Engineering/00_overview]] — [[07_Multi_Agent_and_Orchestration/00_overview]] (trajectory eval)
