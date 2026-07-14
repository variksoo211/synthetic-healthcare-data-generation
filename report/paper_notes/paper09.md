# Paper 09 Notes

**Title**
Can I Trust My Fake Data? A Comprehensive Quality Assessment Framework for Synthetic Tabular Data in Healthcare

**Authors**
Vibeke Binz Vallevik et al.

**Year**
2024

**Type**
Literature Review + Conceptual Framework

---

# Research Problem

Synthetic healthcare data is increasingly used to overcome privacy restrictions and the limited availability of real medical datasets.

Although many synthetic data generators exist, there is still no standardized framework for evaluating whether synthetic datasets are trustworthy enough for healthcare applications.

Different studies use different evaluation metrics, making comparisons difficult and creating uncertainty about synthetic data quality.

---

# Main Objective

The objective of this paper is to propose a comprehensive quality assessment framework for synthetic tabular healthcare data.

The framework helps researchers evaluate synthetic datasets consistently before using them for AI model development or clinical applications.

---

# Methodology

The authors conducted a systematic literature review following the PRISMA methodology.

They reviewed studies published between 2019 and 2023 related to synthetic tabular healthcare data generated using deep generative models.

The review analyzed:

- Quality evaluation metrics
- Existing evaluation frameworks
- Privacy assessment methods
- Utility evaluation
- Fairness evaluation
- Computational complexity

The proposed framework was also benchmarked using a real breast cancer dataset from the Dutch National Cancer Registry (DNCR).

---

# Proposed Quality Framework

The paper introduces five main quality dimensions.

## 1. Similarity

Measures how closely synthetic data matches the statistical properties of the original dataset.

Examples include:

- Distribution similarity
- Correlation preservation
- Statistical tests
- Distance metrics

---

## 2. Usability

Evaluates whether synthetic data can replace real data for downstream machine learning tasks.

Typical evaluation:

- Train on Synthetic, Test on Real (TSTR)
- Classification accuracy
- F1-score
- AUROC
- Precision
- Recall

---

## 3. Privacy

Ensures synthetic data does not leak sensitive patient information.

Evaluation methods include:

- Membership Inference Attack
- Attribute Inference Attack
- Differential Privacy
- Privacy Risk Metrics

---

## 4. Fairness

Checks whether synthetic data preserves balanced representation across different demographic groups and avoids amplifying bias.

The paper highlights that fairness is rarely evaluated in existing studies.

---

## 5. Carbon Footprint

Evaluates computational cost and environmental impact.

Metrics include:

- Training time
- Memory consumption
- Computational complexity
- Energy usage

This dimension is almost completely ignored in current literature.

---

# Literature Review Findings

The authors reviewed 94 research papers.

They identified:

- 616 evaluation metrics

Most studies focused only on:

- Statistical similarity
- Machine learning utility

Very few evaluated:

- Privacy
- Fairness
- Carbon footprint

Only one reviewed paper covered all five quality dimensions.

---

# Proposed Evaluation Pipeline

The framework proposes six evaluation stages.

Stage 0:
Problem definition and intended application.

Stage 1:
Evaluate real training data quality.

Stage 2:
Evaluate synthetic data generation process.

Stage 3:
Evaluate synthetic dataset quality.

Stage 4:
Analytical validation using machine learning.

Stage 5:
Clinical validation in real healthcare settings.

Stage 6:
Continuous monitoring after deployment.

---

# Advantages

- Comprehensive quality assessment.
- Standardized evaluation process.
- Includes privacy and fairness.
- Supports regulatory compliance.
- Suitable for healthcare AI.
- Can guide future synthetic data research.

---

# Limitations

- Conceptual framework only.
- Does not propose a new data generation model.
- Fairness metrics remain limited.
- Carbon footprint evaluation is still underdeveloped.

---

# Key Contributions

The paper contributes by:

- Proposing a unified quality evaluation framework.
- Introducing five quality dimensions.
- Defining a six-stage evaluation pipeline.
- Identifying gaps in current evaluation practices.
- Highlighting the importance of fairness and sustainability.

---

# Relation to My Thesis

This paper is highly relevant because my thesis focuses on synthetic healthcare data generation.

It provides a complete framework for evaluating synthetic datasets beyond statistical similarity.

The proposed quality dimensions (Similarity, Usability, Privacy, Fairness, and Carbon Footprint) can be used later to evaluate the synthetic datasets generated during my project.

---

# Personal Notes

This paper is one of the most comprehensive references for synthetic healthcare data evaluation.

Instead of introducing a new generative model, it focuses on answering an important question:

"How can we determine whether synthetic healthcare data is trustworthy?"

The proposed framework can serve as a guideline for selecting appropriate evaluation metrics in future experiments.


