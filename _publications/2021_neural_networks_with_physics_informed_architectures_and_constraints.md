---
layout: archive
title: "Neural Networks with Physics-Informed Architectures and Constraints for Dynamical Systems Modeling"
permalink: /publication/physics_informed_neural_nodes
author_profile: true
---

Franck Djeumou<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The Learning for Dynamics and Control Conference (L4DC) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://arxiv.org/abs/2109.06407) \| [Code](https://github.com/wuwushrek/physics_constrained_nn)

<img 
src="/images/pinode_results.gif" 
width=600 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. Such a-priori knowledge might arise from physical principles (e.g., conservation laws) or from the system's design (e.g., the Jacobian matrix of a robot), even if large portions of the system dynamics remain unknown. We develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. It represents the system's vector field as a composition of known and unknown functions, the latter of which are parametrized by neural networks. The physics-informed constraints are enforced via the augmented Lagrangian method during the model's training. We experimentally demonstrate the benefits of the proposed approach on a variety of dynamical systems -- including a benchmark suite of robotics environments featuring large state spaces, non-linear dynamics, external forces, contact forces, and control inputs. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset.

<img 
src="/images/pinode_flowchart.png" 
width=1000 >

