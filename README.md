# Collision Avoidance And Path Detection System
The system employs deep reinforcement learning to create an optimised and efficient navigation system which prevents collisions and detects the best possible path for navigation. A collision avoidance system is an advanced technology that helps prevent accidents by alerting drivers of potential collisions. The system uses sensors, cameras and radar to detect objects in the path of the vehicle, and warns the driver if there is a risk of collision. Reinforcement Learning is a type of machine learning algorithm that learns to solve a multi-level problem by trial and error. The machine is trained on real-life scenarios to make a sequence of decisions. It receives either rewards or penalties for the actions it performs. Its goal is to maximize the total reward.

# Deep Reinforcement Learning
The idea is that an agent, having learned from past experience, understands which actions will lead to maximize a numerical result (reward) in a given time horizon, for any given situation (state). In fact, the typical challenge of many RL problems is to maximize not only the best current reward, but also the best future ones, which can be obtained by influencing future states through actions. The agent must be able to perceive the state of the environment and take actions that will affect it, trying to reach one or more goals related to the accomplishment of a predefined task

![image](https://user-images.githubusercontent.com/113916366/234782956-e15da158-565a-49ac-949a-6cae608bc37f.png)

# Parameters in reinforcement learning

Agent - Agent (A) takes actions that affect the environment.

Action - It is the set of all possible operations/moves the agent can make. The agent makes a decision on which action to take from a set of discrete actions (a).

Environment - The environment takes the agent's present state and action as information and returns the reward to the agent with a new state.

State - A state (S) is a particular situation in which the agent finds itself.                    

Reward (R) - The environment gives feedback by which we determine the validity of the agent’s actions in each state. It is crucial in the scenario of Reinforcement Learning where we want the machine to learn all by itself and the only critic that would help it in learning is the feedback/reward it receives.

Discount factor - Over time, the discount factor modifies the importance of incentives. Given the uncertainty of the future it’s better to add variance to the value estimates. Discount factor helps in reducing the degree to which future rewards affect our value function estimates.

Policy (π) - It decides what action to take in a certain state to maximize the reward.

Value (V)—It measures the optimality of a specific state. It is the expected discounted rewards that the agent collects following the specific policy.

Q-value or action-value - Q Value is a measure of the overall expected reward if the agent (A) is in state (s) and takes action (a), and then plays until the end of the episode according to some policy (π).

# Reinforcement and Reward 
Real-time collision avoidance approach using machine learning is presented for safe human-robot coexistence. More specifically, the collision avoidance problem is tackled with Deep Reinforcement Learning (DRL) techniques, applied to robot manipulators with a workspace invaded by unpredictable obstacles. Since the robotic systems are defined in the continuous space, a Normalized Advantage Function (NAF) model-free algorithm has been used.

NORMALISED ADVANTAGE FUNCTION:
Normalized Advantage Function (NAF) is a method that allows one to enable Q-learning in continuous action spaces with deep neural networks. The idea behind this method is to design the Q-function in a way that its maximum argmax aQ(st,at) can be easily computed during each update.

REWARD FUNCTION:
The reward function is a scalar function defined by the weighted sum of three terms: the distance between the endeffector and the target point, the magnitude of the actions, and the distance of the obstacle from the robot

HYPERPARAMETER TUNING:
The hyperparameters are all the elements that have to be set up in order to adjust the learning environment. The exploration of the policy during the training process is defined by the following list of values:

type of noise D: the type of stochastic process added at each time step to the action, in order to keep exploring the environment; it can be either Brownian or Ornstein-Uhlenbeck noise;

noise scale: scaling factor for noise exploration;

noise decay factor: how quickly does the noise decay during the training episode.

# Simulation results and graphs

![image](https://user-images.githubusercontent.com/113916366/234783899-eb02bb31-5acc-4a60-a818-a6336eca1575.png)



