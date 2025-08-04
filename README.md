# Wekeza Dataset: InstructZero v6

A high-quality instruction–response dataset for **Kenyan financial reasoning** generated via *self-instruct* and filtered using an **InstructZero-style validation** pipeline powered by a LoRA-finetuned DistilGPT2 model (`distilgpt2-wekeza-finetuned_v4_lora`).

This is part of the broader [Wekeza LLM](https://github.com/brianbollo/wekeza-llm) initiative to build trustworthy domain-specific assistants for the Kenyan investment ecosystem.

---

## 📁 File

- `kenyan_finance_selfinstruct_v6_instructzero.jsonl`  
  Final dataset with **consistency-verified** instruction–response pairs.

---

## 🔍 Dataset Overview

- ✅ Instructions were *auto-generated* via Self-Instruct + CoT
- 🤖 Each instruction was rewritten into 2–3 semantically equivalent variants
- 🧠 The model generated responses for all variants
- 🧮 Instructions with **inconsistent** outputs across rewrites were **discarded**
- 🧼 Only stable, reliable instruction–response pairs were retained

---

## 📊 Example Entry

```json
{
  "instruction": "Explain the differences between a money market fund and a fixed deposit in Kenya.",
  "response": "A money market fund is a pooled investment that provides daily liquidity and invests in short-term securities. A fixed deposit locks in funds for a set period with a fixed interest rate. MMFs are more flexible, while fixed deposits offer slightly higher returns but less accessibility."
}
