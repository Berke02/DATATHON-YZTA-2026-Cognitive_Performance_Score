# YZTA Datathon 2026 - Cognitive Performance Score Prediction

This project contains the cognitive performance score prediction solution developed for the Artificial Intelligence and Technology Academy (YZTA) Datathon 2026 competition.

## Approach Overview

To increase the size of the training dataset, the original competition data was merged with an external dataset named "Sleep Health and Daily Performance Dataset". The developed pipeline consists of the following steps:

* **Data Harmonization:** To resolve structural differences between the two datasets, Turkish columns and data contents were translated into English, and variables were standardized into a common format.
* **Missing Value Imputation:** Missing values were imputed using classifier models.
* **Feature Engineering:** Sentence embeddings and Principal Component Analysis (PCA) were used for categorical text features.
* **Modeling:** CatBoost algorithm with Optuna hyperparameter optimization was used for regression prediction.

## Results

* **Private Score:** 0.72055
* **Public Score:** 0.72165
