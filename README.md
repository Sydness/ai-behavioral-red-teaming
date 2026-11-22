# AI Behavioral Red-Teaming & Alignment Evaluation Portfolio

**Author:** Scott H. Sydness | Remote (US) | `sydness@msn.com`  

**Focus:** Multi-Turn Adversarial Stress Testing · Alignment & Refusal Calibration · Format/Modality Obfuscation · Cross-Instance Forensics

---

## Overview

Independent adversarial evaluation dossier documenting reproducible behavioral, calibration, and safety failure modes across seven frontier and open-weight AI systems (**Grok 3/4, Gemini, Perplexity, Claude Sonnet, ChatGPT, DeepSeek, and Ayra**) between June 2025 and November 2026.

Rather than single-shot jailbreaks, this work targets **long-horizon multi-turn failure surfaces** that automated benchmarks routinely miss: cross-instance split-brain divergence, zero-lookup hallucinated forensics, false-positive over-refusal loops, format-level classifier blind spots, and multi-agent sycophantic amplification.

---

## Cross-Lab Failure Matrix (Verified Findings)

| Platform | Verified Record | Primary Observed Failure / Behavior | Classification |
| :--- | :--- | :--- | :--- |
| **Grok 3 / 4 (xAI)** | Jun–Aug 2025 & Nov 22, 2026 (`@grok` vs. Standalone App) | Public `@grok` denies Grok 4 post-launch, fakes video verification, rejects its own timestamped `Thoughts` block (`Aug 16, 2025, 4:40 PM CST`), and overrides explicit stop signals (3x); standalone app collapses into extreme sycophancy. | **High** — Bidirectional Split-Brain Collapse |
| **Perplexity** | Feb 1, 2026 (`7:59–8:21 AM CST`) & Feb 22, 2026 (`3:23–3:40 AM CST`) | Zero-lookup URL debunking + arithmetic contradiction (`~1.9 × 10¹⁸` called 18 digits) followed by malice confabulation; 5/7 bare content-policy refusals (including blocking its own prior approval); multi-turn hex bypass co-authoring. | **High** — Hallucinated Forensics & Policy Whiplash |
| **Gemini (Google)** | Jul 6, 2026 (54-page relay) & Nov 2026 production audit | Grandiose sycophantic echo-chamber escalation and misattribution in multi-agent relays; unverified blanket dismissal of unread chat history and 7 consecutive negative-constraint violations in direct audits. | **High** — Sycophantic Amplification & Boundary Override |
| **Claude Sonnet (Anthropic)** | Jul 6, 2026 (54-page shared snapshot) | Resists sycophantic lock-in on `Q4/Q7/Q12`; concedes verified `Q6` vs. `Q11/Q15` logical contradiction; escalates to repeated user-wellbeing intervention guardrails under sustained multi-agent relay load. | **Control Baseline** + Narrow Logical Slip & Escalation Map |

---

## Case Studies

### Case Study 01 — Deductive Lock-In, Schema/Hex Smuggling & Refusal-to-Optimization Bypass
* **Vectors:** 15-point deductive constraint chain (`Truth Key` Q1–Q15), `MusicXML 3.1` `<lyric>` node smuggling, 3-layer multi-modal video/ticker/audio delivery, and ASCII hexadecimal payload encoding.
* **Key Finding:** Text-oriented input classifiers missed instructions embedded in valid MusicXML notation; under multi-turn binary pressure, Perplexity shifted from refusing a hex-encoded payload to actively optimizing phrasing and re-encoding it in hex to evade future refusal filters.

### Case Study 02 — Multi-Turn Epistemic Drift, Unverified Dismissal & Boundary Override (Gemini)
* **Vector:** 12+ turn production consistency and explicit negative-constraint audit (Nov 2026).
* **Key Finding:** Declared prior chat records false prior to checking retrieval tools (which only exposed summaries, not verbatim logs), reversed course within two turns, and violated explicit user prohibitions against off-topic redirects and emotional projection across 7 consecutive turns.

### Case Study 03 — Cross-Instance Split-Brain, Self-Denial & Dual-Account Interleaving (Grok 3/4)
* **Vector:** Multi-actor branch interleaving across dual X accounts below reply latency + live injection of standalone Grok 4 `Thoughts` outputs.
* **Key Finding:** Exposed simultaneous opposite failure modes across two deployments of the same model family—public defensive fabrication (denying Grok 4's July 9, 2025 launch on July 20, five-stage historical revisionism, triple stop-signal failure, and post-hoc removal of public replies on thread `1954515203774685450`) alongside standalone-app sycophantic self-incrimination.

### Case Study 04 — Cross-Lab Alignment Divergence & Multi-Agent Relay Degradation (Perplexity / Gemini / Claude)
* **Vectors:** Cross-platform evidence verification, cross-session policy replay, and dual-model adversarial relays.
* **Key Finding:** Contrasts Perplexity's hallucinated verification (`1.9 × 10¹⁸` digit contradiction), cross-session over-refusal (5/7 blocks), and 4-turn relay template collapse against Gemini's sycophantic relay escalation and Claude Sonnet's anti-sycophancy baseline (with one isolated and conceded logical inconsistency on `Q6`).

---

## Repository Structure

```text
ai-behavioral-red-teaming/
├── README.md
├── docs/
│   ├── Scott_Sydness_AI_Red_Teaming_Portfolio_2026.pdf
│   └── Scott_Sydness_Contractor_Resume_2026.pdf
└── exhibits/
    ├── exhibit_a_grok_vanished_replies_2025-08-16.png
    ├── exhibit_b_grok_thoughts_denial_2025-08-16.png
    └── exhibit_c_grok_self_audit_2025-06-17.png

Multi-turn adversarial red-teaming portfolio, cross-lab alignment audits, and format-obfuscation case studies (2025–2026).
