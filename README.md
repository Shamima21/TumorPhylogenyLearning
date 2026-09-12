from pathlib import Path

readme = """# TumorPhylogenyLearning

This repository contains the preliminary analysis for the project **Learning Conserved Evolutionary Patterns in Cancer from Patient-Specific Tumor Phylogenies**.

## About the Project

The aim of this project is to investigate whether heterogeneous tumor phylogenies show recurrent higher-level evolutionary patterns.

The analysis uses reconstructed tumor phylogenies from the **TRACERx421** cohort. A total of **398 tumor phylogenies** were retained for analysis.

## Preliminary Analysis

The current analysis includes:

- tumor phylogeny processing and validation
- evolutionary feature extraction
- feature correlation analysis
- feature redundancy reduction
- unsupervised clustering
- silhouette analysis
- comparison of clustering methods
- Adjusted Rand Index (ARI) analysis
- UMAP visualization
- representative tumor phylogeny analysis

The analysis initially considered **25 structural and mutation-based evolutionary features**. After examining feature redundancy, the representation was reduced to **6 relatively non-redundant evolutionary features**.

## Dataset

The analysis uses data from the **TRACERx421** study.

Dataset source:

https://zenodo.org/records/7683605

## Repository Files

- `Learning_Conserved_Evolutionary_Patterns_of_Cancer_Metastasis_from_Tumour_Phylogenies.ipynb`  
  Main tumor phylogeny analysis.

- `Feature_corelation__Learning_Conserved_Evolutionary_Patterns_of_Cancer_Metastasis_from_Tumour_Phylogenies.ipynb`  
  Feature correlation and feature reduction analysis.

- `Metastasis__Learning_Conserved_Evolutionary_Patterns_in_Cancer_from_Tumour_Phylogenies_ipynb.ipynb`  
  Additional exploratory analysis related to tumor evolutionary patterns.

## Note

This repository contains **preliminary and exploratory analyses**. 

## Author

**Shamima Naznin**  
Department of Computer Science and Engineering  
Bangladesh University of Engineering and Technology (BUET)
"""

path = Path("/mnt/data/README.md")
path.write_text(readme, encoding="utf-8")

print(path)
