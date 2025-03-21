
# Feed Forward Neural Network from scratch in JavaScript

## Overview

This project implements a simple single-layer neural network that learns to chase food in a 2D game environment. The network receives input from the game world and adjusts its weights in real-time to improve its movement toward the food.

## Features
- A basic 2D game environment where an agent moves toward food.
- A single-layer neural network that learns to optimize movement.
- Visualization of the neural network's decision-making process.
- An optional player-controlled entity to compete with the network.


## How It Works
1. **Input**: The neural network receives a 4D input vector: [x, y, food_x, food_y], representing the agent's position and the food’s position.
2. **Processing**:
    - The input is multiplied by a 4×2 weight matrix to get the weighted sum.
    - A sigmoid activation function is applied to the weighted sum.
    - The outputs determine movement: left/right for the x-axis ([0,1]) and up/down for the y-axis ([0,1]).
3. **Training**:
    - The neural network updates weights using a gradient descent approach.
    - The loss function is based on the squared difference between predicted and optimal movement directions.
    - Weights and biases are adjusted using the learning rate parameter.


## Installation
### Prerequisites
Have a web browser that supports JavaScript and the math.js library.
### Setup
No installation is required. Simply open index.html in a web browser or go to https://smhoody.github.io/feed-forward-nn/


## Running the Game
- Open index.html in a browser.
- The AI-controlled agent (blue) will attempt to reach the food (yellow) using its learned behavior.
- The player-controlled agent (optional) can be moved with WASD keys for comparison.


## Customization
- Modify the learning rate (this.n) inside the NN class in index.html.
- Adjust initial weights and biases in the NN constructor.
- Change food movement patterns by modifying food_dx and food_dy.

## Network diagram:
![network-diagram](https://github.com/user-attachments/assets/842b38b1-9740-490b-9c22-f3fa8f0c7838)

## Environment preview:
![image](https://github.com/user-attachments/assets/9e3229b6-3ed7-440a-8b7e-ece543d0d7a9)
