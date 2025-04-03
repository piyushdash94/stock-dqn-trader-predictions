# 🧠 Stock Price Prediction & DQN Stock Trader – NSE

This project combines two key components:

1. **Stock Price Prediction** using models like XGBoost, Linear Regression, and LSTM
2. **Trading Decision Making** using a Deep Q-Network (DQN) reinforcement learning agent

It is built using **Infosys (INFY.NS)** stock data from the NSE and can be adapted to other stocks.

---

## 📦 What’s Inside

### 🔍 Part 1: Stock Price Prediction
- Historical data fetched from Yahoo Finance
- Technical indicators like **SMA**, **RSI**, **Momentum**, and **Volatility**
- Models used:
  - **Linear Regression**
  - **XGBoost Regressor**
  - **LSTM Neural Network**
- Evaluation metrics: **RMSE**, **MAE**, **R² Score**
- Plots: Predicted vs Actual Close Prices

### 🤖 Part 2: DQN-Based Trading Agent
- Custom **Gym Environment** built for trading logic
- Trains a DQN to decide **Buy, Sell, or Hold**
- Tracks performance and learns via **rewards from profit**
- Saves and reloads the model
- Visualizes portfolio growth and trade decisions

---

## 💡 Why This Structure?

This dual-part setup covers both:
- Forecasting prices using ML models
- Making trading decisions through RL

It gives a fuller view of what’s possible with data-driven trading strategies.

---

## 🧪 Environment

- **State**: Normalized indicators + position flag
- **Actions**: `0 = Hold`, `1 = Buy`, `2 = Sell`
- **Reward**: Profit/loss at the time of sell

---

## 🧠 DQN Agent

- Built using a 3-layer neural net with `ReLU`
- Epsilon-greedy strategy for exploration
- Experience replay for stability

---

## 📊 Visual Outputs

- Technical indicator plots
- Price vs Predicted (from regression models)
- Portfolio value over time
- Buy/Sell markers on price chart

---

## 🛠 Requirements

```bash
pip install -r requirements.txt
```

Main packages:
- `pytorch`, `tensorflow`
- `xgboost`
- `ta`, `yfinance`
- `matplotlib`, `scikit-learn`, `gym`, `numpy`

---

## 🚀 How to Run

1. Clone the repo:
```bash
git clone https://github.com/yourusername/dqn-stock-trader-predictions.git
cd dqn-stock-trader-predictions
```

2. Run the notebook:
```bash
jupyter notebook DQN_Trading_NSE_predictions.ipynb
```

---

## ✅ What to Try Next

- Add more advanced DQNs like **Double DQN**, **Dueling DQN**
- Include indicators like MACD, Bollinger Bands
- Add stop-loss or risk logic
- Test on multiple NSE stocks

---

## 📚 Summary

This repo is a great launchpad for combining Machine Learning and Reinforcement Learning in financial applications.  
Whether you're exploring predictive modeling or building trading bots — this project covers both.

> Fork it, try ideas, and improve the strategy!

---

📬 Feel free to contribute, open issues, or collaborate!