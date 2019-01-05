# Report

I have implemented both Vanilla DQN and DDQN agent to solve the Banana Environment. 

## Model Architecture / Learning Algo:

I have used a Deep Neural Network with layers of size (state_size * 32), (32 * 64), (64* 128) and (128 * action_size) respectively. Also Used Relu for the non linearity and used [Batch norm](https://arxiv.org/abs/1502.03167) for normalizing the activations of the hidden layers. 

## Hyper parameters:

- BUFFER_SIZE = int(1e6)  # replay buffer size
- BATCH_SIZE = 32         # minibatch size
- GAMMA = 0.99            # discount factor
- TAU = 1e-2              # for soft update of target parameters
- LR = 5e-4               # learning rate 
- UPDATE_EVERY = 10        # how often to update the network

I am using a ReplayBuffer and a Target network as mentioned in the [DQN Paper](https://www.nature.com/articles/nature14236) 

UPDATE_EVERY seems to play a major role in how fast the agent is able to converge. I am also using Soft Update for the target parameters which is nothing but a Linear Interpolation of the parameters from local network to the target network controlled by the tau parameter θ_target = τ*θ_local + (1 - τ)*θ_target.

Vanilla DQN tends to overestimate the action values initially and a proposal to solve this problem is given in this paper [DDQN](https://arxiv.org/abs/1509.06461) 

Using DDQN, I am able to solve the environment in about 323 episodes, with an average score of ~ 13.05 for the last 100 1pisodes.


## Rewards Plot: 

![Rewards Plot](/images/report.jpg?raw=true "Agent Rewards")


## Ideas for Future Work

There are lot of proposals for improving the Vanilla DQN. Most of these ideas are summarized and put together in this [Rainbow](https://arxiv.org/abs/1710.02298) paper. Would like to implement a rainbow agent with all the different ideas like Prioritized DDQN, Duelling DDQN, and Rainbow itself.





