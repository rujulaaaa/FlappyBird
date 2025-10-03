# Flappy Bird DQN Agent

This project implements a Deep Q-Network (DQN) agent using PyTorch to play the game Flappy Bird autonomously. The aim was to build and train a reinforcement learning agent capable of learning optimal gameplay strategies from raw game state inputs without human intervention.

## Project Overview

The Flappy Bird agent uses a convolutional neural network (CNN) that learns policies through interaction with the game environment. The DQN algorithm approximates the Q-value function to estimate the expected rewards for actions taken in different game states, enabling the agent to improve its policy over time.

Key components of the project include:
- Environment setup and game simulation for Flappy Bird
- Deep Q-Network architecture with convolution layers suitable for image input
- Experience replay buffer for stabilizing training
- Epsilon-greedy policy for balancing exploration and exploitation
- Training loops with reward tracking and periodic evaluation

## Features

- State representation from preprocessed game frames (grayscale, resized)
- Deep Q-learning with target network updates to stabilize learning
- Frame stacking for temporal context to capture motion dynamics
- Automatic saving and loading of model checkpoints
- TensorBoard logging for real-time training visualization

## Results

The trained agent learned to navigate through the gaps between pipes by flapping at the right time, progressively improving its score with training episodes. The performance was validated through reward curves and evaluation gameplay, demonstrating the effectiveness of the DQN approach for game playing in simple visual environments.

## Project Structure

- `dqn_flappy.py`: Main script to train and evaluate the DQN agent on Flappy Bird
- `model.py`: Defines the CNN-based Q-network architecture
- `replay_buffer.py`: Implements experience replay functionality
- `utils.py`: Utility functions for preprocessing and training
- `runs/flappybird`: Directory containing logs and model checkpoints for training runs on Flappy Bird

## Learning Outcomes

This project deepened my understanding of reinforcement learning, particularly deep Q-learning, experience replay, and stabilizing training using target networks. 
Implementing this in PyTorch helped consolidate practical skills in deep learning frameworks, while the challenge of Flappy Bird provided a visually intuitive and engaging platform for RL experimentation.

## References

https://youtu.be/arR7KzlYs4w?si=mgjode0G0Tn5JUq1
