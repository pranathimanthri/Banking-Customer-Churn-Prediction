## Overview

This project addresses the challenge of predicting customer churn at a bank by combining rigorous data preparation, insightful exploratory analysis, and a suite of machine learning techniques. Starting with the “Bank Churners” dataset—which contains demographic details (age, gender, income category), account metrics (credit limit, transaction counts), and churn labels—we clean and preprocess all fields, encode categorical variables, and handle missing values to ensure a reliable foundation for downstream analysis.

## Data Preparation & Exploratory Analysis

In the data preparation phase, we systematically transform raw customer records into model-ready features. We recode and normalize attributes like education level and credit utilization, then split the dataset into training and test sets. Our exploratory analysis employs histograms, boxplots, and correlation heatmaps to reveal which factors—such as tenure length, credit usage ratios, and transaction patterns—correlate most strongly with churn, guiding our feature selection and engineering efforts.

## Modeling Techniques

We implement four distinct classification models in separate Jupyter notebooks to compare their strengths and trade-offs. A decision tree offers interpretability through clear decision rules, while a support vector machine explores high-dimensional feature spaces using both linear and RBF kernels. Naive Bayes serves as a fast, probabilistic baseline under feature‐independence assumptions, and a neural network (multilayer perceptron) captures complex, nonlinear interactions by tuning hidden layers and learning rates.

## Model Evaluation & Insights

Each model undergoes hyperparameter tuning via cross-validation and is evaluated against a held-out test set using accuracy, precision, recall, F1-score, and ROC AUC. The neural network achieves the highest ROC AUC by uncovering subtle patterns in customer behavior, whereas the SVM and decision tree deliver competitive accuracy with greater interpretability. Naive Bayes, although the quickest to train, shows limitations when feature correlations are strong.

## Conclusion & Future Work

This repository delivers a complete, end-to-end churn prediction pipeline—from raw data ingestion through model comparison and evaluation—equipping data scientists and banking stakeholders with actionable insights. Future enhancements could include ensemble methods for improved stability, time-series modeling of customer engagement, or the development of a deployment pipeline for real-time churn scoring.
