# Deep-RL-Arm-Control

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"

### Introduction

For this project, work is done in [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment.

![Trained Agent][image1]

In this environment, a double-jointed arm can move to target locations.   

You can read more about this environment in the ML-Agents GitHub [here](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#soccer-twos).  To solve this harder task, you'll need to download a new Unity environment. Reward of +0.1 is provided for each step that the agent's hand is in the goal location. 

1. The goal of your agent :  

    To maintain its position at the target location for as many time steps as possible.

2. Project Details : 

    The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1. The Unity environment used contains 20 identical agents, each with its own copy of the environment.  

3. Environment solved criteria:

    In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents).  Specifically,
        - After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent.  This yields 20 (potentially different) scores.  We then take the average of these 20 scores. 
        - This yields an **average score** for each episode (where the average is over all 20 agents).

    The environment is considered solved, when the average (over 100 episodes) of those average scores is at least +30. 

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - **_Twenty (20) Agents_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)

2. Place the file in the DRLND GitHub repository, in the `p2_continuous-control/` folder, and unzip (or decompress) the file. 

3. Start working in the `Continuous_Control.ipynb` file.

### Instructions

Follow the instructions in `Continuous_Control.ipynb` to get started with training your own agent. Run section 5 to train and plot the agent. The model weights gets stored in checkpoint_actor.pth and checkpoint_critic.pth, and can be directly used if you do not wish to train again.


