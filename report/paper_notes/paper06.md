# Paper 06

## Title

Generating Multi-label Discrete Patient Records using Generative Adversarial Networks

## Authors

Edward Choi, Siddharth Biswal, Bradley Malin, Jon Duke, Walter F. Stewart, Jimeng Sun

## Year

2017

## Source

Proceedings of Machine Learning for Healthcare (MLHC)

---

# Main Objective

The paper introduces MedGAN, one of the first deep learning models specifically designed to generate realistic synthetic Electronic Health Records (EHR). The goal is to enable healthcare data sharing while preserving patient privacy.

---

# Problem Addressed

Healthcare datasets are highly sensitive because they contain personal medical information. Access to Electronic Health Records is often restricted due to privacy regulations, making medical research difficult.

Traditional GANs also struggle with high-dimensional discrete medical data.

---

# Proposed Method

The authors propose MedGAN, which combines:

- An Autoencoder
- A Generative Adversarial Network (GAN)
- Minibatch Averaging
- Batch Normalization
- Shortcut Connections

The Autoencoder first learns a compact representation of patient records, and the GAN generates new realistic synthetic records in the latent space.

---

# Dataset

The model is evaluated using Electronic Health Records (EHR) containing binary and count variables representing diagnoses, medications, and medical procedures.

---

# Evaluation

The generated synthetic records are evaluated using:

- Distribution similarity
- Predictive modeling performance
- Medical expert review
- Privacy analysis

The authors also evaluate identity disclosure risk and attribute disclosure risk.

---

# Main Results

MedGAN successfully generates realistic synthetic patient records while preserving important statistical properties.

Machine learning models trained on synthetic data achieve performance close to those trained on real data.

The privacy analysis shows a limited risk of patient re-identification.

---

# Advantages

- Designed specifically for healthcare data.
- Generates high-dimensional discrete patient records.
- Preserves statistical properties.
- Supports privacy-preserving data sharing.
- Improves collaboration between healthcare institutions.

---

# Limitations

- Mainly supports discrete variables.
- Does not model continuous medical variables efficiently.
- Training becomes more difficult on very large datasets.

---

# Relation to My Thesis

MedGAN is an important baseline for synthetic healthcare data generation. It represents one of the earliest healthcare-specific generative models and provides a useful comparison with newer methods such as CTGAN, Tab-VAE, Copula-based models, and discGAN.

---

# Personal Notes

MedGAN is considered one of the pioneering works in synthetic healthcare data generation. Although newer models achieve better performance, MedGAN remains a fundamental reference because it introduced the idea of combining an Autoencoder with a GAN to generate realistic Electronic Health Records while maintaining patient privacy.