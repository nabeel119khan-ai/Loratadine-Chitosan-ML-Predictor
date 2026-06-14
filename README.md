# 💊 Loratadine-Chitosan-ML-Predictor

![Project Banner](https://github.com/nabeel119khan-ai/Loratadine-Chitosan-ML-Predictor/blob/main/Screenshot%202026-06-07%20154112.png)

---

**🚀 AI-Powered Drug Release Prediction Framework**

**Built with**  
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-FF9F00?style=for-the-badge&logo=scikit-learn&logoColor=white)
**Jupyter Notebook** • **SHAP** • **Pandas** • **Matplotlib**

---

**Predicting cumulative Loratadine release (%) from**  
**Chitosan Hydrogel • Ethyl Cellulose Nanosponge • Microsponge Matrices**

---

### 🏆 **Major Breakthrough**

**SVR (RBF Kernel)** achieves **Test R² = 0.992** — **~5× better** than the classical **Korsmeyer-Peppas model (1983)** (R² = 0.780)

Trained on **352 real experimental dissolution data points** collected from multiple scientific papers.

---

### 📊 Performance Comparison

| Model                      | Test R²   | MAE (%) | RMSE (%) |
|----------------------------|-----------|---------|----------|
| **SVR (RBF)**              | **0.992** | **1.95**| **2.41** |
| Gradient Boosting          | 0.989     | 2.10    | 2.65     |
| PyTorch Neural Network     | 0.985     | 2.40    | 3.01     |
| Random Forest              | 0.970     | 3.20    | 4.10     |
| **Korsmeyer-Peppas (1983)**| 0.780     | 8.50    | 10.20    |

---

### ⚙️ Smart Domain-Informed Features
- **Polymer-to-Drug Ratio** (Higuchi matrix theory)
- **Time × pH Interaction** (Peppas-Sahlin dynamics)
- **pH Deviation from Chitosan pKa (~6.5)**

**SHAP Explainability** confirms the model rediscovered real polymer physics.

---

### Why This Project Matters
This project bridges **traditional pharmaceutical chemistry** with **modern machine learning** to make controlled drug release formulation faster, cheaper, and more predictive.

---

### 📁 What's Inside
- `ml_paper_nabeel_FINAL.ipynb` → Full reproducible Jupyter Notebook
- Complete data unification + modeling pipeline
- PyTorch Neural Network implementation
- All SHAP plots and performance visuals

**👉 [Open Full Notebook](ml_paper_nabeel_FINAL.ipynb)**

---

**⭐ If you like this project, please star it!**  
Helps other researchers and students discover it.

---

**Made with ❤️ by**  
**Nabeel Khan**  
5th Semester BS Chemistry Student  
University of Sargodha, Pakistan  

**Passionate about AI for Pharmaceutical Sciences & Green Chemistry**
