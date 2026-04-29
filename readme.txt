# Graph-Based Modeling of Travel Advisory Risk

This repository contains code and resources to reproduce the experiments presented in the NeurIPS submission *“[Title Omitted for Double-Blind Review]”*. The project introduces a graph-based framework for modeling travel advisory systems using representation learning, clustering, and risk scoring.

---

## Overview

We model travel advisories as a graph where nodes represent countries and edges capture relationships derived from advisory signals. Using graph representation learning, we:

* Learn node embeddings using GraphSAGE-style aggregation
* Identify latent structure via clustering (k-means)
* Evaluate cluster validity using elbow, silhouette, and Calinski–Harabasz metrics
* Compute country-level and cluster-level risk scores
* Visualize results using UMAP and choropleth maps

---

## Repository Structure

```
project/
│
├── data/
│   ├── raw/                # Raw advisory data (or instructions to obtain it)
│   └── processed/          # Cleaned and structured data
│
├── scripts/
│   ├── code             # GraphSAGE implementation, Clustering and evaluation scripts, Risk score computation, visualization scripts
│   
│
│
├── results/
│   ├── embeddings
│   ├── clusters.csv        # Country-to-cluster assignments
│   
├── configs/
│   └── config.yaml         # Model and experiment settings
│
└── README.md
```

---

## Setup

Create a Python environment and install dependencies:



## Reproducing Results

### 1. Generate Node Embeddings


### 2. Perform Clustering


This step computes:

* cluster assignments
* evaluation metrics (elbow, silhouette, Calinski–Harabasz)

---

### 3. Compute Risk Scores



---

### 4. Generate Visualizations


This produces:

* UMAP embedding plots
* Choropleth risk maps

---

## Data

The dataset is constructed from publicly available travel advisory sources. Due to potential restrictions on redistribution, we provide:

* Data schema
* Preprocessing scripts
* Instructions to reconstruct the dataset

---

## Computational Requirements

All experiments were conducted on a standard CPU-based system (Intel Core i7-8650U, 64-bit OS).
No GPU is required. Total runtime for reproducing all results is under 2 hours.

---

## Reproducibility Notes

* Fixed random seeds are used where applicable
* Configuration parameters are provided in `configs/config.yaml`
* All figures and tables can be regenerated using provided scripts

---

## Limitations

* Results depend on the quality and consistency of advisory data sources
* Potential biases in reporting may affect learned representations
* Clustering outcomes are sensitive to parameter choices (e.g., number of clusters)

---

## License

This repository is released under an open-source license (to be specified).
All third-party data and libraries are used in accordance with their respective licenses.

---

## Anonymity Notice

This repository is anonymized for double-blind review. Identifying information will be added in the camera-ready version.

---
