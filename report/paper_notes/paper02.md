# Paper 02

## Title

Synthetic data generation methods in healthcare: A review

## Authors

Vasileios C. Pezoulas et al.

## Journal

Informatics in Medicine Unlocked

## Year

2024

## Main Objective

This review analyzes synthetic data generation methods in healthcare and explains how synthetic data can address data scarcity, privacy concerns, and the need for larger datasets for artificial intelligence applications.

## Problem Addressed

Healthcare data are often difficult to access because of privacy regulations, ethical constraints, limited sample sizes, and the sensitivity of patient information. Synthetic data generation is presented as a possible solution because it can create artificial datasets that preserve useful statistical properties without directly exposing real patient records.

## Data Types Discussed

- Tabular data
- Medical imaging data
- Radiomics data
- Time-series data
- Omics data
- Multimodal data

## Methods Reviewed

- Statistical methods
- Probabilistic methods
- Machine learning methods
- Deep learning methods
- GAN-based models
- Variational Autoencoders
- Hybrid approaches

## Main Contributions

- Provides a broad overview of synthetic data generation methods in healthcare.
- Discusses the role of synthetic data in medical research and artificial intelligence.
- Explains the importance of balancing data utility and privacy preservation.
- Reviews different healthcare data modalities, including tabular and imaging data.
- Highlights challenges related to validation, reliability, privacy, and clinical usefulness.

## Advantages

- The paper gives a comprehensive healthcare-focused overview.
- It explains why synthetic data are useful in medical AI.
- It supports the motivation of using synthetic data when real patient data are limited or sensitive.
- It helps justify the use of synthetic data generation techniques in this thesis.

## Limitations

- The paper is a review and does not introduce a new model.
- It covers many types of healthcare data, so it is broader than this thesis, which focuses mainly on tabular data.
- It does not provide a direct implementation of CTGAN, TVAE, or Gaussian Copula on the Stroke Prediction Dataset.

## Why is this paper important for my thesis?

This paper is important because it provides the healthcare context for the thesis. It explains why synthetic healthcare data are useful, especially for privacy preservation, data sharing, and artificial intelligence training. Since my project focuses on generating synthetic tabular healthcare data, this review supports the motivation behind using methods such as CTGAN, TVAE, and Gaussian Copula.

## Personal Notes

This paper helped me understand that synthetic healthcare data generation is not only a technical problem but also a privacy and data access problem. It also confirmed that evaluating synthetic data requires considering both utility and privacy, which will be important later when comparing CTGAN, TVAE, and Gaussian Copula.