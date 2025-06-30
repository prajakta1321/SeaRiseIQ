# 🌊 SeaRiseIQ: Hybrid Forecasting and Trend Detection of Sea Level Rise

**SeaRiseIQ** is a hybrid data science framework that combines classical time series forecasting with quantum-inspired classification to analyze and predict global mean sea level (GMSL) trends.

Using NASA's satellite-based GMSL dataset (with and without Glacial Isostatic Adjustment), this project:
- Forecasts future sea levels using ARIMA and Linear Regression
- Classifies rising vs. non-rising trends using Logistic Regression, SVM, and a simulated Quantum SVM (QSVM)
- Compares model performance using statistical metrics and visual diagnostics

---

## 📈 Features

- 📊 Time series forecasting using **ARIMA**
- 🔁 Regression-based prediction with **Lag Features**
- 🧠 Trend classification using **Logistic Regression**, **SVM**, and **Quantum SVM**
- 🧪 Exploratory data analysis and visual insights
- 📦 Clean, reproducible pipeline in Python (Jupyter Notebook)
- 📉 Performance evaluation: MSE, MAE, R², F1-Score, Confusion Matrix
- 🔍 Comparison of GMSL with vs. without GIA correction

---

## 🧠 Technologies Used

- Python 3.x
- Pandas, NumPy, Matplotlib, Seaborn
- scikit-learn
- statsmodels
- Qiskit Machine Learning (simulated QSVM)

---

## 📁 Dataset

- **Source:** NASA PO.DAAC  
- **File:** `GMSL_TPJAOS_5.2.txt` converted to CSV using custom Python script  
- Columns include:
  - `GMSL_GIA`, `GMSL_noGIA`, `year_fraction`, etc.

---

## 🔍 Visual Outputs

- Sea level rise plots (with and without GIA)
- Difference analysis (~3.91 mm avg)
- ARIMA forecast with 95% confidence intervals
- Residual plots, ACF/PACF analysis
- Trend classification plots and model comparisons

---

## 📊 Model Performance Snapshot

| Model               | MAE (mm) | R² Score | F1 (Class 1) |
|--------------------|----------|----------|---------------|
| Linear Regression   | 1.81     | 0.93     | N/A           |
| ARIMA               | 9.22     | –0.84    | N/A           |
| Logistic Regression | —        | —        | 0.54          |
| Simulated QSVM      | —        | —        | 0.53          |

---

## 🚀 Future Scope

- Integration with live dashboards using Streamlit or Dash
- Extension to multi-class trend labeling
- Deploying real quantum models (e.g., IBM Q backend)
- Using LSTM or hybrid models for deeper learning
