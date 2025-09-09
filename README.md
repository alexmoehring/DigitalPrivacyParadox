# Digital Privacy Paradox Replication Package
This repository contains replication materials for the paper "The Digital Privacy Paradox and Choice Architecture: Evidence from an Experiment in Fintech."

## Files
main.ipynb - Main Jupyter notebook containing all analysis code
data_public.csv - Anonymized experimental data
pyproject.toml - Project dependencies and configuration
poetry.lock - Exact dependency versions for reproducibility
variable_descriptions.pdf - Codebook for data_public.csv

## Data
The dataset (data_public.csv) contains experimental data from 3,108 participants across 4 study years. The variables and their descriptions are provided in variable_descriptions.pdf.

## Requirements
The analysis requires Python 3.11+ with the following packages:

poetry
pandas (>=2.2.3)
statsmodels (>=0.14.5)
pystout (>=0.0.8)
seaborn (>=0.13.2)
matplotlib
numpy
scipy
tqdm

## Replication
We use poetry for environment management. The poetry.lock file contains my exact environment

Install dependencies using:
```poetry install```

Running the Analysis:

1. Ensure data_public.csv is in the project root directory
2. ```poetry run jupyter-lab```
3. Open and run main.ipynb in Jupyter

The notebook generates:
1. Summary statistics tables
2. Balance tests for randomization
3. Treatment effect analyses for both "small costs" and "small talk" interventions
4. Choice model estimations using conditional logit
5. All output tables in LaTeX format

Citation
[Add appropriate citation information when paper is published]
