[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
![Repo Size](https://img.shields.io/github/repo-size/MSBIDynamics/HMPV-Host-VBOF)
[![Zenodo DOI](https://zenodo.org/badge/550401391.svg?style=plastic)](https://doi.org/10.5281/zenodo.15103805)

# Reproducing Optical Density (OD) data from Introduction of the β-hydroxyaspartate cycle in Synechococcus elongatus PCC 794
An existing genome-scale model (GEM) of Synechococcus elongatus PCC 7942 (iMS837) is employed to reproduce experimentally obtained optical density (OD) data and evaluate how the introduction of a new pathway, the β-hydroxyaspartate cycle, reprograms photorespiration metabolism.


# Table of Contents
-----
1. [Project Structure](#project-structure)
2. [Installation](#installation)
3. [Citation](#Cite)
4. [Contact](#Contact)
5. [Licence](#Licence)

---

# Project Structure

```
GEM_HMPV-Host_Interactions/
├── src/                                     # Core module
│   ├── FBA.ipynb                            # main analysis
│
├── Data/                                    # Required data
│   ├── BG11.csv/                            # medium defined for COBRApy 
│   ├── growth_experimental_data.xlsx/       # growth experimental data used for reproducing the data from the model        
│
├── docs/                                   # Documentation
│   ├── Changes_on_Model.pdf                # All changes implemeneted on the model are summerized in this file. 
│   └── metabolic_map_BiGG_ID_Added.pdf     # Metabolic map including core reactions, plus introducing a new pathway
│
├── output/                                 # Generated output files
│   ├── hmpv_vbof.json                      # Raw VBOF stoichiometry
│   ├── hmpv_vbof_normalized.json           # Normalized VBOF
│   ├── hmpv_vbof_summary.txt               # Human-readable VBOF summary
│   ├── iHsaEC21_CLEAN_with_HMPV_VBOF.xml   # Integrated model
│   ├── antiviral_analysis/                 # Antiviral target analysis results
│   └── sensitivity_analysis/               # Sensitivity analysis results
└── README.md                               # Current file
```
---

# Installation

To run the main analysis, FBA.ipynb, Python 3.10 or higher and Python package manager (pip) are prerequisites:

### 1- make a conda environmet with all following requirements:

- **numpy** (2.2.6): Numerical computations
- **pandas** 2.3.3): Data manipulation and analysis
- **scipy** (≥1.15.3): Scientific computing
- **cobra** (0.31.1): Constraint-based metabolic modeling (COBRApy)
- **openpyxl** (3.1.5): A Python library to read/write Excel 2010 xlsx/xlsm files
- **matplotlib** (3.10.9): Visualization with Python

#### 2- Simply run the code, as the first command line in FBA.ipynb Install required packages. You need to run it only once. 


# Contact 
**Author**: Reihaneh Mostolizadeh

For questions or issues, please email Reihaneh.Mostolizadeh@computational.bio.uni-giessen.de.

# License
MIT License
Copyright (c) 2026 Reihaneh Mostolizadeh and MSBIDynamics - Justus Liebig University Giessen and Max Planck Institute for Terrestrial Microbiology
