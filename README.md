# AI Cyber Risk Framework

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

An open-source, practitioner-focused framework for operationalizing AI cyber risk
management in enterprise environments. Developed by [Fire Mountain Labs](https://firemountainlabs.com)
and introduced in the SPIE 2026 proceedings paper
*"Operationalizing Enterprise AI Security: An Open-Source Framework for AI Cyber Risk Management."*

---

## Overview

As AI systems become deeply embedded in enterprise operations, traditional cyber risk
frameworks are insufficient — they were not designed for the unique threats posed by
machine learning models, training pipelines, inference infrastructure, and agentic
systems. This framework addresses that gap.

The AI Cyber Risk Framework is organized into three pillars:

### Pillar I — AI Definitions & Taxonomy
`AIML_DEFINITIONS_AND_TAXONOMY.xlsx`

A controlled vocabulary of **112 terms** across **8 categories**, providing a shared
language for AI security practitioners, risk teams, and leadership. Consistent
terminology is the foundation for meaningful risk communication.

### Pillar II — AI Risk Taxonomy
`AIML_RISK_TAXONOMY.xlsx`

A structured catalog of **171 risks**: **108 AI-specific risks** across **14 categories**
(e.g., prompt injection, data poisoning, model extraction, agentic goal misalignment)
and **63 cyber-technical risks** organized by the six STRIDE categories (spoofing,
tampering, repudiation, information disclosure, denial of service, and elevation of
privilege) as they apply to AI deployment environments.

### Pillar III — AI Control Framework
`AIML_CONTROL_FRAMEWORK.xlsx`

A comprehensive set of **177 sub-controls** across **25 domains** (15 core AI/ML
lifecycle domains and 10 agentic AI domains), mapped to the risks in Pillar II. Each
sub-control is classified as AI-specific (addressing risks unique to AI systems) or
supporting (applying established cybersecurity practice to AI assets), and includes
maturity indicators to support implementation planning.

---

## Getting Started

1. **Clone or download** this repository.
2. Open the spreadsheet for the pillar most relevant to your use case.
3. Use the framework as-is, or adapt it to your organization's terminology and risk
   appetite.
4. If you find errors or want to contribute new entries, see [CONTRIBUTING.md](CONTRIBUTING.md).

---

## Use Cases

- **Risk assessments** — Use Pillar II to identify and scope AI-specific risks in your
  environment.
- **Control gap analysis** — Map your existing controls against Pillar III to identify
  coverage gaps.
- **Governance & policy** — Use Pillar I to establish consistent AI security terminology
  across your organization.
- **AI security program development** — Use all three pillars together as the foundation
  for a structured AI security practice.

---

## Citing This Work

If you use this framework in research or practice, please cite the accompanying paper:

> Josh Harguess, Chris M. Ward, and Eric Cardinal, "Operationalizing enterprise AI
> security: an open-source framework for AI cyber risk management," Proc. SPIE,
> Assurance and Security for AI-enabled Systems 2026 (2026). DOI to be assigned upon
> publication.

A machine-readable citation is available in [CITATION.cff](CITATION.cff).

---

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for
conventions and the pull request process. All contributors must sign the
[Contributor License Agreement](CLA.md) before their first pull request is merged.

---

## License

This work is licensed under the
[Creative Commons Attribution 4.0 International License](LICENSE) (CC BY 4.0).

You are free to share and adapt this material for any purpose, including commercially,
as long as you provide appropriate attribution to Fire Mountain Labs.

---

## Contact

Questions, partnerships, or enterprise inquiries:
[info@firemountainlabs.com](mailto:info@firemountainlabs.com)
