# Neuron Communication Project

## Project Overview
The aim of this project is to investigate the communication between neuron cells and cancer cells in brain metastasis. We utilized five mouse models: **wild type, sham, lung, breast,** and **melanoma**. This repository contains scripts and results that facilitate the analysis of single-cell RNA sequencing (scRNA-seq) data from these models, allowing for a comprehensive understanding of tumor microenvironments (TME).

## Repository Structure
This repository is organized into several folders, each dedicated to specific analysis steps:

### 1. Quality Control
- **Description:** This folder includes scripts that perform quality control checks for each mouse model separately. 
- **Purpose:** The quality control process ensures that the scRNA-seq data meets the necessary criteria for further analysis, allowing us to filter out low-quality cells.

### 2. Preprocessing
- **Description:** This folder contains scripts that handle the preprocessing of the data, which includes:
  - **Normalization:** Adjusting the data to account for variations in sequencing depth.
  - **Selection of Highly Variable Genes:** Identifying genes that show significant variability across the samples, which are crucial for downstream analyses.
  - **Dimensionality Reduction:** Techniques such as PCA or t-SNE to reduce the complexity of the data while retaining essential information.

### 3. Annotation
- **Description:** This folder holds individual files for each mouse model detailing how we annotate the cells. The annotation process assigns cell types based on expression profiles, allowing for a clearer understanding of the cellular composition.
- **InferCNV Results:** Within this folder, you will find results from the InferCNV analysis organized into subfolders named by each mouse model. This analysis provides insights into copy number variations within the tumors.

### 4. Integration
- **Description:** This folder includes two key scripts:
  - **Integration Script:** This script assesses the percentage of each cell type present in each model and integrates the TME data from all mouse models separately.
  - **Annotation of Integrated Data:** This script annotates the integrated data from all mouse models, facilitating comprehensive comparisons across different models.

## Outputs (What you need to check)
- **HTML Files:** These files provide detailed reports of the analyses conducted at each step.
- **PNG Files:** InferCNV Results (infercnv.png and infercnv.17_HMM_predHMMi6.leiden.hmm_mode-subclusters.png)
- **xlsx**: This is excel file contain the marker genes calculated for each cluster in each model or integrated data (within each scel file, each sheet have the genes of each cluster)
- **qs:** This is the original scripts (you don't need to open it or share with with anyone)

## Collaboration and Sharing
This repository is designed to share results with colleagues and collaborators. When the paper is published, we can easily provide the code and analyses to reviewers upon request.

Feel free to explore the folders and files for a detailed understanding of the analyses performed in this project. For any questions or clarifications, please reach out.
