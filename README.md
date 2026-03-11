# Artificial_Intelligence_SaifAlomari_Winter2026
### Saif Alomari

This repository contains Artificial Intelligence projects developed during Winter 2026.  
The focus is on reinforcement learning, intelligent agents, and autonomous decision-making systems.

Each project explores how agents learn through interaction, feedback, and optimization of long-term reward.


---

# 🚀 Project 1: Lunar Lander (Deep Q Learning)

This project implements a Deep Q Network (DQN) agent to solve the LunarLander-v3 environment. The agent learns to safely land a spacecraft between designated flags through reward-based interaction with the environment. 

Over the course of training, the model transitions from unstable, crash-prone behavior to consistent and controlled landings, achieving a mean evaluation reward above 200 across 100 test episodes. This project demonstrates practical reinforcement learning applied to autonomous decision-making and control.

---

## 🎬 Agent Behavior Evolution

### Episode 150 – Early Training (Chaotic Behavior)

![Episode 150](Reinforcement_Learning_Luner_Lander/dqn_train-episode-150.gif)

In early training, the agent behaves randomly, fires engines without clear strategy, and frequently crashes.

---

### Episode 1775 – Stable Landing Policy

![Episode 1775](Reinforcement_Learning_Luner_Lander/dqn_train-episode-1775.gif)

After sufficient training, the agent demonstrates controlled descent, stabilized orientation, and consistent landings between the flags.
