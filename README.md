# Inventory-Management

## Overview

This project implements a Q-learning-based reinforcement learning algorithm for managing inventory efficiently. The goal is to maximize profits by optimizing order decisions while considering demand fluctuations.

## Features

- Simulates an inventory environment where stock levels and demand vary.

- Implements Q-learning to train an agent for optimal decision-making.

- Uses a hyperparameter grid search to find the best learning parameters.

- Plots learning curves to visualize training progress.

- Tests the trained model to evaluate performance.

## How It Works

- The InventoryEnv class simulates an inventory environment where an agent decides how many units to order.

- The train_q_learning function trains the agent using Q-learning, updating a Q-table based on state-action rewards.

- The training process iterates over multiple episodes to refine the Q-values.

- A hyperparameter grid search is conducted to find optimal values for learning rate (alpha), discount factor (gamma), and exploration probability (epsilon).

- The trained model is then tested to evaluate its efficiency in maximizing rewards.

## Hyperparameters

### Parameter and Values Used

- Alpha (learning rate)                         0.1, 0.5
- Gamma (discount factor)                       0.9, 0.99
- Epsilon (exploration rate)                    0.1, 0.2
- Episodes                                      5000

## Results

- The learning curve is plotted to show training performance.

- The best-performing hyperparameters are selected based on total rewards.

- The final Q-table represents the learned policy.

## Output

- The script prints the total reward achieved during testing.

- The Q-table is displayed, where rows represent states and columns represent actions.

