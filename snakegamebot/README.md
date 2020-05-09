# Q-Learning Algorithm
## Project: Train a AI Agent to play Classic Snake Game 

## Introduction
The goal of this project is to create an AI Bot that will be able to learn from scratch how to play the famous game Snake. To do this, I implemented an Algorithm for Deep Reinforcement Learning. This method is to give the machine parameters relevant to its state, and to give a positive or negative reward based on their actions. No rules are given about the game, and the Bot initially doesn't have any information about what to do. The system's goal is to figure it out and devise a strategy to maximize the score-or the reward. we'll see how a Deep Q-Learning algorithm learns how to play snakegame, scoring up to 50 points and showing a solid strategy-in 3 mins of training 

## Install
This project requires Python 3.6 with the pygame library installed, as well as Keras with Tensorflow backend.


## Run
To run the game, executes in the snakegamebot folder:

```python
python classicsnakegameAi.py --display=True --speed=50
```
Arguments description:

- --display - Type bool, default True, display or not game view
- --speed - Type integer, default 50, game speed

This will run and show the agent. The default configuration loads the file *weights/weights.hdf5* and runs a test.
The Deep neural network can be customized in the file classicsnakegameAi.py modifying the dictionary *params* in the function *define_parameters()*



In classicsnakegameAi.py you can set argument *--display*=False and *--speed*=0, if you do not want to see the game running. This speeds up the training phase.

## For Mac users

```                              
def update_screen():
    pygame.display.update() <br>
    pygame.event.get() # <--- Add this line ###
```
