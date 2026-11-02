<p align="center">
  <img src="figures/banner.svg" alt="Operationalizing Enterprise AI Security: an open-source framework for AI cyber risk management." width="100%">
</p>

<p align="center">
  <a href="poster.pdf"><img alt="Download the PDF" src="https://img.shields.io/badge/Poster-36%20%C3%97%2048%20in%20PDF-003452?style=for-the-badge&labelColor=74121D"></a>
  <a href="https://github.com/FireMountainLabs/ai-cyber-risk-framework"><img alt="Framework repository" src="https://img.shields.io/badge/Framework-CC%20BY%204.0-003452?style=for-the-badge&labelColor=56876D"></a>
</p>

---

## 1 · Motivation

<img src="figures/motivation.svg" alt="Traditional cybersecurity is deterministic, with attacks on code, configuration and access. AI systems are non-deterministic, steerable through inputs alone, with an attack surface of training data, weights and inference API." width="100%">

**AI-specific risk classes**

<img src="figures/risk-classes.svg" alt="AI-specific risk classes: prompt injection, data poisoning, model extraction, AI output liability, agentic goal misalignment" width="100%">

## 2 · Framework Overview

<img src="figures/pillars.svg" alt="Three pillars: Pillar I AI Definitions and Taxonomy, 112 terms in 8 categories; Pillar II AI Risk Taxonomy, 171 risks in 14 categories; Pillar III AI Control Framework, 177 sub-controls in 25 domains." width="100%">

- Bidirectional risk–control mapping
- Operationalizes NIST AI RMF MEASURE and MANAGE [4]

## 3 · Pillar I: Definitions

- **112 terms**; sources: ISO/IEC 22989, NIST AI 600-1, OWASP LLM Top 10
- Security implication stated in each definition
- e.g., *User Prompt*: primary attack vector for generative AI

## 4 · Pillar II: Risk Taxonomy

<img src="figures/risk-taxonomy.svg" alt="Pillar II has 171 risks: 108 AI-specific and 63 cyber-technical. The largest AI risk category is AI System Security with 23 risks." width="100%">

<details>
<summary>Risk counts as a table</summary>

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

</details>

## 5 · Risk Classification

| Risk | Class | Control placement |
| --- | --- | --- |
| Prompt injection `AIR.029` | Intentional, post-deployment | Runtime detection & response |
| Bias in training data `AIR.015` | Unintentional, pre-deployment | Data governance during curation |

- Three axes, adapted from the MIT AI Risk Repository [5]: entity, intentionality, timing
- Adversarial entries cross-mapped to MITRE ATLAS tactics and techniques [6]

> [!WARNING]
> **Shadow AI (`AIR.083`):** no owner, review or telemetry; detection depends on network and API-gateway monitoring (`AIMLT`).

## 6 · Pillar III: Controls

<table>
<tr><th>Code</th><th>Core AI/ML domain <sub>(15; 5 shown)</sub></th><th>Code</th><th>Agentic domain <sub>(10; 5 shown)</sub></th></tr>
<tr><td><code>AISDL</code></td><td>Secure data lifecycle</td><td><code>AGAS</code></td><td>Goal alignment &amp; safety</td></tr>
<tr><td><code>AIMDV</code></td><td>Model/agent validation &amp; testing</td><td><code>SI</code></td><td>Safe interruptibility</td></tr>
<tr><td><code>AIMLT</code></td><td>Monitoring &amp; telemetry</td><td><code>TIS</code></td><td>Tool instruction safety</td></tr>
<tr><td><code>AIIR</code></td><td>Incident response &amp; forensics</td><td><code>HOD</code></td><td>Human oversight &amp; decision</td></tr>
<tr><td><code>AIGPC</code></td><td>Governance, compliance &amp; ethics</td><td><code>ARTS</code></td><td>Agentic red-team &amp; simulation</td></tr>
</table>

## 7 · AI Security Service Team

Worked example: risk `R.AIR.058`, *Agent interaction & collusion*, traced through capability areas and control domains to individual controls.

<img src="figures/service-team.svg" alt="Risk R.AIR.058, agent interaction and collusion, maps to four capability areas, five control domains and five controls: Detection and Response (AIMLT.11 behavioral drift and tool-usage monitoring; AIIR.1 AI and agent-aware IR playbook), Adversarial Testing (ARTS.2 multi-agent simulation), Infrastructure (AIIEH.11 agent sandbox and egress control), Agentic Safety (AII.1 agent trust boundary and segmentation)." width="100%">

<sub>Source: AI Cyber Risk Framework, R.AIR.058</sub>

## 8 · Release and Future Work

- CC BY 4.0 spreadsheets: [github.com/FireMountainLabs/ai-cyber-risk-framework](https://github.com/FireMountainLabs/ai-cyber-risk-framework)
- Controls specify requirements, not implementation
- Future: maturity indicators per domain; expanded agentic coverage

## 9 · References

1. J. Harguess and C. M. Ward. Is the next winter coming for AI? The elements of making secure and robust AI. *Trustworthy and Socially Responsible Machine Learning (TSRML), NeurIPS Workshop*, 2022.
2. C. M. Ward, J. Harguess, J. Tao, D. Christman, M. Tan, and P. Spicer. The AI security pyramid of pain. *Assurance and Security for AI-enabled Systems*, vol. 13054, pp. 44–53. SPIE, 2024.
3. J. Harguess and C. M. Ward. Offensive security for AI systems: concepts, practices, and applications. *Assurance and Security for AI-enabled Systems 2025*, vol. 13476. SPIE, 2025.
4. National Institute of Standards and Technology. Artificial Intelligence Risk Management Framework (AI RMF 1.0). NIST AI 100-1, 2023.
5. MIT FutureTech. The AI Risk Repository. arXiv:2408.12622v2, 2025.
6. The MITRE Corporation. MITRE ATLAS. https://atlas.mitre.org/, 2024.

---

## The poster

<a href="poster.pdf"><img src="figures/poster-preview.png" alt="The full poster" width="100%"></a>
