# Delivery Robot in Grid World using Deep Q-Network

This project simulates a delivery robot in a Grid World environment with obstacles.  
The robot starts from an initial position, moves to the pickup point to collect a package, and then delivers it to the destination.

The robot is trained using Deep Q-Network (DQN).  
Four different maps are designed, and a separate DQN model is trained for each map.

## Features

- Grid World environment with obstacles
- Four different maps
- Delivery task: Start → Pickup → Delivery
- Deep Q-Network training
- Separate model for each map
- Save and load trained models from Google Drive
- Dynamic visualization using ipywidgets
- Training reward and success rate visualization

## Environment

The environment contains:

| Symbol | Meaning |
|--------|---------|
| S | Start position |
| K | Pickup point |
| D | Delivery point |
| # | Wall / obstacle |
| R | Robot |

## Actions

The robot can perform four actions:

| Action | Meaning |
|--------|---------|
| 0 | Move up |
| 1 | Move down |
| 2 | Move left |
| 3 | Move right |

## Algorithm

The project uses Deep Q-Network (DQN), a reinforcement learning algorithm that approximates the Q-value function using a neural network.

The DQN receives the current state of the robot and outputs Q-values for four possible actions.

## Training

Each map is trained separately:

- Map 1 → DQN model 1
- Map 2 → DQN model 2
- Map 3 → DQN model 3
- Map 4 → DQN model 4

The trained models are saved to Google Drive and can be loaded again without retraining.

## How to Run

Open the notebook in Google Colab:

1. Run all setup cells.
2. Mount Google Drive.
3. Train or load the DQN models.
4. Use the interface to select a map.
5. Click `AI Play Dynamic` to watch the robot move.
6. Click `Auto Play` to visualize the movement step by step.

## Result

The robot successfully learns to move from the start position to the pickup point and then to the delivery point while avoiding obstacles.

## Technologies

- Python
- PyTorch
- NumPy
- Matplotlib
- ipywidgets
- Google Colab

## Project Title

Delivery Robot in a Grid World Environment with Obstacles using Deep Q-Network
