# Paper 05

## Title

CTGAN: An Improved Generative Adversarial Network for Synthetic Tabular Data

## Authors

David Fuentes
Diana McSpadden
Sodiq Adewole

## Year

2023

## Source

arXiv

---

# Main Objective

The paper presents an improved version of the Conditional Tabular Generative Adversarial Network (CTGAN) for generating high-quality synthetic tabular data. The proposed improvements aim to enhance the quality, stability, and diversity of the generated synthetic datasets.

---

# Problem Addressed

Generating realistic synthetic tabular healthcare data remains challenging because datasets usually contain mixed numerical and categorical variables, highly imbalanced classes, and complex nonlinear relationships.

Traditional GAN models often suffer from:

- Mode collapse
- Unstable training
- Poor minority class generation

The paper proposes improvements to overcome these limitations.

---

# Proposed Method

Improved Conditional Tabular GAN (CTGAN)

---

# Main Contributions

- Improves the original CTGAN architecture.
- Enhances stability during training.
- Generates more realistic synthetic tabular data.
- Preserves statistical relationships between variables.
- Better captures minority classes.

---

# Method Overview

The proposed model follows these main steps:

1. Data preprocessing.
2. Conditional sampling.
3. Generator produces synthetic samples.
4. Discriminator distinguishes real from synthetic data.
5. Adversarial training updates both networks until convergence.

---

# Evaluation

The model is evaluated using:

- Statistical similarity
- Machine Learning Utility
- Classification performance
- Distribution preservation

The generated synthetic data are compared with real datasets and previous GAN models.

---

# Results

The improved CTGAN:

- Produces higher quality synthetic tabular datasets.
- Better preserves correlations.
- Improves minority class generation.
- Achieves better predictive performance compared with previous methods.

---

# Advantages

- Better training stability.
- Improved synthetic data quality.
- Handles mixed-type tabular data.
- Better representation of minority classes.
- Suitable for healthcare datasets.

---

# Limitations

- Training time remains relatively high.
- Requires GPU for efficient training.
- Hyperparameter tuning is still important.

---

# Relevance to My Thesis

This paper is highly relevant because my thesis focuses on generating synthetic healthcare tabular data. The proposed improvements provide useful insights that may be considered when implementing and evaluating CTGAN on the Stroke Prediction Dataset.

---

# Personal Notes

This paper extends the original CTGAN framework and demonstrates that improving the training strategy can significantly increase the realism and utility of synthetic healthcare data. It reinforces the importance of GAN-based methods for medical tabular datasets.