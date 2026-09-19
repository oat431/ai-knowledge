---
title: "Core Machine Learning"
note_type: pillar-overview
pillar: 02
tags: [ai, vault, core-ml, machine-learning, overview]
status: living
source: Understanding Deep Learning (Prince), ISLR (James et al.), Deep Learning (Goodfellow et al.)
---

# 02 Core Machine Learning

> **Positioning:** Classical + deep learning theory. The layer that explains *why* models learn. Slow churn — textbook-grounded.

## What This Pillar Covers

| Topic | File | Why it matters |
|---|---|---|
| Machine Learning (survey) | [[05_Machine_Learning]] | Classical ML overview — seed |
| Reinforcement Learning | [[06_Reinforcement_Learning]] | RLHF depends on RL; agents learn — seed |

## Planned Sub-Folders (on demand)

- `01_ML_Fundamentals/` — supervised/unsupervised, bias-variance, generalization, overfitting
- `02_Linear_and_Logistic_Regression/` — the simplest models that teach the most
- `03_Tree_Based_Models/` — decision trees, RF, GBM, XGBoost (still SOTA for tabular)
- `04_Neural_Network_Fundamentals/` — backprop, activations, optimizers, regularization
- `05_Deep_Learning_Architectures/` — CNN, RNN/Transformer, autoencoder, diffusion
- `06_Reinforcement_Learning/` — RLHF/DPO context for LLM alignment
- `07_Unsupervised_and_Generative/` — clustering, VAEs, diffusion models

## Build Strategy

Go deep only when you hit a wall in applied work. Examples:
- Can't reason about embedding quality → [[04_Neural_Network_Fundamentals]] (representations)
- Can't reason about why fine-tuning helps → [[01_ML_Fundamentals]] (generalization)
- Building a retrieval reranker → [[03_Tree_Based_Models]] (gradient boosting still wins on tabular)

## Sources

- [[10_Source_Index]]

## Related

- [[00_Vault_Overview]] — [[01_Foundations/00_overview]] — [[03_Foundation_Models_and_LLMs/00_overview]]
