[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
![Repo Size](https://img.shields.io/github/repo-size/MSBIDynamics/HMPV-Host-VBOF)
[![Zenodo DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.8270303-blue?style=flat-square&logo=zenodo&logoColor=white)](https://doi.org/10.5281/zenodo.22261626)

# Reproducing Optical Density (OD) data from Introduction of the β-hydroxyaspartate cycle in Synechococcus elongatus PCC 794
An existing genome-scale model (GEM) of Synechococcus elongatus PCC 7942 (iMS837) is employed to reproduce experimentally obtained optical density (OD) data and evaluate how the introduction of a new pathway, the β-hydroxyaspartate cycle, reprograms photorespiration metabolism.


# Table of Contents
1. [Project Structure](#project-structure)
2. [Installation](#installation)
3. [Citation](#Cite)
4. [Contact](#Contact)
5. [Licence](#Licence)


# Project Structure
```
Addition a New Pathway to the GEM of Synechococcus elongatus PCC 7942
├── src/                                                # Core module
│    └── dFBA.ipynb                                         # Main analysis
│
├── Data/                                               # Required data
│   ├── BG11.csv/                                          # Medium defined for COBRApy 
│   ├── growth_experimental_data.xlsx/                     # Growth experimental data used to reproduce data from model        
│   └── iMS837_modified.xml                                # Modified model based on docs
|
├── docs/                                               # Documentation (not required for running code)
│   ├── Changes_on_Model.pdf                               # All changes implemeneted on the model 
│   └── metabolic_map_BiGG_ID_Added.pdf                    # Metabolic map including core reactions, and the new pathway
│
├── output/                                             # Generated output files
│   ├── dFBA_Light_self-shading_Beer_Lambert.png           # The figure including experimental and regenerated data in one
│   ├── errorbar_dFBA_Light_self-shading_Beer_Lambert.png  # The same figure as above including error bar as png
│   ├── errorbar_dFBA_Light_self-shading_Beer_Lambert.pdf  # The same figure as above including error bar as pdf
│   └── dFBA_Light_self_shading_Beer_Lambert.xlsx          # The excel file including the experimental and regenarated data
|                       
└── README.md                                           # Current file
 ```

# Installation
To run the main analysis, dFBA.ipynb, Python 3.10 or higher and Python package manager (pip) are prerequisites:

### 1- Simply run the code, as the first command line in dFBA.ipynb includes Install required packages. You need to run this first cell including packages only once.

### 2- Make a conda environmet with all following requirements:

- **numpy** (2.2.6): Numerical computations
- **pandas** 2.3.3): Data manipulation and analysis
- **scipy** (1.15.3): Scientific computing
- **cobra** (0.31.1): Constraint-based metabolic modeling (COBRApy)
- **openpyxl** (3.1.5): A Python library to read/write Excel 2010 xlsx/xlsm files
- **matplotlib** (3.10.9): Visualization with Python
 

# Contact 
**Author**: Reihaneh Mostolizadeh

For questions or issues, please email Reihaneh.Mostolizadeh@computational.bio.uni-giessen.de.

# License
MIT License
Copyright (c) 2026 Reihaneh Mostolizadeh and MSBIDynamics - Justus Liebig University Giessen and Max Planck Institute for Terrestrial Microbiology
