# LunarLander-DQN-
Implementation and comparison of four Deep Q-Learning variants—Classic DQN, Double DQN, Dueling DQN, and Dueling Double DQN (D3QN)—for the Lunar Lander-v3 environment using PyTorch. Includes neural network architectures, replay buffer, target networks, epsilon-greedy exploration, training loop, and performance evaluation.
# Deep Q-Learning Variants for Lunar Lander

## Overview
This repository contains implementations and comparisons of four Deep Q-Learning algorithms applied to the Lunar Lander-v3 environment from OpenAI Gymnasium. The goal is to train an agent capable of safely landing a spacecraft on the lunar surface while minimizing fuel consumption.

## Task Description
The Lunar Lander environment is a classic reinforcement learning problem where the agent must control a spacecraft with four discrete actions:
- 0: Do nothing
- 1: Fire left orientation engine
- 2: Fire main engine
- 3: Fire right orientation engine

The state space consists of an 8-dimensional vector representing the lander's position, velocity, angle, angular velocity, and leg contact indicators.

The reward structure incentivizes the agent to:
- Approach the landing pad carefully
- Move slowly to avoid crashes
- Maintain a horizontal angle
- Land with legs touching the ground
- Minimize engine fuel consumption

Episodes terminate if the lander crashes, moves out of bounds, or becomes inactive. A successful landing achieves a total reward of at least 200 points.

## Implemented Algorithms
- **Classic DQN:** Baseline Deep Q-Network approach.
- **Double DQN (DDQN):** Reduces overestimation bias in value updates.
- **Dueling DQN:** Separates value and advantage streams for better state evaluation.
- **Dueling Double DQN (D3QN):** Combines Double DQN and Dueling DQN improvements.

## Features
- Neural network architectures for each DQN variant
- Experience replay buffer for stable learning
- Target networks for consistent training targets
- Epsilon-greedy exploration strategy
- Training loops implemented in PyTorch
- Performance evaluation and comparison across models

## Code
All algorithms are fully implemented and tested within this repository. The code is modular and well-documented for easy understanding and extension.

---

Feel free to explore the code and experiment with different hyperparameters to improve agent performance!

