# Students-Performance-Evaluation
ML-based student academic performance prediction using MLP, SVM, KNN, LR, NB and Decision Tree with SHAP explainability on the SAPData dataset.

# 🎓 Student Academic Performance Prediction

A Jupyter Notebook implementation of the research paper:
> *"Evaluation of Machine Learning Models in Student Academic Performance Prediction"*
> — Sandeepa A.G.R. & Mohottala S. | ICARC 2025 | IEEE

---

## 📌 Problem Statement
Predicting a student's academic performance level — **Low (L)**, **Middle (M)**, 
or **High (H)** — based on behavioral, demographic, academic, and parental features 
collected from a Learning Management System (Kalboard 360).

---

## 📦 Dataset
- **Name:** xAPI-Edu-Data (SAPData)
- **Source:** [Kaggle — aljarah/xAPI-Edu-Data](https://www.kaggle.com/datasets/aljarah/xAPI-Edu-Data)
- **Size:** 480 records, 16 features
- **Target Classes:** L (Low) / M (Middle) / H (High)

---

## 🤖 Models Implemented
| Model | Library |
|-------|---------|
| Multi-Layer Perceptron (MLP) | sklearn |
| Support Vector Machine (SVM) | sklearn |
| K-Nearest Neighbors (KNN) | sklearn |
| Logistic Regression (LR) | sklearn |
| Naive Bayes (NB) | sklearn |
| Decision Tree (DT) | sklearn |

---

## 🧪 Evaluation Methods
- Repeated Hold-Out Validation (RHO) — 90:10 split
- 10-Fold Stratified Cross Validation
- Metrics: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## 🔍 Explainability
SHAP (SHapley Additive Explanations) was used to interpret the best 
performing MLP model and validate the feature selection approach.

---

## 🛠️ Tools & Libraries
Python | Jupyter Notebook | Scikit-learn | Pandas | NumPy | Seaborn | Matplotlib | SHAP

---

## 📁 Repository Structure
```
student-performance-prediction/
│
├── student_performance_prediction.ipynb   ← main notebook
├── xAPI-Edu-Data.csv                       ← dataset
└── README.md
```

---

## 📊 Key Results
- **MLP achieved the best average accuracy** across both evaluation protocols
- **Behavioral features** (student absence, raised hands, visited resources) 
  were the most dominant predictors identified via SHAP
- Feature selection (FS protocol) consistently outperformed using all features (WBF)
