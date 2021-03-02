# RL-Reacher-Unity

This project is an implementation of a Reinforcement Learning solution to the Unity Reacher environment. The goal is to teach a double-jointed arm to follow a target location in space for as long as possible. The state space contains 33 dimensions (including position, rotation, velocity, etc.). The action space consists of 4 numbers between -1 and 1 which represent the torque of the two joints. In this version, the environment contains 20 such agents, learning at the same time. The environment is considered solved when the average reward over 100 episodes and over all agents exceeds 30.

## Getting Started

The solution (including installing necessary packages, initialising the environment, and training the agents) can be executed by running the Continuous_Control.ipynb file.

## Project files

The project consists of the model.py and agent.py files, as well as the Continuous_Control.ipynb notebook. They are organized as follows:

* model.py containes the code for the neural network.
* agent.py represents the agent itself. Here the DDPG logic is implemented.
* Continuous_Control.ipynb contains the code for installing the necessary libraries, importing them, initialising the environment, agent and model, and training and saving the model weights.
* The trained model's saved weights:
	* checkpoint_actor_local.pth
	* checkpoint_actor_target.pth
	* checkpoint_critic_local.pth
	* checkpoint_critic_target.pth


These files, as well as the solution and explanation are based on the instructions and sample codes provided in the Udacity Deep RL Nanodegree.