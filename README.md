# Bananas

The goal of our agent is to collect yellow bananas and don't collect blue bananas.
The problem is solved when the agent receives 13+ score in average over 100 episodes

Reward:

Collect Yellow Banana: +1

Collect Blue Bananas: -1

Don't collect Bananas: 0



Environment:

State: Theare are 37 features on each State

Action: There are 4 possible actions to take in each State


The Model:

We will create a Model that will use the following Algorithm:

SumTree
Prioritize Experience Replay - PPER
Dueling DQN
Double DQN
