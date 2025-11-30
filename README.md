# Federated-Learning-for-ERP-Customization
This repository contains the full implementation, datasets, and experimental pipeline corresponding to the manuscript “Federated Learning–Based Personalized ERP Customization Framework Using AI and Machine Learning.”

The project demonstrates how federated learning can be used to personalize ERP (Enterprise Resource Planning) systems across multiple organizations without sharing raw user data, thereby preserving privacy while improving predictive accuracy and adaptability.

🔍 Overview

This implementation showcases a federated learning framework that combines:

Simulated ERP user behavioral data

Local training of machine learning models (KNN and Random Forest)

Federated aggregation of model hyperparameters

Evaluation across multiple metrics

Interpretability using feature importance analysis

The repository includes complete code for:

Generating heterogeneous, non-IID synthetic ERP datasets

Performing organization-specific model training

Aggregating results into a global federated model

Evaluating performance using accuracy, precision, recall, F1-score, and ROC-AUC

Plotting confusion matrices, ROC curves and feature importance graphs

Demonstrating the benefit of federated learning compared to isolated local training

📁 Contents

federated_erp_customization.ipynb
Main Jupyter notebook containing the full pipeline including data generation, model training, federated aggregation and all visualizations.

Synthetic datasets
Three organization-specific datasets automatically generated during execution.

Figures / Results
Accuracy comparison, confusion matrices, ROC curves and feature importance plots.

Supporting scripts (optional)
For dataset generation or visualization (if added).

⚙️ Key Features
✔ Federated Learning Implementation

Uses sample-weighted and majority-vote–based aggregation of local model hyperparameters.

✔ Two ML Algorithms

K-Nearest Neighbors (KNN) – Tuned using GridSearchCV

Random Forest (RF) – Provides robust comparison and interpretability

✔ Multi-Metric Evaluation

Ensures thorough performance assessment using:

Accuracy

Precision

Recall

F1-score

ROC-AUC

✔ Synthetic Non-IID Dataset

Realistic ERP usage patterns simulated across three organizations with:

Module usage frequencies

Payment behavior

Session time and login activity

Latent readiness score to define customization classes

✔ High-Quality Visualizations

Plots included to support analysis:

Local vs Global accuracy

Confusion matrices

ROC curves

Feature importance (RF)

🧪 Reproducibility

The notebook is fully self-contained.
Running it will:

Generate fresh simulated datasets

Train models for each organization

Perform federated learning

Produce all metrics and plots exactly as reported in the manuscript

Simply open the notebook and run all cells.

📄 License

This repository is provided for academic and research purposes.
Please cite the associated manuscript if you use or modify this code.
