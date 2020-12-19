## Actor Critic Method

## Structure
In Actor critic model we have 2 seperate models

### Environment
Here we will be using a **Pendulum** environment which is a continuous environment. It has an infinit input space. Implementing DQN will not work in this environment because it work only in descrete action space. 

## Actor critic has 2 main variants:
1. Asynchronous Advantage Actor Critic(A3C)
2. Advantage Actor Critic(A2C)
**Note:** 
- The key advantage of using A3C is that, it is effective and efficient exploration of the space.
- The difference is that, A2C does not have the asynchronours part of A3C.


### Policy based methods have high variance

## Resources:
1. https://openai.com/blog/baselines-acktr-a2c/ 
1. A3C - https://arxiv.org/abs/1602.01783 