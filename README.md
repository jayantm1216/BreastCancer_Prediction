# BreastCancer_Prediction
Breast cancer classification using Logistic Regression, Random Forest, and SVM on the Wisconsin Diagnostic dataset.

# 🎗️ Breast Cancer Prediction

A machine learning project that predicts whether a breast tumor is **malignant or benign** using the Wisconsin Diagnostic Breast Cancer dataset. Three classification models are trained and compared: Logistic Regression, Random Forest, and Support Vector Machine (SVM).

---

## 📋 Project Overview

Breast cancer is one of the most common cancers worldwide. Early and accurate diagnosis is critical for effective treatment. This project applies supervised machine learning techniques to classify tumors based on features extracted from digitized images of breast mass cell nuclei.

---

## 📁 Repository Structure

```
breast-cancer-prediction/
│
├── BreastCancer_Prediction.ipynb   # Main Jupyter notebook
├── breastcancer_prediction.py      # Python script version
├── cancer.csv                      # Dataset (Wisconsin Diagnostic)
└── README.md
```

---

## 📊 Dataset

**Wisconsin Diagnostic Breast Cancer (WDBC)**

- 569 samples, 30 numeric features
- Each sample is labeled as **Malignant (M)** or **Benign (B)**
- Features include: radius, texture, perimeter, area, smoothness, compactness, concavity, and more — computed from digitized images of cell nuclei

---

## 🤖 Models Used

| Model | Description |
|---|---|
| Logistic Regression | Baseline linear classifier with threshold tuning |
| Random Forest | Ensemble model with feature importance analysis |
| SVM | Support Vector Machine with linear kernel |

---

## 📈 Evaluation Metrics

Each model is evaluated using:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/breast-cancer-prediction.git
cd breast-cancer-prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
Open `BreastCancer_Prediction.ipynb` in Jupyter Notebook or JupyterLab and run all cells.

---

## 🛠️ Requirements

- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn

Install all at once:
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## 📌 Results Summary

Three models were trained and compared. Random Forest and SVM both achieved high accuracy on the test set, with Logistic Regression serving as a strong baseline. Feature importance analysis revealed that **concavity**, **radius**, and **perimeter** are among the most predictive features.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
