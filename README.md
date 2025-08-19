# CS_370
Pirate Pathfinding Agent (Deep Q-Learning)
Summary

This project trains a pirate NPC to find a treasure in an 8×8 maze. I used reinforcement learning with Deep Q-learning and a small neural network. The agent plays many short games and 
learns from feedback. It explores at first, then relies more on what it has learned. A replay buffer helps keep training stable. I tested the result from fixed and random starts and 
checked that it wins from all valid cells. The final policy is fast and reliable for a game loop.

What was provided and what I built

The starter code included the maze environment and the experience replay classes. It also included a Jupyter Notebook with placeholders. I wrote the Deep Q-learning training loop in the 
notebook. I handled state observation, action selection, rewards, saving transitions, sampling from replay, and updating the network. I tuned a few settings: small batch size, several 
training passes per sample, and a step-down in exploration over time. I added quick tests to confirm the agent can win from many different starts.

Connecting this work to computer science

Computer scientists turn ideas into working systems. Here, the idea was “learn from trial and error,” and the system is an agent that finds treasure on its own. This matters because 
reliable automation saves time and scales to many situations. My approach was methodical. I defined the goal and limits then picked a method that fit the problem. I built a minimal
version, tested often, and adjusted when necessary. When the results were a bit noisy, I used clear checks to tell learning from luck. I changed only what the data shows needed changing.
My code was designed to be understandable and testable. I documented assumptions and verified that there was more than one happy path. If this agent affected real users, I would add 
safeguards, monitoring, and fallbacks to protect both the user and the organization.
