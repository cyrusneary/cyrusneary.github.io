---
layout: archive
title: "A Multifidelity Sim-to-Real Pipeline for Verifiable and Compositional Reinforcement Learning"
permalink: /publications/multifidelity_sim_to_real_rl
author_profile: true
---

Cyrus Neary, Christian Ellis, Aryaman Singh Samyal, Craig Lennon, and Ufuk Topcu<br><span style="font-size:12pt">*The IEEE International Conference on Robotics and Automation (ICRA) 2024*.</span>

[Paper](https://arxiv.org/abs/2312.01249) \| [Poster](../files/2024_icra_poster.pdf)

<img 
src="/images/multifidelity_sim_to_real_rl.gif" 
width=600 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** We propose and demonstrate a compositional framework for training and verifying reinforcement learning (RL) systems within a multifidelity sim-to-real pipeline, in order to deploy reliable and adaptable RL policies on physical hardware. By decomposing complex robotic tasks into component subtasks and defining mathematical interfaces between them, the framework allows for the independent training and testing of the corresponding subtask policies, while simultaneously providing guarantees on the overall behavior that results from their composition. By verifying the performance of these subtask policies using a multifidelity simulation pipeline, the framework not only allows for efficient RL training, but also for a refinement of the subtasks and their interfaces in response to challenges arising from discrepancies between simulation and reality. In an experimental case study we apply the framework to train and deploy a compositional RL system that successfully pilots a Warthog unmanned ground robot.

<img 
src="/images/sim_to_real_rl_pipeline.png" 
width=1000 >