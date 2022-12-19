---
layout: archive
title: "Reward Machines for Cooperative Multi-Agent Reinforcement Learning"
permalink: /publications/RM_for_cooperative_MARL
author_profile: true
---

**Cyrus Neary**, Zhe Xu, Bo Wu, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2021*.</span>

[Paper](https://www.ifaamas.org/Proceedings/aamas2021/pdfs/p934.pdf) \| [Presentation](https://slideslive.com/38954933/reward-machines-for-cooperative-multiagent-reinforcement-learning) \| [Slides](/files/2021-01-03_RM_MARL_V2.pdf) \| [Code](https://github.com/cyrusneary/rm-cooperative-marl) 

<img 
src="/images/rm_marl.gif" 
width=550 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** In cooperative multi-agent reinforcement learning, a collection of agents learns to interact in a shared environment to achieve a common goal. We propose the use of reward machines (RM) -- Mealy machines  used as structured representations of reward functions -- to encode the team's task. The proposed novel interpretation of RMs in the multi-agent setting explicitly encodes required teammate interdependencies, allowing the team-level task to be decomposed into sub-tasks for individual agents. We define such a notion of RM decomposition and present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized q-learning algorithm. Furthermore, in the case of undiscounted rewards, we use local value functions to derive lower and upper bounds for the global value function corresponding to the team task. Experimental results in three discrete settings exemplify the effectiveness of the proposed RM decomposition approach, which converges to a successful team policy an order of magnitude faster than a centralized learner and significantly outperforms hierarchical and independent q-learning approaches.

