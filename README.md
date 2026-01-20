# Genomic Mutation Impact Predictor

## Project Overview
This repository contains a probabilistic framework for predicting the pathogenicity of genomic mutations. Using a dataset of **7.87 million variants**, this project implements a **Bayesian Network** to model complex dependencies between biological features and mutation impact.

The primary goal was to achieve high-precision classification within highly imbalanced genomic classes by optimizing model structure and utilizing exact inference techniques.

## Key Results
* **Accuracy:** 91.7% overall accuracy on imbalanced test sets.
* **Precision:** Exceeded historical precision baselines by **4x** using Variable Elimination.
* **Efficiency:** Optimized DAG structure discovery using **HillClimbSearch** and **BIC scoring**.

## Technical Highlights
* **Structural Learning:** Automated model discovery via HillClimbSearch to identify optimal conditional dependencies.
* **Inference Engine:** Implemented **Variable Elimination** for exact probabilistic inference and **Viterbi-path analysis** for decision tracking.
* **Data Scale:** Engineered features and handled preprocessing for a **7.87M variant dataset**.
* **Scoring Metrics:** Leveraged Bayesian Information Criterion (BIC) to prevent model overfitting while maintaining predictive power.

## Tech Stack
* **Language:** Python
* **Libraries:** `pgmpy` (Probabilistic Graphical Models), `scikit-learn`, `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`, `networkx`

## Repository Structure
* `Genomic_Mutation_Predictor.ipynb`: The primary workbook containing data preprocessing, structural learning, and model evaluation.
* `Project_Report.pdf`: A formal technical report detailing the mathematical methodology and results.
