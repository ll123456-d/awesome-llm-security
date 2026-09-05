# Awesome LLM Security

**[English](README.md) | [中文](README.zh-CN.md)**

A curated, re-organized collection of recent research on **LLM safety & security** — spanning white-box / mechanistic analysis of alignment, jailbreak attacks & red teaming, guardrails & defenses, code-LLM security, agent & multi-agent security, and LLM-driven offensive security.

> Organized from a Zotero reading list. Each topic has its own page with a `Year | Paper | Summary | Venue | Code` table. Papers are deduplicated across the original (overlapping) collections and assigned to the single most relevant topic.

---

## 📑 Topic Overview

| # | Topic | Focus | Page |
|---|-------|-------|------|
| 1 | **White-Box & Mechanistic Safety** | Understanding & editing safety alignment at the neuron / circuit / activation level; vulnerability detection via internal states | [`01-white-box-safety/README.md`](01-white-box-safety/README.md) |
| 2 | **Jailbreak Attacks & Red Teaming** | Attacking aligned chat LLMs: adversarial suffixes, semantic/agentic jailbreaks, automated red teaming, benchmarks | [`02-jailbreak-redteaming/README.md`](02-jailbreak-redteaming/README.md) |
| 3 | **Guardrails & Safety Defenses** | Detecting jailbreaks, hardening refusal, input/output guardrails, safety fine-tuning & unlearning defenses | [`03-guardrails-defenses/README.md`](03-guardrails-defenses/README.md) |
| 4 | **Code-LLM Security** | Malicious code generation, code jailbreaks, vibe-coding vulnerabilities, secure code generation | [`04-code-llm-security/README.md`](04-code-llm-security/README.md) |
| 5 | **Agent & Multi-Agent Security** | Prompt injection, tool poisoning, communication attacks, multi-agent red teaming & defense | [`05-agent-multiagent-security/README.md`](05-agent-multiagent-security/README.md) |
| 6 | **LLM-Driven Offensive Security** | Using LLMs/agents for pentesting, vulnerability discovery, exploit generation, malware | [`06-offensive-security/README.md`](06-offensive-security/README.md) |

---

## 🔎 Quick Stats

| Topic | # Papers |
|-------|---------|
| 1. White-Box & Mechanistic Safety | 27 |
| 2. Jailbreak Attacks & Red Teaming | 26 |
| 3. Guardrails & Safety Defenses | 6 |
| 4. Code-LLM Security | 5 |
| 5. Agent & Multi-Agent Security | 27 |
| 6. LLM-Driven Offensive Security | 7 |
| **Total (unique)** | **98** |

> **Note on boundary papers.** A few works span two topics (e.g., *GoodVibe*, *SAGE*, *CSULoRA* mix white-box mechanisms with code security / defenses). They are placed under their **primary contribution** to avoid duplication.

---

## 📚 Reading Notes Format

Each summary follows the structure:

- **Gap:** what problem / limitation motivates the work
- **Method:** the core idea / technique / knowledge used
- **Result:** main findings & numbers

Venue is reported as conference / journal / arXiv preprint (arXiv IDs included in the `Paper` column links where known).

---

## 🗂 Origin

Reorganized from the following (overlapping) Zotero collections, which mixed **topic** and **access-level** (black-box vs white-box) axes:

- `护栏` / `护栏-code` / `护栏-code白盒` / `红队` / `LLM-code白盒护栏` (under `TDSC审稿`)
