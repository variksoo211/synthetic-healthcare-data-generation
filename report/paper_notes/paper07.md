# Paper 07

## Title

CTAB-GAN+: Enhancing Tabular Data Synthesis

## Authors

Zilong Zhao
Aditya Kunar
Robert Birke
Hiek Van der Scheer
Lydia Y. Chen

## Year

2024

## Journal

Frontiers in Big Data

---

# Main Objective

The paper introduces CTAB-GAN+, an improved conditional Generative Adversarial Network designed to generate high-quality synthetic tabular data while simultaneously improving data utility and preserving privacy through Differential Privacy.

---

# Problem Addressed

Although recent GAN-based synthesizers such as CTGAN and CTAB-GAN generate realistic synthetic tabular datasets, they still present several limitations:

- Limited downstream machine learning utility.
- Difficulty modeling highly skewed variables.
- Challenges with mixed continuous and categorical variables.
- Privacy leakage risks when synthetic data becomes too similar to real data.

The authors propose CTAB-GAN+ to overcome these issues.

---

# Proposed Method

CTAB-GAN+ extends CTAB-GAN by introducing:

- Downstream Classification Loss
- Downstream Regression Loss
- Wasserstein GAN with Gradient Penalty (WGAN-GP)
- Improved Conditional Vector Encoding
- Differential Privacy Stochastic Gradient Descent (DP-SGD)

These improvements increase both data utility and privacy.

---

# Data Types Supported

- Continuous variables
- Categorical variables
- Mixed variables
- Long-tail distributions
- Highly imbalanced datasets

---

# Evaluation

The authors evaluate CTAB-GAN+ using:

- Machine Learning Utility
- Statistical Similarity
- Classification Accuracy
- Regression Performance
- Differential Privacy Analysis

The model is compared with:

- CTGAN
- TVAE
- CTAB-GAN
- Gaussian Copula

---

# Main Results

The experiments show that CTAB-GAN+ consistently outperforms previous GAN-based tabular synthesizers.

The proposed downstream feedback mechanism significantly improves predictive performance on synthetic datasets.

The Differential Privacy version provides strong privacy guarantees while maintaining useful synthetic data.

---

# Advantages

- Better synthetic data quality.
- Better downstream ML performance.
- Handles mixed data types.
- Supports skewed distributions.
- Provides Differential Privacy.
- More stable GAN training.

---

# Limitations

- Longer training time than statistical models.
- Requires careful hyperparameter tuning.
- Privacy protection may reduce utility when strict privacy budgets are applied.

---

# Relation to My Thesis

This paper is highly relevant because it represents one of the most advanced GAN-based approaches for synthetic tabular data generation. Although this thesis focuses on CTGAN, TVAE and Gaussian Copula, CTAB-GAN+ provides an important reference for understanding recent improvements in synthetic healthcare data generation, especially regarding data utility and privacy preservation.

---

# Personal Notes

CTAB-GAN+ extends previous GAN-based synthesizers by combining higher-quality synthetic data generation with privacy-preserving mechanisms. The proposed downstream feedback losses improve machine learning performance, making this model one of the strongest recent approaches for tabular data synthesis.