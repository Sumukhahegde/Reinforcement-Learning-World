# Multi Agent Environment
### Types of Multi Agent Environment:
1.	Cooperative:
- A simple approach as the concepts from the single agent carry easily here
- Share team reward
- Coordination problem
2. Competitive:
- Zero Sum games
- Individual Opposing rewards
- Minimax equilibria
3. Mixed:
- Agent maximized their utility which may require cooperating and/or competing
- General Sum Games
- Nash equilibria 


# MADDPG
## Multi Agent Deep Deterministic Policy Gradient

### MADDPG adopts a framework of:
1. Centralized training
- Agents share experience during the training
- Implement via shared experience replay buffer
1. Decentralized Execution
- Each agent used only local observation at execution time

### It is extended Actor-Critic Policy gradient method (DDPG)
- The Critic builds up with information about policies of other agents
- Actor has access only to local information

## Performance
MADDPG agents outperform DDPF agents in a wide variety of test environments.