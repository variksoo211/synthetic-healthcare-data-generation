# Paper 01

## Title

Modeling Tabular Data using Conditional GAN

## Authors

Lei Xu, Maria Skoularidou, Alfredo Cuesta-Infante, Kalyan Veeramachaneni

## Conference

NeurIPS 2019

## Main Objective

The paper proposes a deep learning framework called CTGAN to generate realistic synthetic tabular data while preserving the statistical properties of the original dataset.

## Problem Addressed

Generating synthetic tabular data is more challenging than generating images because tabular datasets contain both continuous and categorical variables. In addition, categorical variables are often highly imbalanced and continuous variables may follow complex multimodal distributions.

## Proposed Methods

- CTGAN (Conditional Tabular GAN)
- TVAE (Tabular Variational Autoencoder)

## Main Contributions

- Introduced CTGAN for synthetic tabular data generation.
- Proposed mode-specific normalization for continuous variables.
- Introduced conditional sampling to better learn imbalanced categorical features.
- Introduced TVAE as a second deep generative model.
- Built a benchmark including multiple real and simulated datasets.

## Evaluation

The authors evaluated CTGAN and TVAE on several real and simulated datasets.

Evaluation focused on:

- Machine Learning Utility
- Statistical Similarity
- Comparison with Bayesian methods
- Comparison with previous GAN models

## Main Findings

CTGAN achieved better performance than previous tabular data generation methods on most real datasets and successfully preserved important statistical characteristics.

## Why is this paper important for my thesis?

This is the most important reference for my project because I will implement and evaluate CTGAN and TVAE on the Stroke Prediction Dataset to generate synthetic healthcare data.

## Personal Notes

This paper introduces the two main models that will be implemented during the thesis. It also explains the main challenges of generating synthetic tabular healthcare data.