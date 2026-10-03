# 🫀 Heart Disease Prediction & Classification System

An end-to-end Machine Learning pipeline designed to predict the likelihood of cardiovascular disease based on clinical patient parameters. This project utilizes automated exploratory data analysis via **DataPrep** and builds a predictive classifier using **Logistic Regression**.

---

## 📌 Project Overview
Cardiovascular diseases (CVDs) are among the leading causes of mortality globally. Early detection through predictive healthcare modeling helps clinicians identify high-risk individuals. This repository contains:
1. Automated Exploratory Data Analysis (EDA) using the `dataprep` framework.
2. Clinical statistical profiling and missing value validation.
3. Classification modeling using **Scikit-learn's Logistic Regression**.

---

## 📊 Dataset Features
The model evaluates the following clinical features (`heart.csv`):

| Feature | Description |
|---|---|
| `age` | Age of the patient (years) |
| `sex` | Biological sex (`1` = male, `0` = female) |
| `cp` | Chest pain type (typical angina, atypical angina, non-anginal pain, asymptomatic) |
| `trestbps` | Resting blood pressure (in mm Hg on admission to hospital) |
| `chol` | Serum cholesterol level in mg/dl |
| `fbs` | Fasting blood sugar (`> 120 mg/dl`: `1` = true, `0` = false) |
| `restecg` | Resting electrocardiographic results (`0`, `1`, `2`) |
| `thalach` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina (`1` = yes, `0` = no) |
| `oldpeak` | ST depression induced by exercise relative to rest |
| `slope` | Slope of the peak exercise ST segment |
| `ca` | Number of major vessels (`0-3`) colored by fluoroscopy |
| `thal` | Thalassemia status (`1` = normal, `2` = fixed defect, `3` = reversible defect) |
| `target` | Presence of heart disease (`1` = presence, `0` = absence) |

---

## 🛠️ Technology Stack
- **Language**: Python
- **Data Manipulation**: Pandas, NumPy
- **Machine Learning**: Scikit-learn (`LogisticRegression`, `accuracy_score`, `train_test_split`)
- **Automated EDA**: DataPrep (`dataprep.eda`)

---

## 📁 Repository Structure

```text
├── data/
│   └── heart.csv                       # Clinical dataset
├── notebooks/
│   └── Heart_Disease_Prediction.ipynb  # Interactive analysis and training notebook
├── src/
│   ├── data_loader.py                  # Data preprocessing and ingestion
│   ├── model.py                        # Training pipeline
│   └── predict.py                      # Evaluation utilities
├── requirements.txt                    # Environment dependencies
├── .gitignore
└── README.md
