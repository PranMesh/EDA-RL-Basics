# Leaning Reinforcement Learning from Basics-Q Learning
## Overview
This initial project implements a Q-learning agent to solve the Taxi-v3 environment using OpenAI's Gym. The Taxi environment(Taxi V3) simulates a simple grid world where an agent (the taxi) must pick up and drop off passengers at designated locations.
The enviroment is visualised using matplotlib for better understanding .
![Visualisation](images/envVisual.png)

# Algorithm
 Q[state,action] += alpha * (reward + gamma * np.max(Q[next_state]) - Q[state,action])
 I adjusted Values as per my preferences , i.e.
alpha = 0.3 #Learning Rate
gamma = 0.8 #Discount Factor
epsilon = 0.1 #Exploration Rate
and then decayed the value of epsilon.

# Prerequisites 
OpenAI gym 
Matplotlib(render node-rgb_array)
Pygame(if the render node is changed to human )
numpy

# Results 

Total Steps before(random actions):1042 
Total Steps taken after QLearing Implimenation:  16
Smart Taxi Succesfully Dropped the paassenger to its location.

