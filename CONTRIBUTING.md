# Contributing to the AI Cyber Risk Framework

Thank you for your interest in contributing! This project is an open community effort
to build a rigorous, practical framework for AI cyber risk management. Contributions
of all kinds are welcome — new terms, risk entries, controls, corrections, and
clarifications.

---

## Before You Contribute

### 1. Sign the Contributor License Agreement (CLA)

All contributors must sign the [Contributor License Agreement](CLA.md) before their
pull request can be merged. This protects both you and the project.

When you open your first pull request, **CLA Assistant** will automatically prompt you
to sign. It takes less than a minute and is tied to your GitHub account — you only
need to sign once.

### 2. Read the Framework Structure

The framework is organized into three pillars, each maintained as a separate
spreadsheet in the `framework/` directory:

| File | Pillar | Description |
|------|--------|-------------|
| `AIML_DEFINITIONS_AND_TAXONOMY.xlsx` | Pillar I | 112+ defined terms across 8 categories |
| `AIML_RISK_TAXONOMY.xlsx` | Pillar II | 187+ risks across 14 categories |
| `AIML_CONTROL_FRAMEWORK.xlsx` | Pillar III | 200+ sub-controls across 25 domains |

Familiarize yourself with the relevant spreadsheet before proposing changes.

---

## Types of Contributions

### New Entries
Adding a new term, risk, or control. Follow the naming and field conventions of
existing entries in the relevant spreadsheet (see conventions below).

### Corrections
Fixing errors in definitions, categorizations, or field values. Please cite a
source or provide a rationale in your pull request description.

### Clarifications
Improving the clarity or precision of existing entries without changing their meaning.

### Structural Suggestions
Proposing changes to categories, taxonomy structure, or field schema. Please open
a **GitHub Issue** first to discuss before submitting a pull request — structural
changes affect the whole framework and benefit from community discussion.

---

## Contribution Conventions

### Pillar I — AI Definitions & Taxonomy

- **Term names** should use Title Case.
- **Definitions** should be written in clear, concise prose — one to three sentences.
- **Category** must match one of the eight established categories. If you believe a
  new category is warranted, open an Issue first.
- **Source** field: cite your source (standard, paper, or established industry usage)
  where applicable.

### Pillar II — AI Risk Taxonomy

- **Risk names** should be concise noun phrases in Title Case (e.g., "Prompt Injection
  via User Input").
- **Classification** must be either `AI-Specific` or `Cyber-Technical`.
- **Category** must match one of the 14 established risk categories.
- **Description** should explain what the risk is and why it matters — typically two
  to four sentences.
- **Adverse Impact** field should describe the potential business or operational
  consequence.
- Do not duplicate an existing risk entry. Search the spreadsheet before adding.

### Pillar III — AI Control Framework

- **Control names** should be action-oriented verb phrases in Title Case (e.g.,
  "Implement Input Validation for Prompt Interfaces").
- **Domain** must match one of the 25 established control domains.
- **Control type** must be one of: Preventive, Detective, Corrective, or Deterrent.
- **Description** should be specific enough that a practitioner knows what to
  implement.
- Map the control to one or more risks from Pillar II where applicable.

---

## Pull Request Process

1. **Fork** the repository and create a branch from `main`.
2. **Make your changes** in the relevant spreadsheet(s).
3. **Describe your changes** clearly in the pull request — what you added or changed
   and why.
4. **Sign the CLA** if prompted by CLA Assistant.
5. A maintainer will review your pull request. We aim to respond within two weeks.

---

## Opening Issues

If you're not ready to submit a pull request but want to flag something — a missing
term, a potential error, a structural suggestion — please open a
[GitHub Issue](https://github.com/FireMountainLabs/ai-cyber-risk-framework/issues).

Use a descriptive title and include:
- Which pillar and spreadsheet is affected
- What you observed or are proposing
- Any supporting references or rationale

---

## Code of Conduct

This project is committed to a welcoming and inclusive environment. Contributors are
expected to engage respectfully and in good faith. Harassment or exclusionary behavior
of any kind will not be tolerated.

---

## Questions?

Open an issue or reach out at [info@firemountainlabs.com](mailto:info@firemountainlabs.com).
