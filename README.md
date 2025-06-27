# 🌍 AICTE Internship Project – Water Quality Prediction (June 2025)

This repository is part of the **AICTE Virtual Internship Program – June 2025**, organized by **Edunet Foundation** under the **Skills4Future** initiative and sponsored by **Shell**. It focuses on applying **Machine Learning** techniques to solve real-world **environmental analytics problems** like water quality forecasting.

---

## 🎯 Internship Overview

- **Program**: AICTE Virtual Internship (Cycle 1)
- **Duration**: June 16 – July 16, 2025 (1 Month)
- **Trainer**: `XXXXXX` (Skills4Future)
- **Sponsored by**: Shell
- **Focus Area**: Environmental Analytics & Machine Learning (Green Skills)
- **Project Title**: Water Quality Prediction using AI/ML

---

## 📁 Repository Structure

Water_Quality_Prediction/
├── Week_1/ # Data exploration, cleaning, and feature engineering
├── Week_2/ # Modeling, training, and predictions
├── dataset/ # Includes PB_All_2000_2021.csv
├── model/ # Saved model .pkl files
├── visuals/ # Plots and prediction outputs
└── README.md # Project documentation


---

## 📌 Project Objective

To build a machine learning model that can predict **multiple water pollutant indicators** (O2, NO3, NO2, SO4, PO4, CL) using data collected from **22 monitoring stations** across different years.

---

## ⚙️ Technologies & Skills Used

- **Python** (Jupyter Notebook)
- **Libraries**: pandas, numpy, matplotlib, seaborn, scikit-learn, joblib
- **Skills Developed**:
  - Exploratory Data Analysis (EDA)
  - Data Cleaning & Preprocessing
  - Multi-output Regression
  - Model Evaluation (MSE, R²)
  - Predictive Modeling
  - Time-based Feature Engineering

---

## 🔧 Project Breakdown

### ✅ Week 1 – Data Understanding & Preprocessing

- Loaded `PB_All_2000_2021.csv` dataset
- Converted `date` column to datetime format
- Extracted features: `year`, `month`
- Selected important pollutants for modeling
- Checked and summarized missing values

### 🤖 Week 2 – MultiOutput Modeling

- Dropped missing values for selected pollutants
- Selected features: `id` (station) and `year`
- Applied one-hot encoding for `id`
- Trained a **MultiOutput RandomForestRegressor**
- Evaluated predictions using **MSE** and **R²**
- Performed sample predictions for new inputs
- Saved model and feature structure using `joblib`

---

## 📊 Evaluation Metrics

Example performance of model on test set:


O2: MSE = 22.21, R² = -0.01
NO3: MSE = 18.15, R² = 0.51
NO2: MSE = 10.60, R² = -78.42
SO4: MSE = 2412.14, R² = 0.41
PO4: MSE = 0.38, R² = 0.32
CL: MSE = 34882.81, R² = 0.73

---

## 🔍 Sample Prediction Output

Predict pollutant levels for a station and year:

```python
Predicted pollutant levels for station '22' in 2022:
 O2: 12.60
 NO3: 6.89
 NO2: 0.13
 SO4: 143.08
 PO4: 0.50
 CL: 67.33

💾 Artifacts Saved
Trained model: pollution_model.pkl[Drive link : ]

Feature structure: model.columns.pkl

📚 Key Learnings & Takeaways
How to clean and preprocess real-world environmental data

Feature engineering using time-based information

Multi-output regression with RandomForestRegressor

Model deployment basics using joblib

Hands-on end-to-end project workflow

📦 Future Scope
Add more input features like Suspended, NH4, BSK5

Improve model using Gradient Boosting or Neural Networks

Create a Streamlit dashboard for water quality monitoring

Deploy as a web app using Flask or FastAPI
