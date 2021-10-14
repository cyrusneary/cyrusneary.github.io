---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

## <u>Preprints</u>

### Neural Networks with Physics-Informed Architectures and Constraints for Dynamical Systems Modeling
[Paper](https://arxiv.org/abs/2109.06407) | [Code](https://github.com/wuwushrek/physics_constrained_nn)

**Abstract:** Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. Such a-priori knowledge might arise from physical principles (e.g., conservation laws) or from the system's design (e.g., the Jacobian matrix of a robot), even if large portions of the system dynamics remain unknown. We develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. It represents the system's vector field as a composition of known and unknown functions, the latter of which are parametrized by neural networks. The physics-informed constraints are enforced via the augmented Lagrangian method during the model's training. We experimentally demonstrate the benefits of the proposed approach on a variety of dynamical systems -- including a benchmark suite of robotics environments featuring large state spaces, non-linear dynamics, external forces, contact forces, and control inputs. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset.

F. Djeumou, C. Neary, E. Goubault, S. Putot, U. Topcu, *Neural Networks with Physics-Informed Architectures and Constraints for Dynamical Systems Modeling,* 2021. arXiv:2109.06407 [cs.LG].

### Verifiable and Compositional Reinforcement Learning Systems
[Paper](https://arxiv.org/abs/2106.05864) | [Code](https://github.com/cyrusneary/verifiable-compositional-rl)

**Abstract:** We propose a novel framework for verifiable and compositional reinforcement learning (RL) in which a collection of RL sub-systems, each of which learns to accomplish a separate sub-task, are composed to achieve an overall task. The framework consists of a *high-level* model, represented as a parametric Markov decision process (pMDP) which is used to plan and to analyze compositions of sub-systems, and of the collection of *low-level* sub-systems themselves. By defining interfaces between the sub-systems, the framework enables automatic decompositons of task specifications, *e.g., reach a target set of states with a probability of at least 0.95*, into individual sub-task specifications, *i.e. achieve the sub-system's exit conditions with at least some minimum probability, given that its entry conditions are met*. This in turn allows for the independent training and testing of the sub-systems; if they each learn a policy satisfying the appropriate sub-task specification, then their composition is guaranteed to satisfy the overall task specification. Conversely, if the sub-task specifications cannot all be satisfied by the learned policies, we present a method, formulated as the problem of finding an optimal set of parameters in the pMDP, to automatically update the sub-task specifications to account for the observed shortcomings. The result is an iterative procedure for defining sub-task specifications, and for training the sub-systems to meet them. As an additional benefit, this procedure allows for particularly challenging or important components of an overall task to be determined automatically, and focused on, during training. Experimental results demonstrate the presented framework's novel capabilities. A collection of RL sub-systems are trained, using proximal policy optimization algorithms, to navigate different portions of a labyrinth environment. A cross-labyrinth task specification is then decomposed into sub-task specifications. Challenging portions of the labyrinth are automatically avoided if their corresponding sub-systems cannot learn satisfactory policies within allowed training budgets. Other unnecessary sub-systems are not trained at all. The result is a compositional RL system that efficiently learns to satisfy its task specification. 

C. Neary, C. Verginis, M. Cubuktepe, and U. Topcu, *Verifiable and compositional reinforcement learning systems,* 2021. arXiv:2106.05864 [cs.LG].

## <u>Conference Publications</u>

### Reward Machines for Cooperative Multi-Agent Reinforcement Learning
[Paper](https://arxiv.org/abs/2007.01962) | [Presentation](https://slideslive.com/38954933/reward-machines-for-cooperative-multiagent-reinforcement-learning) | [Slides](/files/2021-01-03_RM_MARL_V2.pdf) | [Code](https://github.com/cyrusneary/rm-cooperative-marl) 

**Abstract:** In cooperative multi-agent reinforcement learning, a collection of agents learns to interact in a shared environment to achieve a common goal. We propose the use of reward machines (RM) --- Mealy machines  used as structured representations of reward functions --- to encode the team's task. The proposed novel interpretation of RMs in the multi-agent setting explicitly encodes required teammate interdependencies, allowing the team-level task to be decomposed into sub-tasks for individual agents. We define such a notion of RM decomposition and present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized q-learning algorithm. Furthermore, in the case of undiscounted rewards, we use local value functions to derive lower and upper bounds for the global value function corresponding to the team task. Experimental results in three discrete settings exemplify the effectiveness of the proposed RM decomposition approach, which converges to a successful team policy an order of magnitude faster than a centralized learner and significantly outperforms hierarchical and independent q-learning approaches.

C. Neary, Z. Xu, B. Wu, and U. Topcu, “Reward machines for cooperative multi-agent reinforcement learning,” in *Proceedings of the 20th International Conference on Autonomous Agents and MultiAgent Systems,* ser. AAMAS ’21, Virtual Event, United Kingdom: International Foundation for Autonomous Agents and Multiagent Systems, 2021, pp. 934–942.

### Smooth Convex Optimization Using Sub-Zeroth-Order Oracles
[Paper](https://arxiv.org/abs/2103.00667)

**Abstract:** We consider the problem of minimizing a smooth, Lipschitz, convex function over a compact, convex set using sub-zeroth-order oracles: an oracle that outputs the sign of the directional derivative for a given point and a given direction, an oracle that compares the function values for a given pair of points, and an oracle that outputs a noisy function value for a given point. We show that the sample complexity of optimization using these oracles is polynomial in the relevant parameters. The optimization algorithm that we provide for the comparator oracle is the first algorithm with a known rate of convergence that is polynomial in the number of dimensions. We also give an algorithm for the noisy-value oracle that incurs sublinear regret in the number of queries and polynomial regret in the number of dimensions.

M. O. Karabag, C. Neary, and U. Topcu, “Smooth convex optimization using sub-zeroth-order oracles,” *Proceedings of the AAAI Conference on Artificial Intelligence,* vol. 35, no. 5, pp. 3815–3822, May 2021.

<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->
