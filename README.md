# 🧠 Crypto RL Trader — Reinforcement Learning for Market Simulation

This project implements a custom OpenAI Gym environment and reinforcement learning pipeline for simulating and optimizing trading strategies on cryptocurrency market data. It was developed as a hands-on demonstration of deep reinforcement learning applied to real-world time-series forecasting and decision-making under uncertainty.

The dataset consists of hourly historical crypto price data, downloaded from Binance, covering the period from September 1 to at least November 1, 2024. The data is split into training and testing windows to simulate a realistic and temporally consistent trading environment.

Within the simulation, the RL agent is allowed to take discrete actions such as buy, hold, or short the asset at each timestep. In evaluation, the trained agent achieved a +6% return over the test period, while the underlying token declined by -4%, demonstrating the model’s ability to profit in a down-trending market.

---

## 🚀 Project Highlights

- 📈 **Custom Gym Trading Environment**: Tailored simulation with realistic trading mechanics (buy, hold, sell).
- 🧪 **RL Agent Training & Evaluation**: DQN-based agent learns to maximize returns using historical market data.
- 🧠 **Custom Reward Function**: Designed to penalize drawdowns and encourage stable growth, reflecting real trading behavior.
- 📊 **Train/Test Split Based on Time**: Ensures temporally valid evaluation on unseen data.
- 📎 **Modular Pipeline**: Easy to extend with other RL algorithms (e.g., PPO, A2C, SAC).
- 🏗️ **Compatible with Meta's [Pearl](https://github.com/facebookresearch/pearl)**: Designed to integrate advanced production-grade agents.
- 🔧 **Hyperparameter Optimization with [Hyperopt](https://github.com/hyperopt/hyperopt)**: Efficiently tuned learning rate, update frequency, and other agent parameters using Bayesian search space exploration.

---

## 📂 Project Structure

- **`data/`** – Historical crypto market data  
- **`Pearl/`** – Meta's RL library (installed in editable mode)  
- **`renders/`** – Visualizations  
- **`render_logs/`** – Log files  
- **`gym-trader.ipynb`** – Main RL agent logic and tests  
- **`RL_env_setup.ipynb`** – Gym environment definition  
- **`Train_test.ipynb`** – Training and evaluation  
- **`Hyper_params.ipynb`** – Hyperparameter tuning  
- **`requirements.txt`** – Python environment dependencies  
- **`README.md`** – This file
  
## 🙋‍♂️ Author

**Will Enicks**  
Data Scientista & Machine Learning Engineer  
[LinkedIn](www.linkedin.com/in/will-enicks) • [GitHub](https://github.com/Willenicks)
