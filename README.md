# Unlimited-GROMACS-Cloud

> **Run long (100 ns+) GROMACS molecular dynamics simulations on free cloud GPUs using automatic checkpointing and seamless session recovery.**

A lightweight, single-script workflow that enables researchers to perform production-scale molecular dynamics simulations without requiring dedicated HPC infrastructure. Designed for students, researchers, and laboratories with limited computational resources.

---

## Overview

Running long molecular dynamics simulations often requires access to high-performance computing (HPC) clusters or expensive GPU hardware. **Unlimited-GROMACS-Cloud** provides a practical alternative by leveraging free cloud GPU platforms while automatically handling interrupted sessions through checkpoint-based continuation.

The workflow is designed to be simple, reproducible, and beginner-friendly, allowing users to focus on their research rather than infrastructure management.

---

## Features

### Molecular Dynamics Workflow

- Run GROMACS entirely on free cloud GPU platforms
- Automatic checkpoint creation and simulation continuation
- Support for long production simulations (100 ns+)
- Complete end-to-end protein molecular dynamics workflow
- Optimized for limited cloud computing resources
- Single-script execution
- Beginner-friendly and reproducible

---

### Included Analyses

The workflow automatically performs commonly used trajectory analyses:

- ✅ Root Mean Square Deviation (RMSD)
- ✅ Root Mean Square Fluctuation (RMSF)
- ✅ Radius of Gyration (Rg)
- ✅ Solvent Accessible Surface Area (SASA)
- ✅ Hydrogen Bond Analysis
- ✅ Principal Component Analysis (PC1–PC2)
- ✅ 2D Free Energy Surface (FES)
- ✅ 3D Free Energy Landscape (FEL)
- ✅ Dynamic Cross-Correlation Matrix (DCCM)
- ✅ DSSP Secondary Structure Assignment
- ✅ Secondary Structure Heatmap
- ✅ Secondary Structure Population Over Time

---

## Workflow

```
Protein Structure
        │
        ▼
System Preparation
        │
        ▼
Energy Minimization
        │
        ▼
NVT Equilibration
        │
        ▼
NPT Equilibration
        │
        ▼
Production Molecular Dynamics
        │
        ▼
Automatic Checkpoint Recovery
        │
        ▼
Trajectory Analysis
        │
        ▼
Publication-Ready Figures
```

---

## Repository Contents

```
.
├── Unlimited_GROMACS_Cloud.ipynb
└── README.md
```

The notebook contains the complete workflow for running protein-only molecular dynamics simulations and performing automated trajectory analysis.

---

## Intended Users

This project is suitable for:

- Computational biologists
- Structural biologists
- Bioinformaticians
- Molecular dynamics researchers
- Students learning GROMACS
- Researchers without dedicated HPC access
- Laboratories with limited computational resources

---

## Requirements

- Python
- GROMACS
- Free cloud GPU platform (e.g., Kaggle)
- Basic familiarity with molecular dynamics simulations

---

## Citation

If this repository contributes to your research, please consider citing it in your publications and acknowledging the project.

---

## License

This project is released under the appropriate open-source license included in this repository.

---

## Disclaimer

This project is intended for research and educational purposes.

"Unlimited" refers to the practical ability to perform long simulations through automatic checkpointing and continuation across multiple cloud sessions. Actual compute availability is subject to the policies and limits of the cloud platform being used.
