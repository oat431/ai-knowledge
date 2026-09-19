---
title: "AI Operations and MLOps"
note_type: pillar-overview
pillar: 05
tags: [ai, vault, mlops, operations, overview]
status: living
source: Designing Machine Learning Systems (Huyen), LLM Engineer's Handbook (Iusztin & Labonne)
---

# 05 AI Operations and MLOps

> **Positioning:** The infrastructure that runs AI in production. Medium churn — docs + benchmarks.

## What This Pillar Covers

| # | Folder | Focus |
|---|---|---|
| 01 | `01_Data_Pipelines_and_Quality/` | ETL/ELT for ML, data quality, feature stores |
| 02 | `02_Serving_Infrastructure/` | vLLM, SGLang, TensorRT-LLM, quantization (GGUF/GPTQ) |
| 03 | `03_Experiment_Tracking_and_Model_Registry/` | W&B, MLflow, DVC |
| 04 | `04_Monitoring_and_Drift/` | Model drift, data drift, quality monitoring |
| 05 | `05_CI_CD_for_AI_Systems/` | Eval gates in CI, model promotion, rollback |

## Build Strategy

Build when you're responsible for production systems. The boundary with [[career-path/07_SRE_and_Platform_Engineer/00_overview|SRE]] is: LLMOps decides serving architecture; SRE executes infra, CI/CD, deployment. Eval gates live in the pipeline SRE owns.

## Sources

- [[10_Source_Index]]

## Related

- [[README]] — [[04_Applied_AI_Engineering/00_overview]] — [[06_Governance_and_Responsible_AI/00_overview]]
