# Frozen-Lake-problem-using-Reinforcement-Learning
In this project, we apply reinforcement learning to develop a Frozen Lake (8×8) environment where an agent must navigate through the lake and reach the goal state in the fewest steps possible while avoiding holes. 
# Frozen Lake Problem using Reinforcement Learning Approach

## 📄 Project Overview
This project explores four popular **model-free reinforcement learning** methods to solve the classic **Frozen Lake 8×8 environment** from OpenAI Gymnasium. The agent learns to navigate a slippery frozen surface to reach a goal while avoiding holes.

We implemented:
- Q-Learning
- Double Q-Learning
- SARSA
- Monte Carlo

The project includes experimental results, performance comparisons, smoothed learning curves, and analysis on success rates.

---

## 🧠 Algorithms Implemented
| Algorithm         | Type        | Exploration Strategy        | Environment     |
|------------------|-------------|-----------------------------|-----------------|
| Q-Learning        | Off-policy  | Epsilon-greedy with decay   | Deterministic   |
| Double Q-Learning | Off-policy  | Epsilon-greedy with decay   | Stochastic      |
| SARSA             | On-policy   | Epsilon-greedy with decay   | Deterministic   |
| Monte Carlo       | On-policy   | Epsilon-greedy with decay   | Deterministic   |

---

## 🏗️ Requirements

Install the dependencies using:

```bash
pip install -r requirements.txt
requirements.txt
gymnasium
numpy
matplotlib
seaborn
Note: The environment used is FrozenLake-v1 from the gymnasium library.
🚀 Running the Project

Each experiment can be run individually by executing its corresponding script. The implementations support customizable hyperparameters.

Example:

python q_learning_frozenlake.py
python double_q_learning.py
python sarsa_frozenlake.py
python monte_carlo_frozenlake.py
Each script:

Initializes the environment
Trains the agent over a number of episodes
Plots and saves learning curves
Prints success rates
📊 Results Summary

Q-Learning: Success rate up to 99.64% with tuned hyperparameters.
Double Q-Learning: More stable convergence; handled stochastic transitions better.
SARSA: Fast convergence in deterministic setting.
Monte Carlo: Achieved near-optimal policy but with more variability due to episode-based updates.
