# AI-Agent-Trading

1. 📈 AI Agent for Trading

An intelligent Deep Q-Learning (DQN) based trading bot that learns to buy, hold, or sell a stock based on historical price data using reinforcement learning.
🔍 Overview

This project builds a trading agent using Deep Q-Network (DQN) to interact with a simulated stock trading environment. The agent learns over episodes to maximize total portfolio returns.

    📊 Data Source: Yahoo Finance via yfinance
    🧠 Model: Deep Q-Network (PyTorch)
    💸 Actions: Buy / Hold / Sell
    🧪 Backtesting with real data

📁 Files

    AI_Agent_for_Trading.ipynb — Main notebook containing the implementation and training logic.
    AI Agent for Trading.pdf — Exported PDF version for quick reference or sharing.

2. ⚙️ Setup Instructions

Clone the repository:

git clone https://github.com/your-username/ai-agent-for-trading.git
cd ai-agent-for-trading

  Install dependencies: pip install -r requirements.txt

  Run the notebook:

   - Open AI_Agent_for_Trading.ipynb in Google Colab or Jupyter Notebook.

   - Optionally change the stock symbol or date range as needed.

3. 🧠 How It Works

    The agent observes a 4-dimensional state:

     - Close Price

     - 5-Day SMA

     - 20-Day SMA

     - Daily Return

    It interacts with a simulated trading environment:

      - Buy if there's enough balance

      - Sell if holding any stock

      - Hold otherwise

    The reward is based on the change in portfolio value.

   4.  📉 Sample Output

      Episodes 500/500, Total Reward: 21154.55

     Final Balance after testing: $25133.74
          Total Profit: $15133.74

  5. 🚧 Known Issues

        - Some warnings from using float() on pandas.Series. Fixable with .iloc[0].

        - Training is stochastic — results may vary.

        - Basic state features — can be expanded (e.g., RSI, MACD, etc.)

  6. 🔮 Future Enhancements

        - Live trading integration (Alpaca, Zerodha Kite)

        - Advanced RL models (e.g., PPO, A2C)

        - Feature expansion and model optimization
