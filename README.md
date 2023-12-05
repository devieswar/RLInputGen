# RLInputGen: Reinforcement Learning Guided Input Generation

## Introduction
RLInputGen is a project that explores the use of reinforcement learning (RL) to guide the generation of diverse inputs for a specific problem domain. The primary motivation for this project is to enhance the variety and quality of inputs for a system, leveraging the decision-making capabilities of RL agents.

## Problem Statement
In many applications, having diverse and well-distributed inputs is crucial for training and testing systems effectively. RLInputGen aims to address this challenge by using RL agents to generate inputs that follow a specific set of rules or criteria.

## Techniques and Implementation
### BSTEnvironment
The `BSTEnvironment` class represents the environment in which the RL agent operates. It simulates a scenario related to Binary Search Trees (BSTs), where the agent generates inputs with the goal of satisfying certain properties, such as creating valid BSTs.

### RLAgent
The `RLAgent` class is the core component responsible for training and guiding the input generation process. It uses a neural network model to predict the next action based on the current state. The training involves reinforcement learning with a policy gradient approach.

## Usage
1. **Instantiate RLAgent:**
   ```python
   from RLAgent import RLAgent
   agent = RLAgent(input_size, output_size, max_tree_size)
   
2. **Instantiate Environment:**
   ```python
   from BSTEnvironment import BSTEnvironment  #Provide different environment for different test input generation.
   env = BSTEnvironment(max_tree_size)

