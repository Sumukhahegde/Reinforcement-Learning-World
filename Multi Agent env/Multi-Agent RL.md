# Multi-Agent Reinforcement Learning
<img src="image/Tennis.gif" alt="Tennis" align="left"  width="650"/>      
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>


## Multi Agent Environment Types:

* **Cooperative Environments**: 

An environment where multiple agents have to accomplish a goal by working together is called a cooperative environment. In this kind of environment, when both agents are able to successfully complete a task together, they are rewarded and so both of them learn to cooperate in the environment. A good example for this kind of environment is the example we covered above where two drones have to work together to pick a package and deliver it.

* **Competitive Environments**: 

An environment where multiple agents have to compete with each other to reach their goal is called a Competitive Environment. In this kind of environment, each agent is tasked with a similar goal which can only be achieved by one of them and the agent that is able to achieve the goal is rewarded. This reinforces the idea of competing with the other agent in the environment. A good example for this kind of environment is one you will see an implementation of very soon, which is the Tennis Environment in which we work with two agents present on opposite sides of the net and both are tasked with not letting the ball drop on their side. And if the ball drops on the opponent's side then they are rewarded.

* **Mixed Environments**: 

An environment where multiple agents have to both cooperate and compete  with each other by interacting with their environment is called a Mixed Environment. In this kind of environment, each agent is tasked with achieving a goal for which they not only have to cooperate with other agents in the environment but also compete with them. Here depending upon which has more preference, you will assign higher rewards for the kind of action you prefer your agent to fulfill. Say, giving higher positive reward to cooperation and lower positive reward to competition. In this kind of setting the agents would cooperate more and compete less, but they will do both the actions. A good example for Mixed Environment is a Traffic Control setting, where each agent is tasked with reaching their goal as fast as possible. For a Traffic Control environment, each agent has to adhere to the traffic rules and make sure that it does not crash into other agents while driving, but at the same time they have to overtake the other agents in order to reach their goal faster while driving within the speed limits.


