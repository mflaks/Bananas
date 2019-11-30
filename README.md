
# Environment:

## Goal
The goal of our agent is to collect yellow bananas and don't collect blue bananas.
The problem is solved when the agent receives 13+ score in average over 100 episodes

![bananas](Bananas.JPG)

## Game Over
The game ends after 300 steps

## Rewards:
- Collect Yellow Bananas: +1
- Collect Blue Bananass: -1
- Don't collect Bananas: 0

## State Action:
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. 

Four discrete actions are available, corresponding to:
`0`  move forward.
`1`  move backward.
`2`  turn left.
`3`  turn right.

- State: There are 37 features on each State
- Action: There are 4 possible actions to take in each State

# The Model:
We will create a DQN Model that will use the following Algorithm:
- SumTree
- Prioritize Experience Replay - PPER
- Dueling DQN
- Double DQN

# Installation
## Step 1: Clone the DRLND Repository
Follow the instructions in the DRLND GitHub repository https://github.com/udacity/deep-reinforcement-learning#dependencies to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

## Step 2: Download the Unity Environment
For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:

Linux: https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip

Mac OSX: https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip

Windows (32-bit): https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windohttps://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip

Windows (64-bit): https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip

Then, place the file in the p1_navigation/ folder in the DRLND GitHub repository, and unzip (or decompress) the file.

## Step 3: Explore the Environment
After you have followed the instructions above, open Navigation.ipynb (located in the p1_navigation/ folder in the DRLND GitHub repository) and follow the instructions to learn how to use the Python API to control the agent.

# How to Run the Code
- Open the file Navigation
- Run the cell: Import the libraries
- Run the cells SumTree, PER, Network, Agent in order to create classes that your DQN Model will need.
- Select the Hyperparameters you desire and run the cell to create the DQN Model. The trained parameters will be automaticaly saved as parameters3.pt
- Run the cell TEST the Model to see how your agent is doing with the trained parameters

