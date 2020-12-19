### Hill Climbing
* Hill climbing is an iterative algorithm that can be used to find the weights $\theta$ for an optimal policy.
* At each iteration,
** We slightly perturb the values of the current best estimate for the weights $\theta_{best}$, to yield a new set of weights.
** These new weights are then used to collect an episode. If the new weights $\theta_{new}$ resulted in higher return than the old weights, then we set $\theta_{best} \leftarrow \theta_{new}$.

### REINFORCE
The pseudocode for REINFORCE is as follows:
* Use the policy $\pi_\theta$ to collect mm trajectories ${ \tau^{(1)}, \tau^{(2)}, \ldots, \tau^{(m)}}$ with horizon $H$. We refer to the $i$-th trajectory as
$\tau^{(i)} = (s_0^{(i)}, a_0^{(i)}, \ldots, s_H^{(i)}, a_H^{(i)}, s_{H+1}^{(i)})$.
* Use the trajectories to estimate the gradient $\nabla_\theta U(\theta) :
\nabla_\theta U(\theta) \approx \hat{g} := \frac{1}{m}\sum_{i=1}^m \sum_{t=0}^{H} \nabla_\theta \log \pi_\theta(a_t^{(i)}|s_t^{(i)}) R(\tau^{(i)})$
* Update the weights of the policy:
$\theta \leftarrow \theta + \alpha \hat{g}$
 
Loop over steps 1-3.


```python

```
