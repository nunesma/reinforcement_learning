# Project report

## Learning algorithm
We used Actor/Critic architecture model and MADDPG/DDPG algorithm. We chose DDPG because it averages many trajectories to make noise reduction of model gradient and it isn't worry about
each agent interaction. MADDP is similar to DDPG gradient strategies, but different about the agent reward and penalty definition where it uses use the distance to define reward. We selected normal DDPG to learning the state and action and didn't spend much time changing each agent
reward definition. We only utilized the experience to get information of two agent interaction .

We used replay buffer to get N-step states and actions for continuous control; epsilon-greedy method can help model find convergence weight. We also used Soft update model parameters to help model have part properties of previous network

### The deep neural network architecture:
Both Actor and Critic Network were built with 256, 128 nodes in respectively two full connected layes.

### Parameters used in DQN algorithm:
![episodes](hiperparameters.PNG)

### Plot
![episodes](plot.PNG)

![episodes](training.PNG)

### Conclusion:
The Agent solved the environment in 152 episoode with average score 0.50

### Ideas for future work
- Try Other Algorithms such as
1. Distributed Distributional Deterministic Policy Gradients (D4PG)
2. Asynchronous Advantage Actor-Critic (A3C)
3. Proximal Policy Optimization (PPO)
4. Trust Region Policy Optimization (TRPO)
5. Truncated Natural Policy Gradient (TNPG).
- Tune hyperparameters to find better performance and reduce training time
