# Adaptive Congestion-Aware Routing in Software-Defined Networks Using Reinforcement Learning

## Abstract

Dynamic network congestion in Software-Defined
Networks (SDNs) significantly degrades transmission efficiency
and increases latency which makes the traditional shortest-
path algorithms inadequate. This paper presents an adaptive,
data-driven routing approach which utilizes Deep Reinforcement
Learning to mitigate congestion in highly dynamic and volatile
network simulation environments. A Deep Q-Network (DQN)
agent acts as the SDN control plane, which is trained over 3,000
episodes to dynamically route network packets across a simulated
15-node Waxman graph topology. The proposed Markov Decision
Process (MDP) formulates the state representations using posi-
tional encoding and global congestion snapshots, while the reward
function optimizes the agent’s decisions for minimal latency
and congestion avoidance. The architecture utilizes Experience
Replay and an ϵ-greedy exploration strategy to stabilize the
learning process. The proposed method is evaluated under two
scenarios: a low-congestion environment with 35% probability
of node congestion and a high-congestion environment with
70% probability of node congestion. The experiment results
demonstrate that the DRL agent successfully navigates around
congestion to reach destination nodes, with the high-congestion
scenario unexpectedly giving a more stable and consistent reward
as well as better dynamic test results. The findings highlight
the efficiency of reinforcement learning in dynamic SDN traffic
engineering while also identifying the limitations of a lack of
a dataset for the training purposes but only relying on CPU
generated training scenarios.

## Project Overview

This project is a simulation of a congestion aware adaptive routing reinforcement learning agent that adapts to the congestion in the network and re-routes the traffic to reach the destination node. 

### Requirements

This project requires Python 3.13 and Jupyter Notebook to be installed.

Required Dependencies (installable via notebook):
- networkx
- matplotlib
- numpy
- torch

## Getting Started

Clone this Github Repository using git

```sh
git clone https://github.com/SpaciousCoder78/congestion-aware-sdn.git && cd congestion-aware-sdn
```

Launch the notebook using Jupyter Notebook

```sh
jupyter notebook congestion-aware-sdn.ipynb
```

## License

This project and the source code is licensed under a BSD-2-Clause License.


