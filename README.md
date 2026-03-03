# Artificial_Intelligence_SaifAlomari_Winter2026
### Saif Alomari

This repository contains Artificial Intelligence projects developed during Winter 2026.  
The focus is on reinforcement learning, intelligent agents, and autonomous decision-making systems.

Each project explores how agents learn through interaction, feedback, and optimization of long-term reward.

---

# 🚀 Project 1: Lunar Lander (Deep Q Learning)

## 📌 Overview

This project implements a Deep Q Network (DQN) agent to solve the **LunarLander-v3** environment from Gymnasium.

The goal is to train an intelligent control policy that allows a lunar lander to safely descend and land between two flags while minimizing crashes and inefficient fuel usage.

The agent learns entirely through reward-based interaction with the environment.

---

## 🧠 Method

The agent is trained using **Deep Q Learning (DQN)**.

Instead of storing Q-values in a lookup table, a neural network approximates the action-value function.  
This enables learning in continuous state environments including:

- Position
- Velocity
- Angle
- Angular velocity

Training stability is improved using:
- Experience replay
- Target network updates
- Controlled exploration decay

---

## ⚙️ Training Configuration

- Maximum timesteps: 600,000  
- Training duration: 2,000 episodes  
- Exploration schedule properly decayed  

An earlier attempt suffered from insufficient exploration decay, resulting in mostly random behavior and average rewards around -150.  
After correcting the training schedule, the agent achieved consistent rewards above 200.

---

## 📈 Learning Behavior

The training process shows clear learning phases:

**Episodes 0–300**  
Highly unstable behavior. Frequent crashes. Strongly negative rewards.

**Episodes 300–1000**  
Gradual stabilization. Partial descent control but inconsistent landings.

**Around Episode 1000**  
Breakthrough phase. Reward transitions from negative to positive.

**Episodes 1300–1800**  
Stable high performance. Moving average reward consistently above 200.

**After Episode 1800**  
Minor instability due to continued exploration, but overall strong performance maintained.

---

## 🏆 Final Evaluation Results

Evaluation performed over 100 deterministic episodes:

- **Mean Reward:** 206.46  
- **Mean Episode Length:** 183.35  

The average reward exceeds 200, demonstrating consistent and reliable landing performance across varying initial conditions.

---

## 🎬 Example Gameplay

### Successful Landing

(Add your GIF or video below)
