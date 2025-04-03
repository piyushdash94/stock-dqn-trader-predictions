# 🧠 Stock Price Prediction & DQN Trading Agent – INFY (Infosys NSE)

This project brings together two powerful approaches:

1. **Stock Price Prediction** using regression models (XGBoost, Linear Regression, LSTM)
2. **Stock Trading Simulation** using a Deep Q-Network (DQN) reinforcement learning agent

We focus on **Infosys (INFY.NS)** and build a complete pipeline — from predicting prices to learning how to make trading decisions based on them.

---

## 📦 What’s Included

### 🔍 Part 1: Stock Price Prediction
- ✅ Clean historical stock data from Yahoo Finance
- 📈 Feature engineering with indicators like **SMA**, **Momentum**, **RSI**, **Volatility**
- 🔁 Train-Test split with proper scaling
- 📊 Models implemented:
  - **Linear Regression**
  - **XGBoost Regressor**
  - **LSTM Neural Network**
- 📉 Evaluation using RMSE, MAE, and R² Score
- 📈 Visual plots comparing predicted vs actual close prices

### 🤖 Part 2: DQN-Based Trading Agent
- 📐 Builds a **custom OpenAI Gym environment** for stock trading
- 🧠 Trains a **Deep Q-Network (DQN)** using technical indicators + position info
- 🔄 Agent learns to **Buy, Sell, or Hold** based on observed state
- 📈 Plots the portfolio growth and action decisions
- 💾 Model saving and re-evaluation

---

## 💡 Why Two Parts?

We tackle both **prediction** and **decision-making**:
- Traditional models forecast prices.
- Reinforcement Learning lets the agent **learn from trading experience** to maximize long-term profit.

By combining both, we get a clearer view of:
- What price models can tell us
- How an RL agent behaves using only market features

---

## 🧪 Custom Trading Environment

- **State**: Normalized features (e.g., SMA, RSI, position held)
- **Actions**:  
  `0 = Hold`  
  `1 = Buy`  
  `2 = Sell`
- **Reward**: Profit/loss earned on a Sell action

---

## 🧠 Deep Q-Network (DQN) Architecture

- 3-layer neural network (ReLU activations)
- Replay buffer for stable training
- Epsilon-greedy strategy for balanced exploration
- Trained on portfolio profit as reward

---

## 📊 Visual Insights

- Price chart with technical indicators
- Buy/Sell markers plotted on stock price
- Portfolio value tracked over time
- Prediction vs Actual chart for regression models

---

## 🛠 Requirements

```bash
pip install -r requirements.txt
```

Main packages:
- `pytorch`, `tensorflow` (for LSTM & DQN)
- `xgboost`
- `yfinance`, `ta` (technical indicators)
- `scikit-learn`, `matplotlib`, `gym`, `numpy`

---

## 🚀 How to Run

1. Clone the repo:
```bash
git clone https://github.com/yourusername/stock-dqn-trader.git
cd stock-dqn-trader
```

2. Run the notebook:
```bash
jupyter notebook DQN_Trading_INFY_Final_Aligned.ipynb
```

---

## ✅ Suggestions for Improvement

- Compare with **Double DQN**, **Dueling DQN**, or **PPO**
- Try more indicators like **MACD**, **Bollinger Bands**
- Add **risk management rules** like stop-loss
- Extend the setup to **multiple assets or ETFs**

---

## 📚 Summary

This project walks through both:
- Predicting future stock prices using regression techniques
- Learning when to buy/sell using reinforcement learning

It’s a great hands-on way to understand how ML and RL can work in finance — and how to build end-to-end pipelines from scratch.

> Feel free to fork, modify, and experiment with different ideas!

---

📬 Open to feedback, improvements, and collaboration — let’s build cool trading tools together!