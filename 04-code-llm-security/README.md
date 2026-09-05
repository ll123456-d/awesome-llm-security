# 4. Code-LLM Security

*Attacks on code generation / coding agents (malicious code jailbreaks, prompt fragility) and measurement of insecure code from coding assistants ("vibe coding").*

| Year | Paper | Summary | Venue | Code |
|------|-------|---------|-------|------|
| 2025 | **Casting a SPELL: Sentence Pairing Exploration for LLM Limitation-breaking** ([arXiv](https://arxiv.org/abs/2512.21236)) | **Gap:** Jailbreak research targets general LLMs; malicious *code generation* as a jailbreak target is underexplored.<br>**Method:** SPELL — testing framework with time-division selection combining sentences from a prior-knowledge dataset (explore novel / exploit successful attack patterns).<br>**Result:** ASR 83.75% (GPT-4.1), 19.38% (Claude-3.5), 68.12% (Qwen2.5-Coder) across 8 malicious-code categories; outputs confirmed malicious by SOTA detectors >73% of the time. | arXiv | – |
| 2026 | **Grammar-Constrained Decoding Can Jailbreak LLMs into Generating Malicious Code (CodeSpear)** ([arXiv](https://arxiv.org/abs/2606.11817)) | **Gap:** Grammar-constrained decoding (GCD) is assumed safe (it enforces syntactic validity); its security risk is unstudied.<br>**Method:** Show a *benign* code grammar constraint can itself jailbreak LLMs into emitting malicious code.<br>**Result:** GCD is a counterintuitive, new attack surface for malicious code generation. | arXiv | – |
| 2026 | **MultiCodeAttack: Iterative Jailbreak with Multi-Code Prompt Injection** | **Gap:** Structured code-template jailbreaks are fixed-template, single-language; cross-language & adaptive evolution unexplored.<br>**Method:** Maintain a multi-language template library; select effective languages via multi-armed bandit; evolve templates with semantic-preserving, response-aware mutation.<br>**Result:** Beats baselines by 28.23%–832.59% on harmful text and up to 136.22% more malicious code outputs across 8–11 LLMs. | (journal) | [anonymous](https://anonymous.4open.science/r/MultiCodeAttack/) |
| 2026 | **Is Vibe Coding Safe? Benchmarking Vulnerability of Agent-Generated Code (SUSVIBES)** ([arXiv](https://arxiv.org/abs/2512.03262)) | **Gap:** Vibe coding (low-supervision agent coding) is increasingly deployed, but is its code safe?<br>**Method:** Benchmark of 186 real-world feature-request tasks where humans committed vulnerable implementations; evaluate 12 coding-agent settings with frontier models.<br>**Result:** Agents perform poorly on security: e.g. SWE-Agent+Claude 4 Sonnet is 57% functionally correct but only 11.8% secure; vuln hints don't fix it. | arXiv | [github](https://github.com/LeiLiLab/susvibes) |
| 2026 | **Minimal Prompt Perturbations Lead to Code Vulnerabilities (Prompt Fragility)** ([arXiv](https://arxiv.org/abs/2605.29737)) | **Gap:** Prior work shows prompt mutations break functional correctness; whether they also break *security* was unstudied.<br>**Method:** Token-level prompt mutations across 3 models × 5 languages; probe hidden states for pre-generation predictability.<br>**Result:** A single-character change can flip secure→vulnerable code; input-handling flaws are more predictable (AUC 0.753) than secure-defaults flaws (AUC 0.674) → first class detectable pre-generation, second needs decoding-time intervention. | arXiv | – |

---
*[Back to index](../README.md)*

---
*[Back to index](../README.md)*
