# Operationalizing Enterprise AI Security

**An Open-Source Framework for AI Cyber Risk Management**

Josh Harguess, **Chris M. Ward** (Fire Mountain Labs, San Diego, CA, USA) · Eric Cardinal (Delta Dental of California, San Francisco, CA, USA)

[CAMLIS 2026](https://www.camlis.org) (Conference on Applied Machine Learning in Information Security) poster session, 22 October 2026, Arlington, VA. [Download the 36 × 48 in PDF](CAMLIS2026_poster.pdf).

---

## 1. Motivation

| Traditional cybersecurity | AI systems |
| --- | --- |
| Deterministic: same input, same output | Non-deterministic: same prompt, different outputs |
| Attacks exploit code, configuration, access | Behavior steerable through inputs alone |
| Perimeter defense and patch management | Attack surface: training data, weights, inference API |

**AI-specific risk classes**

- Prompt injection
- Data poisoning
- Model extraction
- AI output liability
- Agentic goal misalignment

## 2. Framework Overview

| Pillar | Name | Size |
| --- | --- | --- |
| I | AI Definitions & Taxonomy | 112 terms · 8 categories |
| II | AI Risk Taxonomy | 171 risks · 14 categories |
| III | AI Control Framework | 177 sub-controls · 25 domains |

- Bidirectional risk–control mapping
- Operationalizes NIST AI RMF MEASURE and MANAGE [4]

## 3. Pillar I: Definitions

- 112 terms; sources: ISO/IEC 22989, NIST AI 600-1, OWASP LLM Top 10
- Security implication stated in each definition
- e.g., *User Prompt*: primary attack vector for generative AI

## 4. Pillar II: Risk Taxonomy

| 171 | 108 | 63 |
| :---: | :---: | :---: |
| Total risks | AI-specific | Cyber-technical |

| AI risk category (14) | Risks |
| --- | ---: |
| AI System Security | 23 |
| Model Reliability & Drift | 17 |
| Model Training | 16 |
| Generative Output | 9 |
| Excessive Agency | 9 |
| Socio-economic & Environmental | 8 |
| Third-Party & Supply Chain | 6 |
| Bias & Discrimination | 5 |
| Accountability & Governance | 4 |
| Multi-Agent Systems | 4 |
| Over-Reliance | 3 |
| Explainability | 2 |
| Shadow AI | 1 |
| Competitive Lag | 1 |

## 5. Risk Classification

| Risk | Class | Control placement |
| --- | --- | --- |
| Prompt injection `AIR.029` | Intentional, post-deployment | Runtime detection & response |
| Bias in training data `AIR.015` | Unintentional, pre-deployment | Data governance during curation |

- Three axes, adapted from the MIT AI Risk Repository [5]: entity, intentionality, timing
- Adversarial entries cross-mapped to MITRE ATLAS tactics and techniques [6]

> **Shadow AI (AIR.083):** no owner, review or telemetry; detection depends on network and API-gateway monitoring (AIMLT).

## 6. Pillar III: Controls

| Code | Core AI/ML domain (15; 5 shown) |
| --- | --- |
| `AISDL` | Secure data lifecycle |
| `AIMDV` | Model/agent validation & testing |
| `AIMLT` | Monitoring & telemetry |
| `AIIR` | Incident response & forensics |
| `AIGPC` | Governance, compliance & ethics |

| Code | Agentic domain (10; 5 shown) |
| --- | --- |
| `AGAS` | Goal alignment & safety |
| `SI` | Safe interruptibility |
| `TIS` | Tool instruction safety |
| `HOD` | Human oversight & decision |
| `ARTS` | Agentic red-team & simulation |

## 7. AI Security Service Team

Worked example: risk `R.AIR.058`, *Agent interaction & collusion*, traced through capability areas and control domains to individual controls.

| Capability area | Control domain | Control |
| --- | --- | --- |
| Detection & Response | `AIMLT` Monitoring & Telemetry | `AIMLT.11` Behavioral drift & tool-usage monitoring |
| Detection & Response | `AIIR` Incident Response & Forensics | `AIIR.1` AI & agent-aware IR playbook |
| Adversarial Testing | `ARTS` Agentic Red-Team & Simulation | `ARTS.2` Multi-agent simulation |
| Infrastructure | `AIIEH` Infrastructure Hardening | `AIIEH.11` Agent sandbox & egress control |
| Agentic Safety | `AII` Agent Interaction & Isolation | `AII.1` Agent trust boundary & segmentation |

Source: AI Cyber Risk Framework, R.AIR.058

## 8. Release and Future Work

- CC BY 4.0 spreadsheets: [github.com/FireMountainLabs/ai-cyber-risk-framework](https://github.com/FireMountainLabs/ai-cyber-risk-framework)
- Controls specify requirements, not implementation
- Future: maturity indicators per domain; expanded agentic coverage

## 9. References

1. J. Harguess and C. M. Ward. Is the next winter coming for AI? The elements of making secure and robust AI. *Trustworthy and Socially Responsible Machine Learning (TSRML), NeurIPS Workshop*, 2022.
2. C. M. Ward, J. Harguess, J. Tao, D. Christman, M. Tan, and P. Spicer. The AI security pyramid of pain. *Assurance and Security for AI-enabled Systems*, vol. 13054, pp. 44–53. SPIE, 2024.
3. J. Harguess and C. M. Ward. Offensive security for AI systems: concepts, practices, and applications. *Assurance and Security for AI-enabled Systems 2025*, vol. 13476. SPIE, 2025.
4. National Institute of Standards and Technology. Artificial Intelligence Risk Management Framework (AI RMF 1.0). NIST AI 100-1, 2023.
5. MIT FutureTech. The AI Risk Repository. arXiv:2408.12622v2, 2025.
6. The MITRE Corporation. MITRE ATLAS. https://atlas.mitre.org/, 2024.
