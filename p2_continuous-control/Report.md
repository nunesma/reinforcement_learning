# Project report

## Learning algorithm
A Deep deterministic Policy Gradients(DDPG) algorithm was used for solving the environments of project 2 Continuous Control - Multi Agents Version

### About Deep Deterministic Policy Gradient(DDPG)
DDPG is a different kind of actor-critic method. Instead of an actual actor critic, it could be seen as approximate DQN. Because it is used to approximate the maximizer over the Q value of the next state and not as learned baseline. DDPG uses two deep neural networks: Actor, Critic. Actor is used to approximate the optimal policy determiinistically (output is best believed action for any given state). Critic is used to to evaluate the optimal action value function by using the actors best believed action. But it is not straightforward to use in continuous action spaces.

### The deep neural network architecture:
Both Actor and Critic Network were built with 256, 512 nodes in respectively two full connected layes. The batch normalization was inserted after the first hidden layer.

### Parameters used in DQN algorithm:
![episodes](hiperparameters.PNG)

### Plot
![episodes](plot.PNG)

![episodes](training.PNG)

### Conclusion:
The Agent solved the environment in 87 episoode with average score 30.06

### Ideas for future work
- Try Other Algorithms such as
1. Trust Region Policy Optimization (TRPO)
2. Truncated Natural Policy Gradient (TNPG)
3. Proximal Policy Optimization (PPO).
- Tune hyperparameters to find better performance and reduce training time
