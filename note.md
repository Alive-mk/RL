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
$$
给定当前的状态s_t和动作a_t,下一个状态s_{t+1}和奖励r_{t+1}的概率分布，与过去的所有状态和动作
s_{t-1},a_{t-1},\ldots,s_0,a_0都无关。
$$

> The answer is that, once the policy in an `MDP` is fixed, the `MDP` degenerates into an `MP`.
>
> That is because optimal policies are invariant to affine transformations of the rewards.
>
> <img src="pictures\image-20250406231419527.png" alt="image-20250406231419527" style="zoom:67%;" />

# 2. **Chapter 2 State Values and Bellman Equation**

```json
in a nutshell,inequality,aforementioned,comply with,bootstrapping,compactly,identity martix,appropriate,
invertible,notation,constitute,for the sake of simplicity,derivation,substitute,literature,solely,
matrix-vector,elementwise,concisely,nonnegative,convergence,illustrative,rigorous,block diagonal matrix,

```

- bootstrapping--自举
  **Bootstrapping** 是指在强化学习算法中，利用当前的估计值（例如状态值或动作值）来更新自己的估计。这种方法通过借助已有的信息来逐步改进估计，而不是依赖于完全的现实反馈。

  <img src="pictures\image-20250414170726117.png" alt="image-20250414170726117" style="zoom:67%;" />

- Bellman equation
  <img src="pictures\image-20250417103919104.png" alt="image-20250417103919104" style="zoom:67%;" />

  <img src="pictures\image-20250417110415939.png" alt="image-20250417110415939" style="zoom:80%;" />

- the low of total probability
  <img src="pictures\image-20250417104339286.png" alt="image-20250417104339286" style="zoom:80%;" />

- closed-form solution
  <img src="pictures\image-20250417110646817.png" alt="image-20250417110646817" style="zoom: 67%;" />

- iterative solution
  

<img src="pictures\image-20250417110902388.png" alt="image-20250417110902388" style="zoom:67%;" />

- action value
  <img src="pictures\image-20250417112047120.png" alt="image-20250417112047120" style="zoom:67%;" />
  <img src="pictures\image-20250417112114204.png" alt="image-20250417112114204" style="zoom:67%;" />
- 

> we know that different policies may have the same state values.
>
> 

