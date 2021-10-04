# Data-Science

# Reinforcement Learning

This is my reinforcement learning project where I have used Q-learning and SARSA algorithms to solve 6*6 GridWorld environments.



The environment description is as follows 
# Deterministic Environment
• I have defined a deterministic environment using a grid world of 6*6 which includes a total of 36
states.

• Start position for the agent is [0, 0] and terminal state is [5, 5].

• There are 3 reward positions defined which are [2, 2], [3, 3] and [5, 4] there is no discount factor 
introduced at this point of time. 

• The reward values defined are +25 for position [2,2], +25 for position [3, 3] and +15 for position 
[5, 4]. Terminal state will fetch a reward of +10. The logic behind doing this is as the agent reaches 
closer to the terminal position the higher the reward he will get.

• For deterministic environment I have kept the action set as {up, down, left, right and diagonal} out 
of which one action is chosen at random. Actions are executed 100% of the time once they are 
finalized by agent.

# Stochastic Environment
• The stochastic environment is also defined using a grid world of 6*6 which includes a total of 36
states.

• There are 4 reward positions for the agent.

• Reward position - [2, 2] with reward = +25(Agent needsto reach this hideout within 25-time step
mark otherwise criminal runs away and the reward is vanished).

• Reward position – [5, 4] with reward = +15(Agent needs to reach this hideout by 25-time step mark 
otherwise criminal runs away and reward is vanished).

• Reward position – [3, 3] with reward = +25(Agent needs to reach this hideout by 15-time step mark
otherwise criminal runs away and reward is vanished).

• Reward position – [2, 5] with reward = +10(Agent needs to reach this hideout by 35-time step mark
otherwise criminal runs away and reward is vanished.

• Terminal position gives a reward of +40

• The game stops when agent reaches the terminal state or when maximum time-steps are reached. 
(max_timesteps = 50)

• For the part 2 of the assignment my aim is that agent should catch all the criminals and reach the 
terminal position as fast as possible.
