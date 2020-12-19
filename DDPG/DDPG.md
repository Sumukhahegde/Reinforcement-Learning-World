## DDPG
### Deep Deterministic Policy Gradient Method
Deep Deterministic Policy Gradient (DDPG) is an algorithm which concurrently learns a Q-function and a policy. It uses off-policy data and the Bellman equation to learn the Q-function, and uses the Q-function to learn the policy.
- DDPG is Off policy Algorithm
- It is a Deep-Q learning for continuous action spaces

## Essentials
- Basic knowledge of Value & policy based learning
- Actor Critic method

## Why we nee DDPG?
- Q learning cannot handle the continuous action spaces
- When there is finite number of actions or a discrete action space, we can directly compute q-values for each action and compare them. But when action space is continuous, we cant evaluate all the space. Calculating $Q_max$ in this case, would computationally very expensive. 

## Type of Actor Critic Method required
- 2 distinct Actor-Critic networks
- Critic will evaluate the State-Action Pair
- Actor will decide on action to take the current state
    - It will output the action values (Not probabilities)

## Network Schema
DDPG has 4 neural networks, 
- Q network
- Deterministic Policy Function
- Target Q network
- Target Policy Network

> The ``Actor`` function directly maps the states to actionsinstead of outputting the probability distribution
> The ``Target`` networks are time delayed copies of the original networks. They essentially help in improving the stability of the netowrk
> ``Replay Buffer`` is used, similar to the Deep Q learning, where the experiences are saved in form of tuples (state, action, reward, next_state). A random batch from these samples are used for updatingthe value and policy network.

## Pseudo-code for DDPG
<img src = "image/ddpg_pseudocode.png">

## There are 4 parts
1. Experience Replay
1. Actor Critic network updates
1. Target Network Updates
1. Exploration


## Resources:
1. https://spinningup.openai.com/en/latest/algorithms/ddpg.html
2. https://stable-baselines3.readthedocs.io/en/master/modules/ddpg.html#notes 
3. https://towardsdatascience.com/deep-deterministic-policy-gradients-explained-2d94655a9b7b 