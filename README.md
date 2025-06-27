# 🌍 AICTE Internship Project – Water Quality Prediction (June 2025)

This repository is part of the **AICTE Virtual Internship Program – June 2025**, organized by **Edunet Foundation** under the **Skills4Future** initiative and sponsored by **Shell**. This project uses **Machine Learning (ML)** to predict water quality indicators based on environmental monitoring data.

---

## 🎯 Internship Overview

- **Program**: AICTE Virtual Internship (Cycle 1)  
- **Duration**: June 16 – July 16, 2025  
- **Trainer**: Raghunandan M S (Skills4Future)  
- **Sponsored by**: Shell  
- **Focus Area**: Environmental Analytics & Machine Learning  
- **Project Title**: Water Quality Prediction using AI/ML  

---

## 📁 Repository Structure

Water_Quality_Prediction:
  Week_1: "Data exploration, cleaning, and feature engineering"
  Week_2: "Modeling, training, and predictions"
  dataset: "Raw data files (e.g., PB_All_2000_2021.csv)"
  model: "Trained model files (.pkl)"
  visuals: "Visual outputs and plots"
  README.md: "Project documentation"


---

## 📌 Project Objective

To build a regression model that predicts multiple pollutant concentrations —  
**O₂, NO₃, NO₂, SO₄, PO₄, and Cl⁻** — using historical water quality data from 22 monitoring stations.

---

## ⚙️ Technologies & Skills Used

**Languages & Tools**:
- Python (Jupyter Notebook)
- pandas, numpy, matplotlib, seaborn
- scikit-learn, joblib

**Skills Developed**:
- Data Cleaning & Preprocessing  
- Feature Engineering  
- Exploratory Data Analysis (EDA)  
- MultiOutput Regression Modeling  
- Model Evaluation (MSE, R² Score)  
- Model Serialization & Prediction  

---

## 🔧 Project Breakdown

### ✅ Week 1 – Data Preparation
- Loaded dataset: `PB_All_2000_2021.csv`
- Converted `date` column to datetime
- Extracted `year` and `month`
- Identified missing values
- Selected target pollutant columns

### 🤖 Week 2 – MultiOutput Regression Model
- Dropped rows with missing pollutant data
- Selected `id` and `year` as input features
- Applied OneHotEncoding to station ID
- Trained `MultiOutputRegressor` with `RandomForestRegressor`
- Evaluated model with MSE & R²
- Made predictions for a test station/year
- Saved model and columns using `joblib`

---

## 📊 Model Evaluation

| Pollutant | MSE        | R² Score     |
|-----------|------------|--------------|
| O₂        | 22.21      | -0.01        |
| NO₃       | 18.15      | 0.51         |
| NO₂       | 10.60      | -78.42       |
| SO₄       | 2412.14    | 0.41         |
| PO₄       | 0.38       | 0.32         |
| Cl⁻       | 34882.81   | 0.73         |

---

## 🔍 Sample Prediction Output

Predicted pollutant levels for station `'22'` in **2022**:

- **O₂**: `12.60`  
- **NO₃**: `6.89`  
- **NO₂**: `0.13`  
- **SO₄**: `143.08`  
- **PO₄**: `0.50`  
- **CL**: `67.33`


---

## 💾 Saved Artifacts

- ✅ `pollution_model.pkl` – Trained ML model  [Drive Link : https://drive.google.com/file/d/18RJzu35vyuMgpcAE590u1IaDvHY3-SWq/view?usp=sharing]
- ✅ `model.columns.pkl` – Feature columns used during training  

---

## 📚 Key Learnings

- End-to-end ML workflow on real-world environmental data  
- How to clean, preprocess, and analyze time-series water quality data  
- Building and evaluating multi-output regression models  
- Making forward predictions and saving models for reuse  

---

## 🚀 Future Improvements

- Include additional variables: `NH4`, `Suspended`, `BSK5`
- Try advanced ML algorithms: XGBoost, LightGBM, Neural Nets
- Build a web interface using **Streamlit** or **Flask**
- Deploy prediction API with **FastAPI**

---

## 👤 Author

*Suvetha S*  
Internship Cycle: June 16 – July 16, 2025  

