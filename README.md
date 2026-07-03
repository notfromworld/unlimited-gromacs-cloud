# Unlimited-GROMACS-Cloud-Analysis

> **A cloud-based Jupyter notebook for step-by-step analysis of GROMACS molecular dynamics trajectories.**

**Online-GROMACS-Analysis** is an open-source Jupyter notebook designed to perform comprehensive post-simulation analysis of GROMACS molecular dynamics trajectories using free cloud computing platforms such as Kaggle. The notebook provides a structured, cell-by-cell workflow that guides users through commonly used trajectory analyses and generates publication-ready figures for protein molecular dynamics studies.

Unlike automated pipelines, each analysis step is presented individually, allowing users to understand, modify, and execute every stage of the workflow according to their research requirements.

---

## Overview

Trajectory analysis is an essential component of molecular dynamics simulations, providing insights into structural stability, flexibility, conformational changes, correlated motions, and energetic landscapes. However, setting up analysis scripts can be repetitive and time-consuming, particularly for new users.

This repository consolidates commonly used GROMACS trajectory analyses into a single notebook with clearly organized sections. Each analysis can be executed independently, making the notebook suitable for both educational purposes and research projects.

The notebook is intended for **post-processing only**. Molecular dynamics simulations should be completed prior to using this repository.

---

## Features

* Step-by-step Jupyter notebook workflow
* Runs on free cloud computing platforms (e.g., Kaggle)
* No local GPU required for notebook execution
* Individual analysis sections that can be run independently
* Publication-ready figures
* Beginner-friendly organization
* Easily customizable for different systems
* Suitable for protein molecular dynamics trajectories

---

## Included Analyses

The notebook includes the following analyses:

* Root Mean Square Deviation (RMSD)
* Root Mean Square Fluctuation (RMSF)
* Radius of Gyration (Rg)
* Solvent Accessible Surface Area (SASA)
* Hydrogen Bond Analysis
* MM/PBSA Binding Free Energy Analysis
* Principal Component Analysis (PC1–PC2)
* Two-Dimensional Free Energy Surface (2D FES)
* Three-Dimensional Free Energy Landscape (3D FEL)
* Dynamic Cross-Correlation Matrix (DCCM)
* DSSP Secondary Structure Assignment
* Secondary Structure Heatmap
* Secondary Structure Population Over Time

---

## Repository Structure

```text
Online-GROMACS-Analysis/
│
├── Online_GROMACS_Analysis.ipynb
├── README.md
├── LICENSE
├── CITATION.cff
└── requirements.txt
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/Online-GROMACS-Analysis.git
```

### 2. Open the notebook

Launch Jupyter Notebook or upload the notebook to Kaggle.

### 3. Prepare your simulation outputs

The notebook expects trajectories and topology files generated from completed GROMACS simulations.

Typical input files include:

* `.xtc`
* `.tpr`
* `.gro`
* `.top`
* `.edr`
* index files (`.ndx`) where applicable

### 4. Execute analyses

Run each notebook cell sequentially. Every section contains the commands necessary for a specific analysis and can be modified to suit individual projects.

---

## Software Requirements

* Python 3.x
* GROMACS
* Jupyter Notebook
* NumPy
* Pandas
* Matplotlib
* MDTraj (where applicable)
* DSSP
* gmx_MMPBSA (for MM/PBSA calculations)

Additional dependencies are listed in `requirements.txt`.

---

## Intended Users

This repository is intended for:

* Molecular dynamics researchers
* Computational biologists
* Structural biologists
* Bioinformaticians
* Students learning GROMACS analysis
* Researchers without access to dedicated HPC resources

---

## Limitations

* This repository does **not** perform molecular dynamics simulations.
* Users are expected to have completed their simulations before using the notebook.
* Input trajectories should be generated using GROMACS.
* Individual analyses may require additional software such as DSSP or gmx_MMPBSA.

---

## Citation

If this notebook contributes to your research, please cite the archived Zenodo release.

After publication on Zenodo, the citation information will be available through both the DOI and GitHub's **"Cite this repository"** feature.

Example BibTeX:

```bibtex
@software{ray2026onlinegromacsanalysis,
  author    = {Soumyadeep Ray},
  title     = {Online GROMACS Analysis},
  year      = {2026},
  publisher = {Zenodo},
  doi       = {10.5281/zenodo.xxxxxxx}
}
```

---

## License

This project is distributed under the license included in this repository.

---

## Acknowledgements

This notebook was developed to simplify post-simulation molecular dynamics analysis for the broader research community by consolidating commonly used GROMACS analyses into a single, organized workflow.

Contributions, suggestions, and improvements are welcome through GitHub Issues and Pull Requests.
