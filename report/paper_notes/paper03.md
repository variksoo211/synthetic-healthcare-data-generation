# Paper 03

## Title

Generation and Simulation of Synthetic Datasets with Copulas

## Authors

(To be completed from the paper)

## Source

arXiv

## Year

2022

## Main Objective

The paper presents copula-based methods for generating synthetic tabular datasets while preserving the statistical relationships among variables.

## Problem Addressed

Real datasets may contain sensitive or confidential information and therefore cannot always be freely shared. Copula-based synthetic data generation offers a statistical approach for creating artificial datasets that maintain important properties of the original data.

## Proposed Method

Gaussian Copula

## How the Model Works

1. Estimate the probability distribution of each variable.
2. Transform variables into a Gaussian latent space.
3. Learn the dependency structure among variables using a Gaussian Copula.
4. Generate new synthetic samples.
5. Transform the generated samples back to the original data space.

## Main Contributions

- Presents copula-based synthetic data generation.
- Explains how dependencies among variables can be modeled.
- Shows how synthetic datasets can preserve statistical properties.
- Provides a statistical alternative to deep learning methods.

## Advantages

- Fast training.
- Easy to interpret.
- Low computational cost.
- Suitable for structured tabular datasets.
- Useful as a baseline model.

## Limitations

- May not capture complex nonlinear relationships.
- Assumes dependencies can be represented through copula-based statistical relationships.
- Usually less flexible than deep learning approaches such as CTGAN and TVAE.

## Evaluation

The synthetic data can be evaluated by comparing distributions, statistical similarity, correlations, and machine learning utility between the original and generated datasets.

## Why is this paper important for my thesis?

This paper is important because Gaussian Copula will be used as the baseline statistical model in my thesis. Its performance will be compared with deep learning approaches such as CTGAN and TVAE on the Stroke Prediction Dataset.

## Personal Notes

This paper helped me understand why Gaussian Copula is a good baseline for synthetic tabular data generation. It is simpler and faster than deep learning models, but it may be less accurate when the dataset contains complex nonlinear relationships.