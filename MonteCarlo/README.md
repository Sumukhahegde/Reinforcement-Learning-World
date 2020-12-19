Algorithms that solve the prediction problem determine the value function $v_\pi$​(or $q_\pi$​) corresponding to a policy $\pi$.

<br>
When working with finite MDPs, we can estimate the action-value function $q_\pi$ corresponding to a policy \piπ in a table known as a Q-table. This table has one row for each state and one column for each action. The entry in the ss-th row and aa-th column contains the agent's estimate for expected return that is likely to follow, if the agent starts in state ss, selects action aa, and then henceforth follows the policy $\pi$.
<br>
Each occurrence of the state-action pair $s,as,a (s\in\mathcal{S},a\in\mathcal{A}$ in an episode is called a visit to $s,as,a$.

There are two types of MC prediction methods (for estimating $q_\pi$):
<br>
<br>
First-visit MC estimates $q_\pi(s,a)$ as the average of the returns following only first visits to s,as,a (that is, it ignores returns that are associated to later visits).
<br><br>
Every-visit MC estimates $q_\pi(s,a)$ as the average of the returns following all visits to s,as,a.


```python

```
