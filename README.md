# FUTURE_ML_02
📊 About the Stock Price Forecasting Model
This project focuses on forecasting stock prices using a Gated Recurrent Unit (GRU)-based deep learning model. The model is trained on historical stock data of Apple Inc. (AAPL) from 2015 to 2024, sourced using the yfinance API. The objective is to predict future closing prices by capturing temporal dependencies in the stock market data.

🧠 Model: GRU (Gated Recurrent Unit)
🏁 Overall Performance
MSE (Mean Squared Error):  16.62

(Best result with a 90-day sequence window)

📦 Deliverables
Forecasting Visualization: Displays actual vs. predicted stock prices.
Model Architecture: 2 GRU layers with dropout regularization.
Sequence Length Optimization: Experimented with different time windows (60, 90, 120 days).
Residuals Analysis: Evaluated model errors and stability through visualization and metric tracking.

🧪 Key Learnings
The GRU model efficiently captures temporal trends in stock prices.
Increasing the sequence length beyond 90 days (e.g., to 120) negatively impacted accuracy due to overfitting or excess noise.
Dropout usage had mixed results and required careful tuning.
Increasing training epochs helped improve model performance.
Using Recurrent Neural Networks for time series forecasting provides flexibility in learning sequential patterns.

📁 Repository Contents
AAPL_stock_data.csv – Historical stock data (2015–2024)
future_ml_02.py – Python script for data preprocessing, model building, training, and forecasting
actual_vs_predicted (2).png – Visualization comparing actual and predicted prices
README.md – Project documentation (this file)

✅ Accuracy Summary
Metric	Value
MSE	 16.62
(Best model with 90-day sequence)	

📌 Future Enhancements
Experiment with Bidirectional GRU or LSTM layers
Add technical indicators (e.g., moving averages, RSI) as features
Train on additional stocks or market indices
Deploy the model as a web app using Flask or Streamlit
Integrate real-time stock prediction with live APIs
