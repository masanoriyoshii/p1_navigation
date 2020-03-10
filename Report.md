
# Report

## Overview

This project aims to understand Reinforcement Learning through the coding exercise. Deep Q Network is used to train the RL agent.


## Hyper Parameters

### Training
- n_episodes (int): maximum number of training episodes
- max_t (int): maximum number of timesteps per episode
- eps_start (float): starting value of epsilon, for epsilon-greedy action selection
- eps_end (float): minimum value of epsilon
- eps_decay (float): multiplicative factor (per episode) for decreasing epsilon


### DQN Agent
- BUFFER_SIZE : replay buffer size
- BATCH_SIZE : minibatch size
- GAMMA : discount factor
- TAU : for soft update of target parameters
- LR : learning rate
- UPDATE_EVERY : how often to update the network

## Neural Network
- The QNetwork model involves the 3 Fully Connected layers.  
- Relu is used as an activation function.


## Result

### Starting Point

```
n_episodes = 2000
max_t = 1000
eps_start = 1.0
eps_end = 0.01
eps_decay = 0.995
```

```
BUFFER_SIZE = int(1e5)  # replay buffer size
BATCH_SIZE = 64         # minibatch size
GAMMA = 0.99            # discount factor
TAU = 1e-3              # for soft update of target parameters
LR = 5e-4               # learning rate
UPDATE_EVERY = 4        # how often to update the network
```

```
Episode 100	Average Score: 1.19
Episode 200	Average Score: 4.43
Episode 300	Average Score: 8.47
Episode 400	Average Score: 10.56
Episode 500	Average Score: 12.31
Episode 600	Average Score: 13.18
Episode 700	Average Score: 14.00
Episode 800	Average Score: 14.77
Episode 900	Average Score: 15.97
Episode 1000	Average Score: 16.08
Episode 1100	Average Score: 16.00
Episode 1200	Average Score: 16.21
Episode 1300	Average Score: 17.20
Episode 1400	Average Score: 16.53
Episode 1500	Average Score: 15.63
Episode 1600	Average Score: 16.55
Episode 1700	Average Score: 15.56
Episode 1800	Average Score: 15.48
Episode 1900	Average Score: 15.22
Episode 2000	Average Score: 16.19
```

![](https://user-images.githubusercontent.com/4464676/74999091-fc6fb780-549d-11ea-9cd4-8c8876fb7a0a.png)


### After tweaking the hyper parameters

```
n_episodes = 1000
max_t = 1000
eps_start = 0.75
eps_end = 0.01
eps_decay = 0.9
```

```
BUFFER_SIZE = int(1e5)  # replay buffer size
BATCH_SIZE = 64         # minibatch size
GAMMA = 0.99            # discount factor
TAU = 1e-3              # for soft update of target parameters
LR = 5e-4               # learning rate
UPDATE_EVERY = 4        # how often to update the network
```

```
Episode 100	Average Score: 4.14
Episode 200	Average Score: 8.68
Episode 300	Average Score: 12.62
Episode 305	Average Score: 13.01
Environment solved in 205 episodes!	Average Score: 13.01
```

![](https://user-images.githubusercontent.com/4464676/76272910-dd578f00-62bf-11ea-8be3-4a8473c8336a.png)

## Ideas for Future Work

Try other algorithms.
- Experience Replay Buffer
- Double DQN
- Dueling DQN
