# Traffic Analysis Prediction using Machine Learning

**Course:** BIA 678  
**Project Title:** Traffic Analysis Prediction  
**Instructor:** Prof. Denghui Zhang  
**Institution:** Stevens Institute of Technology  
**Contributors:**  
- Jash Shah (20020618)  
- Prerna Desai (20022778)

---

## 🚦 Project Overview

This project focuses on predicting vehicle traffic congestion at four urban junctions using historical data. Leveraging machine learning and parallel computation techniques, the analysis aims to develop a robust predictive model to help urban planners improve traffic flow, reduce congestion, and optimize infrastructure utilization.

---

## 📊 Dataset

- **Rows:** ~48,120  
- **Columns:**  
  - `Datetime`  
  - `Junction`  
  - `Vehicles`  
  - `Id`  
- **Format:** CSV  
- **Observations:** Hourly vehicle counts at four junctions

---

## 🔍 Key Steps & Analyses

### 1. Exploratory Data Analysis
- Data distribution via histograms
- Correlation matrix and scatter plots
- Time-series visualization for seasonal and hourly patterns

### 2. Data Visualization
- Line and area charts to show traffic patterns over time, by month, hour, and junction

### 3. Parallel Computation
- Serial execution time: `0.0494 seconds`
- Parallel execution time: `0.4264 seconds`  
  *(Note: Slower due to multiprocessing overhead for small-scale data)*

### 4. Performance Metrics
- **Time Complexity:** Measured for both serial and parallel tasks
- **Resource Consumption:** ~40.7% CPU, ~3.18 GB RAM
- **Scalability:** Analysis of model efficiency under increasing data loads

---

## 🤖 Model Fitting

Machine Learning Models Tested:
- Random Forest ✅ (Best Performer)
- XGBoost
- KNN
- Decision Tree

**Best Model:** `Random Forest`  
- **Parameters:** `{'max_depth': None, 'n_estimators': 100}`  
- **Evaluation Metrics:**
  - MSE: `0.00156`
  - MAE, RMSE: Lowest among all
  - Accuracy, Precision, Recall, AUC: `1.0`

---

## 🧠 Insights

- **Junction 1** records the highest vehicle traffic.
- **Temporal patterns** reveal peak traffic hours and monthly congestion trends.
- **Random Forest** outperformed others in accuracy and consistency across evaluation metrics.

---

## 📌 Conclusion

The predictive model developed in this project provides actionable insights for urban traffic management. With high-performing machine learning techniques like Random Forest, city planners can better anticipate congestion and implement proactive measures. The project demonstrates the power of combining exploratory analysis, parallel computation, and ML modeling for real-world data challenges.

---

## 🚀 Future Work

- Extend model to live traffic feeds via streaming data
- Integrate weather or event-based data for enhanced prediction
- Explore deployment via a web-based dashboard or traffic monitoring system

---

> 📝 _This project was completed as part of BIA 678 coursework and is intended for academic and learning purposes._
