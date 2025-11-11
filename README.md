# Inventory-Demand-Forecasting-
Inventory Demand Forecasting system using Machine Learning and Time-Series models (ARIMA, Prophet, XGBoost, LSTM) on the Olist Brazilian E-Commerce dataset to optimize stock levels and improve supply chain efficiency.

# Inventory Demand Forecasting using Machine Learning

This project implements an intelligent **Inventory Demand Forecasting System** that predicts future product demand using a combination of **Time-Series Forecasting** and **Machine Learning models**. The goal is to help businesses optimize stock levels, avoid overstocking or stockouts, and make data-driven supply chain decisions.

The system uses the **Olist Brazilian E-Commerce Dataset**, which includes detailed transactional, product, and customer-level data. Multiple forecasting models such as **ARIMA, Prophet, XGBoost, and LSTM** are developed, evaluated, and compared to identify the best-performing model.

---

## 🚀 Key Features

- End-to-end forecasting pipeline: **data preprocessing → feature engineering → model training → evaluation**.
- Supports multiple forecasting approaches:
  - **ARIMA / SARIMAX** for trend and seasonality patterns
  - **Facebook Prophet** for long-term trend and holiday impact modeling
  - **XGBoost Regressor** for non-linear feature-based demand learning
  - **LSTM Neural Network** for deep temporal dependency modeling
- Performance assessed using **MAE, RMSE, and MAPE** metrics.
- Feature importance visualization to support **explainability** for business decisions.

---

## 📂 Dataset

This project uses the **Olist Brazilian E-Commerce Public Dataset**, available on Kaggle:

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Key data components used:
- Orders & purchase timestamps
- Customer & seller records
- Product category details
- Reviews and delivery performance
- Payment and pricing attributes

---

## 🛠 Tools and Technologies Used

| Category | Libraries / Tools |
|---------|------------------|
| **Language** | Python 3.x |
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Machine Learning** | Scikit-learn, XGBoost |
| **Time-Series Models** | Statsmodels (ARIMA), Prophet |
| **Deep Learning** | TensorFlow / Keras (LSTM) |

---

## 🔧 System Workflow

1. **Data Collection & Merging**
2. **Cleaning & Preprocessing**
3. **Feature Engineering**
   - Time-based features (month, week, season)
   - Lag features and rolling statistics
   - Encoded product & customer attributes
4. **Model Training (ARIMA, Prophet, XGBoost, LSTM)**
5. **Model Evaluation**
6. **Comparison & Interpretation**

---

## 📊 Model Performance Summary

| Model | MAE ↓ | RMSE ↓ | MAPE ↓ | Notes |
|------|------|-------|--------|------|
| ARIMA / SARIMAX | Moderate | Moderate | Higher | Good for basic trend but limited adaptability |
| Prophet | Good | Good | Stable | Captures seasonal patterns well |
| **XGBoost (Best Overall)** | **Lowest** | **Lowest** | **Most accurate** | Handles non-linear & multi-feature interactions best |
| LSTM | Good | Good | Slightly higher | Best at sequential dependencies but computationally heavy |

**Conclusion:**  
**XGBoost** provided the most stable and accurate forecasts across product categories.  
Combining **XGBoost + Prophet** offers a strong hybrid forecasting strategy.

---

## 📈 Visual Outputs (Examples)

- Predicted vs Actual Demand Curves
- Feature Importance Charts (XGBoost)
- Seasonality Components (Prophet Trend Analysis)

> Add these visuals in the repository’s `results/` folder for clarity.

---

## 🔮 Future Enhancements

- Integrate **real-time demand forecasting** with streaming data.
- Expand model with **external data** such as weather, holidays, and marketing events.
- Deploy model as a **web dashboard** using Streamlit or Flask.
- Implement **Automated Model Retraining** as new data arrives.

---

## 🤝 Contributors
- Anant Jain
- Arnav Pandey
- Akshat Pratik  
Under the guidance of **Dr. Sowmya J**, Department of Computational Intelligence, SRM Institute of Science and Technology.

---

## 📜 License
This project is for academic and research purposes. Modify and extend as needed for real-world applications.


