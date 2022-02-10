---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
<!-- <span style="font-size:12pt;"> <sup>*</sup> indicates equal contribution. </span> -->

---

**[Verifiable and Compositional Reinforcement Learning Systems](../_publications/2021_verifiable_and_compositional_rl.md)**

**Cyrus Neary**, Christos Verginis, Murat Cubuktepe, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The International Conference on Automated Planning and Scheduling (ICAPS) 2022*.</span>

<img 
src="/images/compositional_rl.gif" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

We propose a framework for verifiable and compositional reinforcement learning (RL) in which a collection of RL sub-systems -- each of which learns to accomplish a separate sub-task -- are composed to achieve an overall task. By defining interfaces between the sub-systems, the framework enables automatic decompositons of task specifications, *e.g., reach a target set of states with a probability of at least 0.95*, into individual sub-task specifications, *i.e. achieve the sub-system's exit conditions with at least some minimum probability, given that its entry conditions are met*. This in turn allows for the independent training and testing of the sub-systems; if they each learn a policy satisfying the appropriate sub-task specification, then their composition is guaranteed to satisfy the overall task specification.

[Read More](../_publications/2021_verifiable_and_compositional_rl.md) \| [Paper](https://arxiv.org/abs/2106.05864) \| [Code](https://github.com/cyrusneary/verifiable-compositional-rl)

---

**[Taylor-Lagrange Neural Ordinary Differential Equations: Toward Fast Training and Evaluation of Neural ODEs](../_publications/2022_taylor_lagrange_nodes.md)**

Franck Djeumou<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The International Joint Conferences on Artificial Intelligence (IJCAI) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/tl_node_bar_charts.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

We accelerate the training and evaluation of Neural Ordinary Differential Equations (NODEs) by proposing a data-driven approach to their numerical integration. A suite of numerical experiments -- including modeling dynamical systems, image classification, and density estimation -- demonstrate that Taylor-Lagrange NODEs can be trained more than an order of magnitude faster than state-of-the-art approaches, without any loss in performance.
<!-- The proposed Taylor-Lagrange NODEs use a fixed-order Taylor expansion for numerical integration, while also learning to estimate the expansion's approximation error.  -->

[Read More](../_publications/2022_taylor_lagrange_nodes.md) \| [Paper](https://arxiv.org/abs/2201.05715) \| [Code](https://github.com/wuwushrek/TayLaNets)

---

**[Planning Not to Talk: Multiagent Systems that are Robust to Communication Loss](../_publications/2022_planning_not_to_talk.md)**

Mustafa O. Karabag<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/intermittent_comms_labeled.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

In a cooperative multiagent system, a collection of agents executes a joint policy in order to achieve some common objective. The successful deployment of such systems hinges on the availability of reliable inter-agent communication. However, many sources of potential disruption to communication exist in practice -- such as radio interference, hardware failure, and adversarial attacks. In this work, we develop joint policies for cooperative multiagent systems that are robust to potential losses in communication. Numerical experiments show that the proposed minimum-dependency policies require minimal coordination between the agents while incurring little to no loss in performance.

[Read More](../_publications/2022_planning_not_to_talk.md) \| [Paper](https://arxiv.org/abs/2201.06619) \| [Code](https://github.com/cyrusneary/multi-agent-comms)

---

**[Neural Networks with Physics-Informed Architectures and Constraints for Dynamical Systems Modeling](../_publications/2021_neural_networks_with_physics_informed_architectures_and_constraints.md)**

Franck Djeumou<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The Learning for Dynamics and Control Conference (L4DC) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/pinode_results.gif" 
width=550 
style="float: right; margin-left: 10px; margin-right: 10px;">

Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. We accordingly develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset.

<!-- **Abstract:** Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. Such a-priori knowledge might arise from physical principles (e.g., conservation laws) or from the system's design (e.g., the Jacobian matrix of a robot), even if large portions of the system dynamics remain unknown. We develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. It represents the system's vector field as a composition of known and unknown functions, the latter of which are parametrized by neural networks. The physics-informed constraints are enforced via the augmented Lagrangian method during the model's training. We experimentally demonstrate the benefits of the proposed approach on a variety of dynamical systems -- including a benchmark suite of robotics environments featuring large state spaces, non-linear dynamics, external forces, contact forces, and control inputs. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset. -->

[Read More](../_publications/2021_neural_networks_with_physics_informed_architectures_and_constraints.md) \| [Paper](https://arxiv.org/abs/2109.06407) \| [Code](https://github.com/wuwushrek/physics_constrained_nn)

---

**[Reward Machines for Cooperative Multi-Agent Reinforcement Learning](../_publications/2021_rms_for_cooperative_marl.md)**

**Cyrus Neary**, Zhe Xu, Bo Wu, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2021*.</span>

<img 
src="/images/rm_marl.gif" 
width=550 
style="float: right; margin-left: 10px; margin-right: 20px;">

In cooperative multi-agent reinforcement learning, a collection of agents learns to interact in a shared environment to achieve a common goal. We propose the use of reward machines (RMs) to encode the team's task, which allows the team-level task to be automatically decomposed into sub-tasks for individual agents. We present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized Q-learning algorithm and demonstrate its superior sample complexity through two numerical experiments involving three agents and ten agents, respectively.

<!-- The proposed novel interpretation of RMs in the multi-agent setting explicitly encodes required teammate interdependencies, allowing the team-level task to be decomposed into sub-tasks for individual agents. We define such a notion of RM decomposition and present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized q-learning algorithm. Furthermore, in the case of undiscounted rewards, we use local value functions to derive lower and upper bounds for the global value function corresponding to the team task. Experimental results in three discrete settings exemplify the effectiveness of the proposed RM decomposition approach, which converges to a successful team policy an order of magnitude faster than a centralized learner and significantly outperforms hierarchical and independent q-learning approaches. -->

[Read More](../_publications/2021_rms_for_cooperative_marl.md) \| [Paper](https://arxiv.org/abs/2007.01962) \| [Presentation](https://slideslive.com/38954933/reward-machines-for-cooperative-multiagent-reinforcement-learning) \| [Slides](/files/2021-01-03_RM_MARL_V2.pdf) \| [Code](https://github.com/cyrusneary/rm-cooperative-marl) 

--- 

<!--  -->

**[Smooth Convex Optimization Using Sub-Zeroth-Order Oracles](../_publications/2021_smooth_convex_opt_using.md)**

Mustafa O. Karabag, **Cyrus Neary**, and Ufuk Topcu<br><span style="font-size:12pt">*The AAAI Conference on Artificial Intelligence (AAAI) 2021*.</span>

<img 
src="/images/labeled_gradient_pruning.png" 
width=400 
style="float: right; margin-left: 10px; margin-right: 10px;">

We present an algorithm to minimize smooth, Lipschitz, convex functions over a compact, convex sets using sub-zeroth-order oracles: an oracle that outputs the sign of the directional derivative for a given point and a given direction, an oracle that compares the function values for a given pair of points, and an oracle that outputs a noisy function value for a given point. We show that the sample complexity of optimization using these oracles is polynomial in the relevant parameters. We also give an algorithm for the noisy-value oracle that incurs sublinear regret in the number of queries and polynomial regret in the number of dimensions.
<!-- 
<img 
src="/images/sub_zero_opt_algorithm_flowchart.png" 
width=1000 > -->

[Read More](../_publications/2021_smooth_convex_opt_using.md) \| [Paper](https://arxiv.org/abs/2103.00667)



<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->
