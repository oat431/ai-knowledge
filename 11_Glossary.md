---
title: "AI Engineering Vault — Glossary"
note_type: glossary
tags: [ai, vault, glossary, terms, evergreen]
status: living
---

# AI Engineering Vault — Glossary

> Key terms with cross-links to topic notes. Thai Speaker Traps flagged where Thai speakers commonly misuse the English term.

## A

- **Alignment** — Making a model follow intended behavior + be safe (RLHF, DPO, constitutional). ⚠️ Thai trap: ≠ การจัดตำแหน่ง (positioning) = การทำให้โมเดลเชื่อฟัก/ปลอดภัย. See [[03_Foundation_Models_and_LLMs/00_overview]].
- **Agent Loop** — Plan → Act → Observe cycle, bounded by iteration/token/time limits. See [[04_Applied_AI_Engineering/01_LLM_Application_Patterns/00_overview]].
- **Attention** — The mechanism behind transformers; lets the model weigh different parts of input. See [[03_Foundation_Models_and_LLMs/00_overview]].

## B

- **Blast Radius** — The scope of damage a model/agent can cause if it misbehaves. Minimized by least-privilege tools. See [[04_Applied_AI_Engineering/04_AI_Security_and_Guardrails/00_overview]].
- **Bounded Agent** — An agent scoped to one job, one domain, with least-privilege tools. The 2026 winner over "general agents." See [[04_Applied_AI_Engineering/07_Multi_Agent_and_Orchestration/00_overview]].

## C

- **Context Engineering** — Managing the entire informational environment the model sees (superseded "prompt engineering" in 2026, per Karpathy). ⚠️ Thai trap: ≠ แค่เขียน prompt ให้สวย = การคัดสรรสิ่งที่ใส่เข้า context window. See [[04_Applied_AI_Engineering/02_Context_and_Prompt_Engineering/00_overview]].
- **Context Window** — The token budget a model can process in one call. Economics: every token costs latency + $.

## E

- **Eval-Driven Development (EDD)** — Treating evals as the unit tests of LLM software; CI regression gates block merges. See [[04_Applied_AI_Engineering/03_Evaluation_and_Observability/00_overview]].
- **Embedding** — A vector representation of text/image; enables similarity search. RAG depends on this.

## F

- **Foundation Model** — A large pretrained model consumed via API or open weights; the applied engineer's building block. See [[03_Foundation_Models_and_LLMs/00_overview]].
- **Fine-Tuning** — Adapting a pretrained model with task-specific data. ⚠️ Rarely worth it — RAG + prompting + routing beats it for ~90% of needs. See [[04_Applied_AI_Engineering/06_Fine_Tuning_Strategy/00_overview]].
- **Function Calling** — A structured channel: the model "calls a tool" whose parameters are your target schema. More reliable than JSON mode. See [[04_Applied_AI_Engineering/01_LLM_Application_Patterns/00_overview]].

## G

- **Guardrails** — Input/output filters + fallback logic layered around the model. See [[04_Applied_AI_Engineering/04_AI_Security_and_Guardrails/00_overview]].

## I

- **Inference** — Running a model to produce output. ⚠️ Thai trap: ≠ การอนุมานเชิงตรรกะ (logical inference) = การรันโมเดลเพื่อได้ผลลัพธ์. See [[04_Applied_AI_Engineering/05_Model_and_Inference_Operations/00_overview]].
- **Injection (Prompt)** — An unsolved attack class: hostile input manipulates the model. See [[04_Applied_AI_Engineering/04_AI_Security_and_Guardrails/00_overview]].

## L

- **LLM-as-Judge** — Using an LLM to grade another LLM's output. Has biases; calibrate against human labels. See [[04_Applied_AI_Engineering/03_Evaluation_and_Observability/00_overview]].
- **LoRA / QLoRA** — Parameter-efficient fine-tuning (cheaper, reversible). Usually the right method when fine-tuning is justified at all.

## M

- **Model Routing** — Directing queries to the right model by complexity + risk. Static single-model deployment is the anti-pattern. See [[04_Applied_AI_Engineering/05_Model_and_Inference_Operations/00_overview]].

## P

- **Prompt Injection** — see Injection.
- **Prompt Engineering** — (Legacy term) phrasing instructions well. Superseded by context engineering in 2026.

## R

- **RAG (Retrieval-Augmented Generation)** — Retrieve relevant docs → inject into context → generate. Retrieval quality determines generation quality. See [[04_Applied_AI_Engineering/01_LLM_Application_Patterns/00_overview]].
- **RLHF** — Reinforcement Learning from Human Feedback. The dominant alignment method. See [[03_Foundation_Models_and_LLMs/00_overview]].
- **Regression Gate** — A CI check that blocks merges when eval quality drops below baseline. See [[04_Applied_AI_Engineering/03_Evaluation_and_Observability/00_overview]].

## S

- **Structured Outputs** — Machine-verifiable model output enforced by schema (JSON mode or function calling). The norm; free text must justify itself. See [[04_Applied_AI_Engineering/01_LLM_Application_Patterns/00_overview]].

## T

- **Token** — The unit a model processes; roughly ¾ of a word for English. Costs latency + $ per token.
- **Tokenization** — Splitting text into tokens (BPE, SentencePiece). See [[03_Foundation_Models_and_LLMs/00_overview]].
- **Trajectory Evaluation** — Evaluating every step of an agent run, not just the final answer. Filter by `failed agent → trajectory → step`. See [[04_Applied_AI_Engineering/03_Evaluation_and_Observability/00_overview]].
- **Transformer** — The architecture behind modern LLMs (attention-based). See [[03_Foundation_Models_and_LLMs/00_overview]].

## V

- **Vertical AI Agent** — A bounded agent for one job in one industry (score the lead, review the prior-auth). See [[04_Applied_AI_Engineering/07_Multi_Agent_and_Orchestration/00_overview]].

## Related

- [[00_Vault_Overview]]
