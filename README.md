# 🎗️ Breast Cancer Prediction

A machine learning project that predicts whether a breast tumor is **malignant or benign** using the Wisconsin Diagnostic Breast Cancer dataset. Three classification models are trained and compared: Logistic Regression, Random Forest, and Support Vector Machine (SVM).

📄 See the full project report: [Breast_Cancer_Prediction_Portfolio_Project.pdf](Breast_Cancer_Prediction_Portfolio_Project.pdf)

---

## 📋 Project Overview

Breast cancer is one of the most common cancers among women worldwide. Early detection plays a significant role in improving treatment outcomes and survival rates. This project applies supervised machine learning techniques to classify tumors based on features extracted from digitized images of breast mass cell nuclei.

**Authors:** Jayant Manem and Mahitha Bodicherla

---

## 📁 Repository Structure

```
breast-cancer-prediction/
│
├── BreastCancer_Prediction.ipynb              # Main Jupyter notebook
├── breastcancer_prediction.py                 # Python script version
├── cancer.csv                                 # Dataset (Wisconsin Diagnostic)
├── Breast_Cancer_Prediction_Portfolio_Project.pdf  # Full project report
└── README.md
```

---

## 📊 Dataset

**Wisconsin Diagnostic Breast Cancer (WDBC)**

- 569 samples: 357 benign, 212 malignant
- Each sample is labeled as **Malignant (M)** or **Benign (B)**
- 30 numeric features computed from digitized images of cell nuclei
- Features used: radius, texture, perimeter, area, smoothness, compactness, concavity, concave points, symmetry, and fractal dimension (mean values only)

---

## 🔍 Exploratory Data Analysis

Before modeling, the dataset was cleaned and explored:
- Dropped non-informative columns (`id`, `Unnamed: 32`) and redundant columns (all `*_se` and `*_worst` columns)
- Checked for missing and duplicate values
- Visualized the distribution of malignant vs. benign diagnoses
- Final feature set: 11 columns (diagnosis + 10 mean features)

---

## 🤖 Models Used

| Model | Description |
|---|---|
| Logistic Regression | Baseline linear classifier with threshold tuning |
| Random Forest | Ensemble model with feature importance analysis |
| SVM | Support Vector Machine with linear kernel |

All models used a 70/30 train-test split with StandardScaler normalization.

---

## 📈 Results

| Model | Accuracy | Correctly Diagnosed | Incorrectly Diagnosed |
|---|---|---|---|
| Logistic Regression | 94.7% | 162 | 9 |
| Random Forest | 93.5% | 160 | 11 |
| **SVM** ✅ | **95.3%** | **163** | **8** |

**SVM achieved the highest accuracy** with strong precision and recall across both classes.

Feature importance analysis (Random Forest) identified **concavity**, **radius**, and **perimeter** as the most predictive features.

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/breast-cancer-prediction.git
cd breast-cancer-prediction
```

### 2. Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
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

---

## 🔮 Future Work

- Explore deep learning approaches (e.g., neural networks with TensorFlow or PyTorch)
- Incorporate richer clinical and demographic data
- Deploy the model as a real-time web or API tool for healthcare integration
- Apply explainability techniques like SHAP or LIME for transparent predictions
- Hyperparameter tuning and cross-validation for improved generalization

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
