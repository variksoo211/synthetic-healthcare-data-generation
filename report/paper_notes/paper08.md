# Paper 08

## Title

An Evaluation Framework for Synthetic Data Generation Models

## Authors

Ioannis E. Livieris,
Nikos Alimpertis,
George Domalis,
Dimitris Tsakalidis

## Year

2024

## Source

IFIP International Conference on Artificial Intelligence Applications and Innovations (AIAI)

---

# Main Objective

The paper proposes a statistical evaluation framework for comparing synthetic tabular data generation models. Instead of relying on a single metric, it combines multiple evaluation tests with statistical analysis to identify the model that generates the highest-quality synthetic data.

---

# Motivation

Synthetic healthcare datasets must satisfy multiple requirements simultaneously:

- Preserve statistical properties
- Maintain feature relationships
- Protect sensitive information
- Produce realistic samples

The authors point out that many existing evaluation metrics often provide conflicting conclusions, making it difficult to determine which synthetic data generator performs best.

---

# Problem Addressed

Most previous studies evaluate synthetic data using only one or two metrics.

However:

- Different evaluation metrics often rank models differently.
- No universal evaluation methodology exists.
- Researchers need an objective framework to compare synthetic data generators.

---

# Synthetic Data Models Reviewed

The paper reviews several popular tabular data generators:

- Gaussian Copula
- Gaussian Mixture Models (GMM)
- CTGAN
- TVAE
- CopulaGAN

Each model has different strengths and weaknesses depending on the dataset characteristics.

---

# Proposed Evaluation Framework

The framework evaluates every synthetic dataset using multiple complementary tests.

The workflow consists of:

1. Generate synthetic data.
2. Perform data validity checks.
3. Apply several evaluation metrics.
4. Rank all models statistically.
5. Select the best-performing synthetic dataset.

---

# Evaluation Metrics

The framework includes four main evaluation tests.

## 1. Wasserstein / Cramer's V Test

Measures similarity between real and synthetic feature distributions.

Used for:

- Numerical variables
- Categorical variables

Lower distance indicates better quality.

---

## 2. Novelty Test

Measures whether the generator creates new realistic samples instead of simply copying the original dataset.

Higher novelty indicates better diversity.

---

## 3. Domain Classifier Test

A classifier is trained to distinguish real data from synthetic data.

If the classifier cannot distinguish them (AUC close to 0.5), the synthetic data are considered highly realistic.

---

## 4. Anomaly Detection Test

Detects abnormal synthetic samples.

A lower anomaly score indicates that generated records closely follow the real data distribution.

---

# Statistical Analysis

Instead of selecting the model based on a single metric, the framework applies:

- Friedman Aligned-Ranks Test
- Finner Post-hoc Test

These statistical tests determine whether the observed differences between generators are statistically significant.

---

# Experimental Evaluation

The framework was evaluated on two real-world datasets:

- Travel Review Ratings Dataset
- Obesity Risk Dataset

The experiments compared:

- Gaussian Copula
- GMM
- CTGAN
- TVAE
- CopulaGAN

The results demonstrate that no single generator consistently performs best across every dataset.

---

# Main Findings

- Different evaluation metrics may produce conflicting rankings.
- Combining multiple metrics provides a more reliable evaluation.
- Statistical hypothesis testing offers stronger evidence than simple score comparison.
- The proposed framework allows objective comparison of synthetic data generators.

---

# Advantages

- Comprehensive evaluation methodology.
- Flexible and extensible framework.
- Supports unlabeled tabular datasets.
- Uses statistical significance testing.
- Can easily integrate additional evaluation metrics.

---

# Limitations

- Only evaluated tabular datasets.
- Does not introduce a new synthetic data generation model.
- Future work includes image data and additional statistical metrics.

---

# Relation to My Thesis

This paper is highly relevant because my thesis compares several synthetic healthcare data generators, including Gaussian Copula, CTGAN and TVAE.

The proposed evaluation framework provides an excellent methodology for comparing the generated datasets using multiple quality metrics and statistical analysis.

Several evaluation techniques described in this paper can be directly adopted in my experimental analysis.

---

# Personal Notes

This paper is one of the most useful references for my thesis because it explains how synthetic data generators should be evaluated instead of simply presenting generation models.

It will help design the evaluation section of my thesis and justify the comparison between different synthetic healthcare data generation techniques.