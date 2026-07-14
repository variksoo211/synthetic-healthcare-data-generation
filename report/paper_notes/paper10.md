# Paper 10

## Title

Synthcity: Facilitating Innovative Use Cases of Synthetic Data in Different Data Modalities

## Authors

Zhoazhi Qian,
Bogdan-Constantin Cebere,
Mihaela van der Schaar

## Year

2023

## Source

arXiv

---

# Main Objective

The paper introduces SynthCity, an open-source software framework that provides a unified platform for generating, evaluating, and benchmarking synthetic data across different data modalities.

Its goal is to simplify the adoption of synthetic data technologies by providing a modular and extensible framework for researchers and practitioners.

---

# Problem Addressed

Synthetic data research has produced many generation models, but most implementations are isolated, difficult to compare, and limited to specific use cases.

Researchers often face challenges such as:

- Different software implementations.
- Lack of interoperability.
- Limited benchmarking tools.
- Difficulty comparing multiple synthetic data generators.
- Different data modalities requiring different approaches.

---

# Proposed Solution

The authors developed SynthCity, an open-source framework that integrates multiple synthetic data generators into a single platform.

The framework supports:

- Synthetic data generation.
- Model benchmarking.
- Privacy evaluation.
- Fairness evaluation.
- Data augmentation.
- Utility evaluation.

---

# Supported Data Modalities

SynthCity supports multiple types of datasets, including:

- Static tabular data.
- Regular time series.
- Irregular time series.
- Survival (censored) data.
- Multi-source datasets.
- Composite datasets.

---

# Supported Use Cases

The framework is designed for several machine learning applications:

- Privacy-preserving data sharing.
- Machine learning fairness.
- Data augmentation.
- Synthetic data generation.
- Benchmarking.
- Research experimentation.

---

# SynthCity Workflow

The standard workflow consists of four main steps:

1. Load the dataset using the DataLoader.
2. Train a synthetic data generator through the Plugin interface.
3. Generate synthetic data.
4. Evaluate the generated data using built-in evaluation metrics.

---

# Framework Components

## DataLoader

Provides a unified interface for loading different data modalities.

---

## Plugin System

Each synthetic data generator is implemented as a plugin.

Examples include different GANs, VAEs, Bayesian models, and statistical generators.

---

## Metrics Module

The framework evaluates synthetic datasets using metrics related to:

- Fidelity
- Utility
- Privacy

---

## Benchmark Module

Allows automatic comparison between multiple synthetic data generators using the same evaluation pipeline.

---

# Main Contributions

- Unified synthetic data platform.
- Modular architecture.
- Large collection of generation models.
- Integrated benchmarking.
- Built-in evaluation metrics.
- Open-source implementation.
- Easy extensibility for future research.

---

# Advantages

- Supports many data modalities.
- Modular and extensible design.
- Facilitates fair comparison between models.
- Includes evaluation tools.
- Open-source and actively maintained.
- Useful for both research and practical applications.

---

# Limitations

- Focuses mainly on software infrastructure rather than proposing a new generation algorithm.
- Performance still depends on the selected synthetic data generator.
- Requires familiarity with Python and machine learning workflows.

---

# Relation to My Thesis

This paper is highly relevant because my thesis compares different synthetic healthcare data generation methods.

Although SynthCity is not itself a generation model, it provides a unified framework capable of implementing, evaluating, and benchmarking several models such as CTGAN, TVAE, Gaussian Copula, and other synthetic data generators.

The evaluation workflow presented in this paper may be useful during the implementation and comparison phase of my thesis.

---

# Personal Notes

SynthCity represents an important contribution to synthetic data research because it standardizes the complete workflow of synthetic data generation and evaluation.

Instead of introducing a new algorithm, it provides researchers with a flexible platform for testing multiple synthetic data generators under the same experimental conditions, making research more reproducible and comparable.
