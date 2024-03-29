# Udacity Deep Reinforcement Learning - Project 1 - Navigation
--------------------------------------------------------------

This is the repository for Project 1 - Navigation from the Deep Reinforcement Learning Nanodegree of Udacity.

## Project details

The goal of the project is to train an agent to navigate a flat square world and collect bananas. The agent should be able to use its experience to gradually choose better actions when interacting with the environment.

The state space has `37` dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.

The simulation contains a single agent that navigates the environment.  At each time step, it has four actions at its disposal:
- `0` - walk forward 
- `1` - walk backward
- `2` - turn left
- `3` - turn right

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The task is episodic and, in order to solve the environment, the agent must pick an average score of +13 over 100 consecutive episodes.

## Getting Started

The top level of the project has been developed as a Jupyter notebook (`Navigation.ipynb`) in Python 3, thus make sure that you have a running Python and Jupyter working installation.

The world is provided as an Unity environment and is external to the project itself. To install the environment you will need a distribution of the ml-agents package from Unity. Please follow the installation instructions there, as this may change, in our case we followed the installation instructions of Udacity.

The agent is provided in `agent.py`, and the underlying neural network model in `model.py` (both these files were obtained from Udacity Qnetwork project). For these to run one needs to install Pytorch; other packages that need to be imported directly are numpy, and matplotlib. To install them, please run

`pip install numpy matplotlib pytorch`

In addition all these packkages will have dependencies themselves, which need to be satisfied before proceeding. A complete list of all the dependencies can be found in `requiriments.txt`, and istalled using

`pip requirements.txt`

## Instructions

The notebook is pretty much self-contained. It contains only three cells. 

- Run the first one one to set up the angent and the environment itself.
- The second one is optional, provides some information about the environment and basic usage interface of the agent and its interactions with the environment, as well as an example of how to use the agent. This can be used (by changing epsilon, as indicated in the notebook) to evaluate the trained or untrained agents. A window should pop up that allows you to observe the agent, as it moves through the environment.
- The third one provides the code for the training itself, run this if you want to train the agent.

