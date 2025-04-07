# 1. **Chapter 1 Basic Concepts**

```json
reinforcement learning,formalize,markov decision processes,grid world,adjacent,intuitive,illustrate,
algorithm,ultimate,detour,trivial,by trial and error,with respect to,scenarios,encounter,step into,
simulation,tabular,mathmatically,indicate,preliminary,deterministic,stochastic,wind gust,apply across,
simplicity,depict,dashed lines,cumulative,immediate reward,diverge,discounted return,criterion,notion,
episode,notably,ingredient,derive,stationary,actuator,invariant,affine,equivalently,trajectory,divergence,
stochastic dynamical systems,
```

<img src="pictures\image-20250406105937675.png" alt="image-20250406105937675" style="zoom:67%;" />

<img src="pictures\image-20250406111116644.png" alt="image-20250406111116644" style="zoom:67%;" /><img src="pictures\image-20250406111611856.png" alt="image-20250406111611856" style="zoom:67%;" />

<img src="pictures\image-20250406111745415.png" alt="image-20250406111745415" style="zoom:67%;" />

<img src="pictures\image-20250406224056652.png" alt="image-20250406224056652" style="zoom:67%;" />



- episodic tasks

  tasks with episodes

- continuing tasks
  have no terminal states

- absorbing states
  the agent never leaves a state once reached.

when we treat the terminal state as a normal state and the reward received at the terminal state is positive, a discount rate must be used to calculate the discounted return to avoid divergence.

<img src="pictures\image-20250407110305445.png" alt="image-20250407110305445" style="zoom:67%;" />

> The answer is that, once the policy in an `MDP` is fixed, the `MDP` degenerates into an `MP`.
>
> That is because optimal policies are invariant to affine transformations of the rewards.
>
> <img src="pictures\image-20250406231419527.png" alt="image-20250406231419527" style="zoom:67%;" />

