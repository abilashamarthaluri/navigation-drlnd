# Navigation using Reinforcement Learning 

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"


## About this project
    
This project is done as part of the Reinforcement Learning Nanodegree by Udacity. In this project, we have an environment provided by [Unity](https://unity3d.com/) in which there are 2 kinds of Banana's Yellow and Blue. 
    
For this project, we will train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.
    
    
## Prerequisites

1. Please follow the instructions given at [Udacity DRLND](https://github.com/udacity/deep-reinforcement-learning/#dependencies) repository for setting up the environment we need with python 3.6 and the other requirements. 

2. Also download the Unity 3d Banana environment / app based on the machine / OS you have.
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/VisualBanana_Windows_x86_64.zip)

3. Make a folder ./data/ relative to the current folder 

4. Then place the respective unzipped environment under ./data/ folder.

## Training a Smart Agent

Open up Navigation.ipynb notebook and follow the instructions to train a smart agent, interact with the enviroment, and later watch a smart Agent.

## Implementation Details

Please take a look at [Report](./Report.md) for more details on the implementation.

    
