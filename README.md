# Testing New Variational Approximations for Bayesian Inference

This repository contains the materials, code, and documentation for my Master’s thesis titled **“Testing New Variational Approximations for Bayesian Inference”**. The thesis explores and compares novel variational approximation methods for Bayesian inference, with applications to both simulated Gaussian models and real medical datasets.

---

## Table of Contents
1. [Introduction](#introduction)  
2. [Problem Setup and Relevant Literature](#problem-setup-and-relevant-literature)  
   - [The Reparametrization Trick](#the-reparametrization-trick)  
   - [Automatic-Differentiation Variational Inference (ADVI)](#automatic-differentiation-variational-inference-advi)  
   - [Deterministic ADVI (DADVI)](#deterministic-advi-dadvi)  
3. [Experiments](#experiments)  
   - [One and Two-Dimensional Variational Families](#one-and-two-dimensional-variational-families)  
   - [Three-Dimensional Gaussian Variational Family](#three-dimensional-gaussian-variational-family)  
   - [Four-Dimensional Gaussian Variational Family](#four-dimensional-gaussian-variational-family)  
   - [Model with Mixture of Gaussians](#model-with-mixture-of-gaussians)  
   - [Application to a Real Medical Dataset](#application-to-a-real-medical-dataset)  
4. [Conclusion](#conclusion)  
5. [Limitations and Future Work](#limitations-and-future-work)  
6. [Appendix](#appendix)  

---

## Introduction
Bayesian inference provides a probabilistic framework for modeling uncertainty. Exact posterior computation is often intractable, especially in high-dimensional or complex models. Variational inference approximates the posterior by optimizing a tractable distribution to be close to the true posterior. This thesis investigates new variational approximations, including deterministic variants, and evaluates their performance on both synthetic and real datasets.

---

## Problem Setup and Relevant Literature
This section presents the theoretical background, relevant literature, and key methods used in the thesis.

### The Reparametrization Trick
A technique to compute gradients for stochastic variables efficiently, essential for variational inference optimization.

### Automatic-Differentiation Variational Inference (ADVI)
Introduces ADVI as a scalable and general-purpose method for approximating posterior distributions.

### Deterministic ADVI (DADVI)
Explores a deterministic variant of ADVI aimed at improving stability and convergence in variational inference.

---

## Experiments
Experiments were conducted on Gaussian models of increasing dimensionality, mixtures of Gaussians, and a real medical dataset to evaluate the practical performance of the methods.

### One and Two-Dimensional Variational Families
- Computation of the true posterior.  
- Comparison of ADVI and DADVI performance.

### Three-Dimensional Gaussian Variational Family
- Posterior approximation and evaluation of ELBO convergence.

### Four-Dimensional Gaussian Variational Family
- High-dimensional posterior estimation and analysis.

### Model with Mixture of Gaussians
- Evaluation of approximations on multimodal posteriors.

### Application to a Real Medical Dataset
- Application of ADVI and DADVI to longitudinal medical data.  
- Assessment of predictive performance and interpretability of results.

---

## Conclusion
Summarizes the findings regarding the accuracy, efficiency, and limitations of the tested variational approximation methods.

---

## Limitations and Future Work
- **Limitations:** High-dimensional posterior estimation, computational constraints, sensitivity to initialization.  
- **Future Work:** Explore alternative variational families, improved optimization strategies, and applications to more complex datasets.

---

## Appendix
Contains visualizations of posterior approximations, mixture models for small sample sizes, and additional diagnostic plots.

---

## Installation
```bash
# Clone the repository
git clone https://github.com/mbethlehem/Masters-Thesis.git
# Navigate to the repository
cd variational-approximations

# Install required Python packages
pip install -r requirements.txt
