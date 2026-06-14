# 💊 Loratadine-Chitosan-ML-Predictor

**AI-Powered Prediction of Loratadine Drug Release from Advanced Polymer Matrices**

![Project Banner](https://github.com/nabeel119khan-ai/Loratadine-Chitosan-ML-Predictor/blob/main/Screenshot%202026-06-07%20154026.png)

---

### 🚀 **Key Achievement**
**SVR (RBF Kernel)** achieves **Test R² = 0.992** — beating the classical **Korsmeyer-Peppas model (1983)** by **~5× lower error**.

This project proves that modern Machine Learning + smart chemistry features can significantly outperform 40-year-old equations in **controlled drug release** prediction.

---

### 📊 Results at a Glance

| Model                    | Test R²   | MAE (%) | RMSE (%) |
|--------------------------|-----------|---------|----------|
| **SVR (RBF)**            | **0.992** | **1.95**| **2.41** |
| Gradient Boosting        | 0.989     | 2.10    | 2.65     |
| PyTorch Neural Network   | 0.985     | 2.40    | 3.01     |
| Random Forest            | 0.970     | 3.20    | 4.10     |
| **Korsmeyer-Peppas**     | 0.780     | 8.50    | 10.20    |

**352 real experimental data points** from multiple literature sources.

---

### ⚗️ Smart Domain-Informed Features
- **Polymer-to-Drug Ratio** (Higuchi matrix theory)
- **Time × pH Interaction** (Peppas-Sahlin dynamics)
- **pH Deviation from Chitosan pKa (~6.5)**

SHAP analysis confirms the model independently rediscovered real polymer physics.

---

### Why This Project Matters
Traditional pharmaceutical models are limited. This work shows how **AI + Chemistry knowledge** can accelerate formulation development, reduce experiments, and improve controlled-release drug design.

**Perfect for researchers in:**
- Drug Delivery
- Chemoinformatics
- Green Chemistry
- Pharmaceutical Sciences

---

### 📁 What's Inside
- `ml_paper_nabeel_FINAL.ipynb` → Full reproducible notebook
- Complete data processing + modeling pipeline
- SHAP explanations + performance plots
- All screenshots of results

---

**👉 Open the Notebook:** [ml_paper_nabeel_FINAL.ipynb](ml_paper_nabeel_FINAL.ipynb)

---

**⭐ If you find this useful, please star the repo!**  
It helps other researchers discover this work.

---

**Made by**  
**Nabeel Khan**  
5th Semester BS Chemistry Student  
University of Sargodha, Pakistan  
Passionate about **AI for Pharmaceutical Sciences**

---

**Topics:** `machine-learning` `drug-delivery` `chemoinformatics` `controlled-release` `pharmaceutical-sciences` `shap` `pytorch` `green-chemistry`
