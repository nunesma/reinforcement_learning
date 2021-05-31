# Deep Q-Network (DQN)


This repository contains material related to Deep Q-Network (DQN) algorithm. <br><br>

The DQN algorithm attempts to find a policy π which maps a given state to an action such that it maximizes the expected reward of the agent from some starting state. <br><br>

DQN obtains π implicitly by calculating a state-value function Q(s,a) parameterized by θ, which measures the goodness of the given state-action with respect to some behavioral policy. State-action values, or state-values for that matter, don’t make sense unless they are also attached to some policy.  <br><br>

The Deep Q-Networks (DQN) algorithm was suggested by Mnih et al. It combines the Q-Learning algorithm with deep neural networks (DNNs). They are used to approximate the Q-function, replacing the need for a table to store the Q-values. <br><br>

### Table of contents:
- 1-Deep_Q_Network: Explore how to use a Deep Q-Network (DQN) to navigate a space vehicle without crashing.
- 2-Lunas Lander project: you will implement Deep Q-Learning to solve OpenAI Gym's LunarLander environment. 
