# DRL-stock_trading
## Financial Modeling and Trading Environment Simulation
# Overview
This project is focused on simulating a stock trading environment using historical stock data. It aims to train a reinforcement learning model using the Proximal Policy Optimization (PPO) algorithm to make profitable trading decisions. The simulation environment is built upon the OpenAI Gym framework, allowing for an extensible and standardized approach to developing and testing trading strategies.

# Features
Data Collection and Processing: Fetches and processes historical stock data, including enterprise values, EBITDA, market capitalization, and sector information.
Trading Environment: A custom stock trading environment (AdvancedStockTradingEnv) that simulates the buying and selling actions within the stock market, tracking the net asset value (NAV) over time.
Reinforcement Learning Model: Utilizes the PPO algorithm from the Stable Baselines 3 library to train a model on the trading environment, with the goal of maximizing the NAV through strategic trading actions.
Evaluation and Analysis: After training, the model's performance is evaluated on a separate test dataset, and the NAV progression is visualized to assess the effectiveness of the trading strategy.
# Dependencies
Python 3.8+
pandas
matplotlib
numpy
gym
stable-baselines3
requests (for data fetching)
#Installation
Ensure you have Python 3.8 or higher installed. Clone this repository, navigate to the project directory, and install the required dependencies:

Copy code
pip install -r requirements.txt
# Usage
To run the trading simulation and model training, execute the main script DRL_EDA:

css
Copy code
python main.py
This will start the process of data fetching, environment setup, model training, and evaluation. Adjustments to the training parameters and data sources can be made within the script or by modifying the environment's configuration.

# Customization
The trading environment and model can be customized to fit different datasets, financial instruments, and trading strategies. The environment's __init__ method and the model's hyperparameters are key areas for customization.

# Evaluation
After training, the model's performance is evaluated on unseen test data. The NAV progression during the evaluation period is plotted, providing insight into the trading strategy's effectiveness over time.

# Contributing
Contributions to improve the simulation environment, model performance, or expand the dataset are welcome. Please submit a pull request or open an issue to discuss potential changes.

