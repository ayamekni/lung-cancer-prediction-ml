# 🫁 Lung Cancer Prediction using Machine Learning  

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Imbalanced-Learn](https://img.shields.io/badge/imbalanced--learn-FF6F00?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/EDUCATIONAL%20ONLY-NOT%20FOR%20MEDICAL%20USE-critical?style=for-the-badge)

> **Medical Disclaimer**  
> This project is **for study/education only**. It is **not a medical device**, **not validated clinically**, and **must not be used for diagnosis, treatment, or patient decision-making**. Any insights are illustrative and based on a public survey dataset—not on clinical data.

---

## 📖 Project Overview  

This notebook demonstrates a complete ML workflow to explore whether survey features can **predict lung-cancer labels**.  
It covers:  
- 🔹 Data cleaning & preprocessing  
- 🔹 Exploratory Data Analysis (EDA)  
- 🔹 Feature engineering  
- 🔹 Handling class imbalance with **ADASYN**  
- 🔹 Model training & evaluation

> **Scope & Limitations**  
> - The dataset is survey-based and may include bias/noise; it **does not** represent clinical ground truth.  
> - Results are **not generalizable** to medical settings without rigorous clinical validation, calibration, and regulatory review.

---

## 📂 Dataset  

- File: `survey_lung_cancer.csv`  
- Example features: Age, Gender, Smoking, Wheezing, Coughing, Fatigue, etc.  
- Target: `LUNG_CANCER` (Yes/No)

---

## ✨ Key Steps  

### 1) 🧹 Data Cleaning & Preprocessing  
- Duplicate checks, missing-value checks  
- Label encoding for categorical variables

### 2) 📊 Exploratory Data Analysis  
- Target distribution  
- Feature–outcome plots (e.g., Smoking, Age, Gender, Symptoms)  
- Correlation heatmap

### 3) 🛠 Feature Engineering  
- Dropped weak features per EDA  
- Created `ANXYELFIN` = Anxiety × Yellow_Fingers

### 4) ⚖️ Class Imbalance  
- **ADASYN** used to rebalance classes

### 5) ✂️ Split  
- Train/Test = 80/20 (fixed random seed)

### 6) 🤖 Modeling & Evaluation  
- Models (e.g., Logistic Regression, Random Forest)  
- Metrics: accuracy, confusion matrix, classification report

---

## 🚀 How to Run  

```bash
# Clone
git clone https://github.com/ayamekni/Lung-Cancer-Prediction-ML.git
cd Lung-Cancer-Prediction-ML

# Launch
jupyter notebook Lung_cancer_predection_ML.ipynb
