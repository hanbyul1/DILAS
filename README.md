# DILAS

This repository contains the evaluation artifacts for the paper:

> **A Systematic Architectural Modeling Approach for Data-Intelligent Software Systems**

The repository provides the complete materials required to reproduce the architectural structuring evaluation presented in the paper, including the prompt histories used during AI-assisted development and the computed architectural analysis results.

---

# Repository Structure

```
DILAS
├── chat logs/
└── snapshot analysis/
```

## chat logs/

This directory contains representative chat histories generated during the AI-assisted development of the evaluated systems. These logs document the architectural modeling and implementation interactions between the developer and large language models.

The directory includes chat logs for:

- **MenuCal**
- **NutriCompass**
- **PartGuard**
- **DocuSense**

The logs illustrate different AI-assisted development approaches, including:

- vibe coding
- vibe architecting
- DILAS-guided architectural modeling
- DILAS-guided implementation

These artifacts provide transparency regarding the architectural decisions made throughout system development.

---

## snapshot analysis/

This directory contains the complete architectural analysis results used in the paper.

For each evaluated system, the following files are provided.

### `<system>_as_modules.csv`

Organizational modules identified for architectural analysis together with their inferred architectural responsibilities.

---

### `<system>_as_dependencies.csv`

Inter-module dependency relationships extracted from the implementation.

---

### `<system>_as_cyclic_modules.csv`

Modules participating in dependency cycles identified during Dependency Organization (DO) analysis.

---

### `<system>_as_ignored_types.csv`

Implementation types excluded from dependency analysis because they could not be associated with identifiable architectural responsibilities.

---

### `<system>_as_snapshots.csv`

Architectural Structuring (AS) results for all development snapshots used in the longitudinal evaluation.

---

### `<system>_as_summary.json`

Summary statistics for the evaluated system, including the final values of:

- Responsibility Separation (RS)
- Dependency Organization (DO)
- Architectural Structuring (AS)

---

# Evaluated Systems

The repository contains evaluation results for four AI-enabled software systems.

| System | Development Approach |
|---------|----------------------|
| MenuCal | Vibe Coding |
| NutriCompass | Vibe Architecting + Vibe Coding |
| PartGuard | Vibe Architecting (with partial DILAS influence) + Vibe Coding |
| DocuSense | DILAS + Vibe Coding |

---

# Reproducibility

The repository contains the artifacts necessary to reproduce the architectural structuring evaluation reported in the paper, including:

- AI-assisted development chat logs
- Architectural analysis outputs
- Longitudinal snapshot results
- Summary metrics

These materials support independent verification of the reported Responsibility Separation (RS), Dependency Organization (DO), and Architectural Structuring (AS) results.

---

# Citation

If you use this repository, please cite:

```bibtex
@article{Kim2026DILAS,
  title   = {A Systematic Architectural Modeling Approach for Data-Intelligent Software Systems},
  author  = {Dae-Kyoo Kim},
  year    = {2026}
}
```

---

# License

This repository is provided for research and reproducibility purposes.
