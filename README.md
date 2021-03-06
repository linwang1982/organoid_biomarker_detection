# organoid_biomarker_detection
# Network-based biomarker detection from organoid models to predict drug response in cancer patients
Source code to reproduce the paper "Network-based machine-learning in colorectal and bladder organoid models predicts anti-cancer drug efficacy in patients", Kong et al

# Requirements
- python (v 2.7.13)
- pandas (v 0.24.2)
- matplotlib (v 2.0.0)
- numpy (v 1.16.6)
- scipy (v 1.2.2)
- sklearn (v 0.20.2)
- lifelines (v 0.19.5)
- gseapy 

# Installation instruction
- All python packages can be installed via pip (https://pypi.org/project/pip/).
- e.g. pip install [package name].
- Installations would take few minutes for each python package.

# Code (for python)
- "run_ssGSEA.py" to generate pathway level expression profiles using single sample GSEA (ssGSEA) tool (gseapy)
- "single_pathway_prediction.py" to predict drug response in cancer patients using a single pathway
- "multiple_pathway_prediction.py" to predict drug response in cancer patients using multiple pathways

# Demo
- Code for drug response prediction of 5fluorouracil-treated colorectal cancer patients using colorectal cancer organoids
- Expected results are provided under "./python/results/" folder.
- The majority of the code runs within several minutes, with the execption of "run_ssGSEA.py", which may take several hours depending on the size of a sample cohort.


# Network proximity was calculated using codes from
- 'Uncovering disease-disease relationships through the incomplete interactome' Menche et al, Science, 2015
- 'Network-based in silico drug efficacy screening' Emre et al, Nature Communications, 2016
- https://github.com/emreg00/toolbox

