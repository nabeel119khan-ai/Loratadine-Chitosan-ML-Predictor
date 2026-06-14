# 💊 Loratadine-Chitosan-ML-Predictor

![Project Banner](https://github.com/nabeel119khan-ai/Loratadine-Chitosan-ML-Predictor/blob/main/Screenshot%202026-06-07%20154026.png)

---

**🚀 AI-Powered Drug Release Prediction Framework**

**Predicting cumulative release of Loratadine from**  
**Chitosan Hydrogel • Ethyl Cellulose Nanosponge • Microsponge Matrices**

---

### 🏆 **Major Breakthrough**
**SVR (RBF Kernel)** achieves **Test R² = 0.992** — **~5× better** than the classical **Korsmeyer-Peppas model (1983)** (R² = 0.780)

Trained on **352 real experimental dissolution data points** from literature.

---

### 📊 Performance Comparison

| Model                      | Test R²   | MAE (%) | RMSE (%) |
|----------------------------|-----------|---------|----------|
| **SVR (RBF)**              | **0.992** | **1.95**| **2.41** |
| Gradient Boosting          | 0.989     | 2.10    | 2.65     |
| PyTorch Neural Network     | 0.985     | 2.40    | 3.01     |
| Random Forest              | 0.970     | 3.20    | 4.10     |
| **Korsmeyer-Peppas (1983)**| 0.780     | 8.50    | 10.20    |

**ML models significantly outperform the 40-year-old equation ✅**

---

### ⚗️ Smart Domain-Informed Features
- **Polymer-to-Drug Ratio** (Higuchi matrix theory)
- **Time × pH Interaction** (Peppas-Sahlin dynamics)
- **pH Deviation from Chitosan pKa (~6.5)**

**SHAP analysis** shows the model naturally rediscovered real polymer physics and pharmaceutical principles.

---

### Why This Project Matters
This work demonstrates how **Chemistry + Modern AI** can accelerate formulation development, reduce costly lab experiments, and improve controlled drug release systems.

**Ideal for researchers in** Drug Delivery, Chemoinformatics, Green Chemistry, and Pharmaceutical Sciences.

---

### 📁 What's Inside
- `ml_paper_nabeel_FINAL.ipynb` — Complete reproducible Jupyter Notebook
- Full data processing, modeling, and SHAP explainability
- All result plots and screenshots

**👉 Open Notebook:** [ml_paper_nabeel_FINAL.ipynb](ml_paper_nabeel_FINAL.ipynb)

---

**⭐ Star this repo if you're working in Pharma AI or Drug Delivery!**  
It helps other researchers find this work.

---

**Made with ❤️ by**  
**Nabeel Khan**  
5th Semester BS Chemistry Student  
University of Sargodha, Pakistan  
Passionate about **AI for Pharmaceutical Sciences**

---

**Topics:** `machine-learning` `drug-delivery` `chemoinformatics` `controlled-release` `pharmaceutical-sciences` `shap` `pytorch` `green-chemistry`
