# 🌊 Water Quality Prediction using Machine Learning

This project focuses on predicting water quality indicators — specifically **nitrate concentration (NO₃)** — using historical data from the Southern Bug River. The dataset contains water quality measurements from multiple monitoring stations over time.

---

## 📌 Project Objective

To develop a machine learning model that accurately predicts **NO₃ (nitrate)** levels based on other chemical properties in water such as:

- O₂ (Dissolved Oxygen)
- NO₂ (Nitrite)
- SO₄ (Sulfate)
- PO₄ (Phosphate)
- CL (Chloride)
- Date-based features: **month**, **year**

---

## 📁 Dataset

- Name: `PB_All_2000_2021.csv`
- Source: Southern Bug River Monitoring Stations
- Format: CSV with columns like `id`, `date`, and various chemical pollutants

---

## ⚙️ Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (for machine learning models)

---

## 📈 ML Model Used

- **Random Forest Regressor**: A robust ensemble learning algorithm suitable for tabular data.

---

## 🔧 Steps Performed

1. **Data Loading** and preprocessing
2. **Datetime Conversion** and feature engineering (`year`, `month`)
3. **Missing Value Handling**
4. **Feature Selection** (`O2`, `NO2`, `SO4`, `PO4`, `CL`, `month`, `year`)
5. **Train-Test Split** (80:20 ratio)
6. **Model Training** using Random Forest
7. **Evaluation** using MAE, RMSE, and R² Score
8. **Visualization** of actual vs predicted NO₃ concentrations

---

## 📊 Model Evaluation

- **MAE**: Mean Absolute Error
- **RMSE**: Root Mean Squared Error
- **R² Score**: Coefficient of Determination

These metrics help assess the accuracy and generalization of the trained model.

---

## 📉 Output Visualization

A scatter plot compares actual vs predicted NO₃ values to help visually analyze model accuracy.

---

## 📌 How to Run

1. Clone this repository
2. Open `Water_Quality_Prediction.ipynb` in Google Colab or Jupyter Notebook
3. Upload the dataset: `PB_All_2000_2021.csv`
4. Run the notebook cells step by step

---

## 📚 Improvisations Done

- Extracted time-based features to capture seasonal trends
- Cleaned the dataset by removing missing values
- Selected key pollutant indicators as input features
- Visualized model predictions for better interpretation
- Modularized code for readability and reproducibility

---

## 📦 Future Improvements

- Add more advanced models (e.g. LSTM, XGBoost)
- Deploy using Streamlit or Flask as a web app
- Predict other indicators or use a multi-output model
- Implement real-time water quality alert system

