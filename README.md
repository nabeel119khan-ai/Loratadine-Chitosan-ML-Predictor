<div align="center">

# 💊 ML Prediction of Loratadine Drug Release
### Chitosan Hydrogel · Ethyl Cellulose Nanosponge · Microsponge Matrices

[![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)](https://python.org)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0-EE4C2C?style=flat-square&logo=pytorch)](https://pytorch.org)
[![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-1.3-F7931E?style=flat-square&logo=scikit-learn)](https://scikit-learn.org)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Status](https://img.shields.io/badge/Manuscript-Under%20Review-orange?style=flat-square)](.)

</div>

---

## 📌 Overview

This repository contains a **complete machine learning framework** for predicting cumulative drug release percentage of **Loratadine** from polymer-based controlled release matrices.

Four ML models — SVR, Random Forest, Gradient Boosting, and a custom PyTorch Neural Network — were trained on **352 dissolution data points** unified from multiple published literature sources. All models were benchmarked against the classical **Korsmeyer-Peppas kinetic equation (1983)**.

> **Key finding:** The best ML model achieves Test R² = 0.992, outperforming the Korsmeyer-Peppas classical model by ΔR² = 0.212 — validated by Wilcoxon signed-rank test (p < 0.05).

---

## 🏆 Results Summary

| Model | Test R² | CV R² (±95% CI) | MAE (%) | RMSE (%) |
|-------|---------|-----------------|---------|----------|
| **SVR (RBF kernel)** | **0.992** | **0.989 ± 0.008** | **1.95** | **2.41** |
| Gradient Boosting | 0.989 | 0.986 ± 0.009 | 2.10 | 2.65 |
| PyTorch Neural Net | 0.985 | N/A | 2.40 | 3.01 |
| Random Forest | 0.970 | 0.967 ± 0.011 | 3.20 | 4.10 |
| **Korsmeyer-Peppas** *(classical baseline)* | 0.780 | — | 8.50 | 10.20 |

**ML significantly outperforms the 40-year-old classical equation ✅**

---

## 🗂️ Dataset

| Property | Value |
|----------|-------|
| **Total data points** | 352 dissolution observations |
| **Matrix systems** | Chitosan hydrogel, Ethyl Cellulose nanosponge, Microsponge |
| **Source** | Multi-paper literature extraction from published dissolution studies |
| **Drug** | Loratadine (MW = 382.88 g/mol, LogP = 5.1, pKa = 4.97) |
| **Target variable** | Cumulative drug release (%) |
| **Time range** | 0.5 – 24 hours |
| **pH conditions** | 1.2, 4.5, 6.8, 7.4 |

---

## ⚗️ Feature Engineering — 3 Domain-Informed Features

### Feature A — Polymer-to-Drug Ratio
```python
polymer_to_drug_ratio = (chitosan_mg + ethyl_cellulose_mg + pva_mg) / (loratadine_mg + 0.001)
```
**Basis:** Higuchi (1963) matrix diffusion. Higher ratio = denser polymer network = reduced diffusion coefficient = slower release.

### Feature B — Time × pH Interaction
```python
time_ph_interaction = time_hours × ph
```
**Basis:** Chitosan pKa ≈ 6.5. Below pKa, protonation drives swelling and accelerated diffusion. This effect scales with time — multiplicative term captures the coupling (Peppas & Sahlin, 1989).

### Feature C — pH Deviation from Chitosan pKa
```python
ph_deviation_from_pka = abs(ph - 6.5)
```
**Basis:** Further pH deviates from pKa in either direction, the more extreme the ionisation-driven swelling response.

**All 3 engineered features ranked in the top 5 SHAP importance scores ✅**

---

## 🧠 SHAP Feature Importance

| Rank | Feature | Mean SHAP | Pharmaceutical Basis |
|------|---------|-----------|----------------------|
| 1 | time_hours | 0.92 | Korsmeyer-Peppas kinetics |
| 2 | time_ph_interaction | 0.71 | Peppas-Sahlin diffusion-relaxation coupling |
| 3 | polymer_to_drug_ratio | 0.48 | Higuchi matrix diffusion |
| 4 | ph | 0.31 | Chitosan polyelectrolyte switching at pKa 6.5 |
| 5 | ph_deviation_from_pka | 0.22 | Ionisation state → swelling magnitude |

> The AI independently rediscovered 40 years of pharmaceutical physics from data alone.

---

## 📁 Repository Structure
