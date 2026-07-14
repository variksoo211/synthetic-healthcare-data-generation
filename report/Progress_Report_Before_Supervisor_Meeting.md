# Thesis Preparation Notes

**Student:** Youssef Aidi

**Master's Degree:** Computer Science and Digital Innovation

**Supervisor:** Prof. Sara Montagna

**Thesis Topic:**
Synthetic Healthcare Data Generation from Clinical Data Models

---

# 1. Selected Dataset

## Dataset Name

Healthcare Stroke Dataset

## Source

Kaggle

## Dataset Description

The Healthcare Stroke Dataset contains demographic information, medical history, lifestyle factors, and a binary target variable indicating whether a patient has experienced a stroke.

The dataset is suitable for machine learning and synthetic data generation because it contains both numerical and categorical variables with realistic healthcare characteristics.

---

## Main Features

- Gender
- Age
- Hypertension
- Heart Disease
- Ever Married
- Work Type
- Residence Type
- Average Glucose Level
- BMI
- Smoking Status
- Stroke (Target)

---

## Why this Dataset?

The dataset was selected because:

- It is publicly available.
- It contains realistic healthcare information.
- It includes both numerical and categorical variables.
- It is commonly used in healthcare machine learning research.
- It is appropriate for evaluating synthetic healthcare data generation methods.

---

# 2. Literature Review

A literature review was conducted to understand the current state of synthetic healthcare data generation.

Ten scientific papers were reviewed and summarized.

---

## Paper 01

### Topic

CTGAN

### Main Contribution

Introduced Conditional Tabular GAN for generating realistic synthetic tabular datasets with mixed continuous and categorical variables.

### Important Points

- Conditional Generator
- Mixed Data Types
- Statistical Fidelity
- Machine Learning Utility

---

## Paper 02

### Topic

Healthcare Synthetic Data Review

### Main Contribution

Provides a comprehensive review of synthetic healthcare data generation techniques, applications, challenges, and future research directions.

### Important Points

- Privacy Protection
- Healthcare Applications
- Existing Challenges
- Future Directions

---

## Paper 03

### Topic

Copula-based Synthetic Data Generation

### Main Contribution

Explains probabilistic approaches for modeling dependencies between variables using Gaussian Copulas.

### Important Points

- Statistical Modeling
- Correlation Preservation
- Efficient Generation
- Easy Interpretation

---

## Paper 04

### Topic

Tab-VAE

### Main Contribution

Introduces a Variational Autoencoder specifically designed for tabular datasets.

### Important Points

- Latent Representation
- Stable Training
- Mixed Variables
- Synthetic Tabular Data

---

## Paper 05

### Topic

discGAN

### Main Contribution

Improves GAN training for tabular data using distributed conditional generation.

### Important Points

- Better Data Utility
- Improved Diversity
- Stable GAN Training

---

## Paper 06

### Topic

MedGAN

### Main Contribution

One of the first GAN models specifically developed for Electronic Health Records (EHR).

### Important Points

- Healthcare-specific GAN
- Electronic Health Records
- Privacy Preservation
- Autoencoder + GAN

---

## Paper 07

### Topic

CTAB-GAN+

### Main Contribution

Improves CTGAN by introducing downstream learning objectives and Differential Privacy.

### Important Points

- Better Utility
- Differential Privacy
- Improved GAN Training
- Mixed Data Types

---

## Paper 08

### Topic

Evaluation Framework for Synthetic Data

### Main Contribution

Introduces a statistical framework for evaluating synthetic data generation models using multiple quality metrics.

### Important Points

- Statistical Similarity
- Machine Learning Utility
- Novelty
- Domain Classifier
- Statistical Ranking

---

## Paper 09

### Topic

Healthcare Quality Assessment Framework

### Main Contribution

Proposes a comprehensive framework for evaluating synthetic healthcare datasets.

### Important Points

Five Quality Dimensions:

- Similarity
- Usability
- Privacy
- Fairness
- Carbon Footprint

---

## Paper 10

### Topic

SynthCity Framework

### Main Contribution

Introduces an open-source framework for generating, benchmarking, and evaluating synthetic datasets.

### Important Points

- Modular Architecture
- Benchmarking
- Evaluation Metrics
- Multiple Data Modalities

---

# 3. Main Techniques Identified

After reviewing the literature, the following techniques were identified as the most relevant for synthetic healthcare data generation.

## Statistical Methods

- Gaussian Copula

---

## Deep Learning Methods

- MedGAN
- CTGAN
- Tab-VAE
- CTAB-GAN+
- discGAN

---

## Evaluation Methods

- Statistical Similarity
- Machine Learning Utility
- Privacy Evaluation
- Fairness Evaluation
- Domain Classifier
- Novelty Analysis
- Distribution Comparison

---

# 4. Models Planned for the Thesis

Based on the literature review and the characteristics of the selected dataset, the following models are planned for implementation and comparison:

## Model 1

Gaussian Copula

Reason:

Classical statistical baseline for tabular synthetic data generation.

---

## Model 2

CTGAN

Reason:

One of the most widely used deep learning models for synthetic tabular healthcare data.

---

## Model 3

TVAE (Tabular Variational Autoencoder)

Reason:

Provides stable probabilistic generation and serves as a strong baseline for comparison with GAN-based methods.

---

## Planned Comparison

The generated synthetic datasets will be compared using:

- Statistical Similarity
- Data Distribution
- Machine Learning Utility
- Data Quality Metrics

The final selection of models and evaluation metrics will be confirmed after discussion with the thesis supervisor.

---

# 5. Questions for the Supervisor

## Dataset

- Is the selected Healthcare Stroke Dataset appropriate for the thesis?

---

## Models

- Should I compare only Gaussian Copula, CTGAN, and TVAE?

- Would you recommend including additional models such as MedGAN or CTAB-GAN+?

---

## Evaluation

- Which evaluation metrics would you recommend for comparing the generated datasets?

- Should privacy evaluation be included in the experiments?

---

## Implementation

- Is the proposed implementation plan suitable for the thesis?

- Should additional preprocessing steps be performed before training the models?

---

## Expected Outcome

- What level of experimental analysis do you expect for the final thesis?

- Are there any additional requirements or recommendations before starting the implementation phase?

---

# Current Progress

## Completed

- Dataset selection
- Initial dataset exploration
- Literature review (10 scientific papers)
- Research notes for all reviewed papers
- Identification of relevant synthetic data generation techniques

---

## Next Step

After meeting with the supervisor:

- Confirm the selected models.
- Implement the synthetic data generation methods.
- Compare their performances.
- Analyze the experimental results.
- Write the final thesis.