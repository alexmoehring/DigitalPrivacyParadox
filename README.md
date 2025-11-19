# Digital Privacy Paradox Replication Package
This repository contains replication materials for the paper "The Digital Privacy Paradox and Choice Architecture: Evidence from an Experiment in Fintech." We are unable to share the underlying data due to privacy concerns, and therefore generate a simulated dataset to facilitate inspection of the code.

## Files
- main.ipynb - Main Jupyter notebook containing all analysis code
- pyproject.toml - Project dependencies and configuration
- poetry.lock - Exact dependency versions for reproducibility
- variable_descriptions.pdf - Variable names and definitions
- simluate_data.ipynb - Jupyter notebook that generates simulated dataset
- data_simulated.csv - Simulated dataset that can be used to verify the code.

## Requirements
The analysis requires Python 3.11+ with the following packages. The exact package versions, and all packages installed when running the code, can be found in the poetry.lock file or the requirements.txt file included in this repo.

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
We use poetry for environment management. The poetry.lock file contains the exact environment used. To construct the figures and tables from the paper, run the jupyter-notebook main.ipynb. Note the figures and tables created using the simulated data will differ from those using the real data.

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
