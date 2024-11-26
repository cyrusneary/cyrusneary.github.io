---
layout: archive
title: "Featured Publications"
permalink: /publications/
author_profile: true
---
<!-- <span style="font-size:12pt;"> <sup>*</sup> indicates equal contribution. </span> -->

A more complete list of my publications is available [here](https://scholar.google.com/citations?user=z4JrPP0AAAAJ&hl=en&oi=ao).

---

**[A Multifidelity Sim-to-Real Pipeline for Verifiable and Compositional Reinforcement Learning](../_publications/2024_multifidelity_sim_to_real_rl.md)**

Cyrus Neary, Christian Ellis, Aryaman Singh Samyal, Craig Lennon, and Ufuk Topcu<br><span style="font-size:12pt">*The IEEE International Conference on Robotics and Automation (ICRA) 2024*.</span>

<img 
src="/images/multifidelity_sim_to_real_rl.gif" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

We propose and demonstrate a compositional framework for training and verifying reinforcement learning (RL) systems within a multifidelity sim-to-real pipeline, in order to deploy reliable and adaptable RL policies on physical hardware. By decomposing complex robotic tasks into component subtasks and defining mathematical interfaces between them, the framework allows for the independent training and testing of the corresponding subtask policies, while simultaneously providing guarantees on the overall behavior that results from their composition. By verifying the performance of these subtask policies using a multifidelity simulation pipeline, the framework not only allows for efficient RL training, but also for a refinement of the subtasks and their interfaces in response to challenges arising from discrepancies between simulation and reality. In an experimental case study we apply the framework to train and deploy a compositional RL system that successfully pilots a Warthog unmanned ground robot.

[Read More](../_publications/2024_multifidelity_sim_to_real_rl.md) \| [Paper](https://arxiv.org/abs/2312.01249) \| [Poster](../files/2024_icra_poster.pdf)

---

**[How to Learn and Generalize From Three Minutes of Data: Physics-Constrained and Uncertainty-Aware Neural Stochastic Differential Equations](../_publications/2023_how_to_sde_in_3_mins.md)**

Franck Djeumou<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, and Ufuk Topcu<br><span style="font-size:12pt">*The Conference on Robot Learning (CORL) 2023* --- oral presentation.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<!-- src="/images/hexa_fig_8_v2.png"  -->
<img 
src="/images/side_view_figure_8.gif"
width=400
style="float: right; margin-left: 10px; margin-right: 10px;">

We present a framework and algorithms to learn controlled dynamics models using neural stochastic differential equations (SDEs)—SDEs whose drift and diffusion terms are both parametrized by neural networks. We construct the drift term to leverage a priori physics knowledge as inductive bias, and we design the diffusion term to represent a distance-aware estimate of the uncertainty in the learned model’s predictions. The proposed neural SDEs can be evaluated quickly enough for use in model predictive control algorithms, or they can be used as simulators for model-based reinforcement learning. We demonstrate these capabilities through experiments on simulated robotic systems, as well as by using them to model and control a hexacopter’s flight dynamics: A neural SDE trained using only three minutes of manually collected flight data results in a model-based control policy that accurately tracks aggressive trajectories that push the hexacopter’s velocity and Euler angles to nearly double the maximum values observed in the training dataset.

[Read More](../_publications/2023_how_to_sde_in_3_mins.md) \| [Paper](https://arxiv.org/abs/2306.06335) \| [Poster](../files/2023_corl_neuralSDE_poster_cyrus_neary.pdf) \| [Youtube Video](https://youtu.be/Ml_gYWTNay4?si=72k97hgsTt8xdUpy) \| [Data Collection Videos](https://tinyurl.com/29xr5vya)

---

**[Compositional Learning of Dynamical System Models Using Port-Hamiltonian Neural Networks](../_publications/2022_compositional_ph_nodes.md)**

Cyrus Neary and Ufuk Topcu<br><span style="font-size:12pt">*The Learning for Dynamics and Control Conference (L4DC) 2023*.</span>

<img 
src="/images/ph_node_idea_illustration.png" 
width=650 
style="float: right; margin-left: 10px; margin-right: 10px;">

Many dynamical systems -- from robots interacting with their surroundings to large-scale multiphysics systems -- involve a number of interacting subsystems. Toward the objective of learning composite models of such systems from data, we present i) a framework for compositional neural networks, ii) algorithms to train these models, iii) a method to compose the learned models, iv) theoretical results that bound the error of the resulting composite models, and v) a method to learn the composition itself, when it is not known a prior. The end result is a modular approach to learning: neural network submodels are trained on trajectory data generated by relatively simple subsystems, and the dynamics of more complex composite systems are then predicted without requiring additional data generated by the composite systems themselves. We achieve this compositionality by representing the system of interest, as well as each of its subsystems, as a port-Hamiltonian neural network (PHNN) -- a class of neural ordinary differential equations that uses the port-Hamiltonian systems formulation as inductive bias. 

<!-- We compose collections of PHNNs by using the system's physics-informed interconnection structure, which may be known a priori, or may itself be learned from data. We demonstrate the novel capabilities of the proposed framework through numerical examples involving interacting spring-mass-damper systems. Models of these systems, which include nonlinear energy dissipation and control inputs, are learned independently. Accurate compositions are learned using an amount of training data that is negligible in comparison with that required to train a new model from scratch. Finally, we observe that the composite PHNNs enjoy properties of port-Hamiltonian systems, such as cyclo-passivity -- a property that is useful for control purposes.  -->

[Read More](../_publications/2022_compositional_ph_nodes.md) \| [Paper](https://arxiv.org/abs/2212.00893) \| [Poster](../files/2023_l4dc_poster.pdf) \| [Code](https://github.com/cyrusneary/compositional_port_hamiltonian_NNs)

---

**[Differential Privacy in Cooperative Multiagent Planning](../_publications/2023_differential_privacy_in_cooperative_multiagent_planning.md)**

Bo Chen<sup>\*</sup>, Calvin Hawkins<sup>\*</sup>, Mustafa O. Karabag<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, Matthew Hale, and Ufuk Topcu<br><span style="font-size:12pt">*The Conference on Uncertainty in Aritifical Intelligence (UAI) 2023*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/differential_privacy_results_screenshot.png" 
width=400 
style="float: right; margin-left: 10px; margin-right: 10px;">

Privacy-aware multiagent systems must protect agents' sensitive data while simultaneously ensuring that agents accomplish their shared objectives. Towards this goal, we propose a framework to privatize inter-agent communications in cooperative multiagent decision-making problems. More specifically, we apply a differential privacy mechanism to privatize agents' communicated symbolic state trajectories, and analyze tradeoffs between the strength of privacy and the team's performance. For a given level of privacy, this tradeoff is shown to depend critically upon the total correlation among agents' state-action processes. We use this analysis to develop algorithms to synthesize policies that are robust to privacy by reducing the value of the total correlation.

 <!-- Numerical experiments demonstrate that the team's performance under these policies decreases by only \(6\) percent when comparing private versus non-private implementations of communication. By contrast, the team's performance decreases by \(88\) percent when using baseline policies that ignore total correlation and only optimize team performance. -->

[Read More](../_publications/2023_differential_privacy_in_cooperative_multiagent_planning.md) \| [Paper](https://arxiv.org/abs/2301.08811) \| [Code](https://github.com/cyrusneary/differential_privacy_in_mas)

---

**[Physics-Informed Kernel Embeddings: Integrating Prior System Knowledge with Data-Driven Control](../_publications/2023_physics_informed_kernel_embeddings.md)**

Adam J. Thorpe<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, Franck Djeumou<sup>\*</sup>, Meeko M. K. Oishi, and Ufuk Topcu<br><span style="font-size:12pt">*The IEEE American Control Conference (ACC) 2024*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/rkhs_intro_figure.png" 
width=600 
style="float: right; margin-left: 10px; margin-right: 10px;">

Data-driven control algorithms use observations of system dynamics to construct an implicit model for the purpose of control. However, in practice, data-driven techniques often require excessive sample sizes, which may be infeasible in real-world scenarios where only limited observations of the system are available. Furthermore, purely data-driven methods often neglect useful a priori knowledge, such as approximate models of the system dynamics. We present a method to incorporate such prior knowledge into data-driven control algorithms using kernel embeddings, a nonparametric machine learning technique based in the theory of reproducing kernel Hilbert spaces. We demonstrate an application of our method to control through a target tracking problem with nonholonomic dynamics, and on spring-mass-damper and F-16 aircraft state prediction tasks.


<!-- Our proposed approach incorporates prior knowledge of the system dynamics as a bias term in the kernel learning problem. We formulate the biased learning problem as a least-squares problem with a regularization term that is informed by the dynamics, that has an efficiently computable, closed-form solution.  -->
<!-- Through numerical experiments, we empirically demonstrate the improved sample efficiency and out-of-sample generalization of our approach over a purely data-driven baseline.  -->

[Read More](../_publications/2023_physics_informed_kernel_embeddings.md) \| [Paper](https://arxiv.org/abs/2301.03565) \| [Code](https://github.com/ajthor/socks)

---

**[Verifiable and Compositional Reinforcement Learning Systems](../_publications/2021_verifiable_and_compositional_rl.md)**

Cyrus Neary, Christos Verginis, Murat Cubuktepe, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Automated Planning and Scheduling (ICAPS) 2022*.</span>

<img 
src="/images/compositional_rl.gif" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

We propose a framework for verifiable and compositional reinforcement learning (RL) in which a collection of RL sub-systems -- each of which learns to accomplish a separate sub-task -- are composed to achieve an overall task. By defining interfaces between the sub-systems, the framework enables automatic decompositons of task specifications, *e.g., reach a target set of states with a probability of at least 0.95*, into individual sub-task specifications, *i.e. achieve the sub-system's exit conditions with at least some minimum probability, given that its entry conditions are met*. This in turn allows for the independent training and testing of the sub-systems; if they each learn a policy satisfying the appropriate sub-task specification, then their composition is guaranteed to satisfy the overall task specification.

[Read More](../_publications/2021_verifiable_and_compositional_rl.md) \| [Paper](https://ojs.aaai.org/index.php/ICAPS/article/view/19849) \| [Poster](../files/2022_icaps_poster.pdf) \| [Code](https://github.com/cyrusneary/verifiable-compositional-rl)

---

**[Taylor-Lagrange Neural Ordinary Differential Equations: Toward Fast Training and Evaluation of Neural ODEs](../_publications/2022_taylor_lagrange_nodes.md)**

Franck Djeumou<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">*The International Joint Conferences on Artificial Intelligence (IJCAI) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/tl_node_bar_charts.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

We accelerate the training and evaluation of Neural Ordinary Differential Equations (NODEs) by proposing a data-driven approach to their numerical integration. A suite of numerical experiments -- including modeling dynamical systems, image classification, and density estimation -- demonstrate that Taylor-Lagrange NODEs can be trained more than an order of magnitude faster than state-of-the-art approaches, without any loss in performance.
<!-- The proposed Taylor-Lagrange NODEs use a fixed-order Taylor expansion for numerical integration, while also learning to estimate the expansion's approximation error.  -->

[Read More](../_publications/2022_taylor_lagrange_nodes.md) \| [Paper](https://www.ijcai.org/proceedings/2022/0405) \| [Poster](../files/2022_ijcai_poster.pdf) \| [Code](https://github.com/wuwushrek/TayLaNets)

---

**[Planning Not to Talk: Multiagent Systems that are Robust to Communication Loss](../_publications/2022_planning_not_to_talk.md)**

Mustafa O. Karabag<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/intermittent_comms_labeled.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

In a cooperative multiagent system, a collection of agents executes a joint policy in order to achieve some common objective. The successful deployment of such systems hinges on the availability of reliable inter-agent communication. However, many sources of potential disruption to communication exist in practice -- such as radio interference, hardware failure, and adversarial attacks. In this work, we develop joint policies for cooperative multiagent systems that are robust to potential losses in communication. Numerical experiments show that the proposed minimum-dependency policies require minimal coordination between the agents while incurring little to no loss in performance.

[Read More](../_publications/2022_planning_not_to_talk.md) \| [Paper](https://www.ifaamas.org/Proceedings/aamas2022/pdfs/p705.pdf) \| [Code](https://github.com/cyrusneary/multi-agent-comms)

---

**[Neural Networks with Physics-Informed Architectures and Constraints for Dynamical Systems Modeling](../_publications/2021_neural_networks_with_physics_informed_architectures_and_constraints.md)**

Franck Djeumou<sup>\*</sup>, Cyrus Neary<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">*The Learning for Dynamics and Control Conference (L4DC) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

<img 
src="/images/pinode_results.gif" 
width=550 
style="float: right; margin-left: 10px; margin-right: 10px;">

Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. We accordingly develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset.

<!-- **Abstract:** Effective inclusion of physics-based knowledge into deep neural network models of dynamical systems can greatly improve data efficiency and generalization. Such a-priori knowledge might arise from physical principles (e.g., conservation laws) or from the system's design (e.g., the Jacobian matrix of a robot), even if large portions of the system dynamics remain unknown. We develop a framework to learn dynamics models from trajectory data while incorporating a-priori system knowledge as inductive bias. More specifically, the proposed framework uses physics-based side information to inform the structure of the neural network itself, and to place constraints on the values of the outputs and the internal states of the model. It represents the system's vector field as a composition of known and unknown functions, the latter of which are parametrized by neural networks. The physics-informed constraints are enforced via the augmented Lagrangian method during the model's training. We experimentally demonstrate the benefits of the proposed approach on a variety of dynamical systems -- including a benchmark suite of robotics environments featuring large state spaces, non-linear dynamics, external forces, contact forces, and control inputs. By exploiting a-priori system knowledge during training, the proposed approach learns to predict the system dynamics two orders of magnitude more accurately than a baseline approach that does not include prior knowledge, given the same training dataset. -->

[Read More](../_publications/2021_neural_networks_with_physics_informed_architectures_and_constraints.md) \| [Paper](https://proceedings.mlr.press/v168/djeumou22a) \| [Poster](../files/2022_l4dc_poster.pdf) \| [Code](https://github.com/wuwushrek/physics_constrained_nn)

---

**[Multiscale Heterogeneous Optimal Lockdown Control for COVID-19 Using Geographic Information](../_publications/2022_covid_paper.md)**

Cyrus Neary, Murat Cubuktepe, Niklas Lauffer, Xueting Jin, Alexander J. Phillips, Zhe Xu, Daoqin Tong, and Ufuk Topcu<br><span style="font-size:12pt">*Scientific Reports*.</span>

<img 
src="/images/heterogeneous_control_idea.png" 
width=700 
style="float: right; margin-left: 10px; margin-right: 10px;">

We study the problem of synthesizing lockdown policies—schedules of maximum capacities for different types of activity sites—to minimize the number of deceased individuals due to a pandemic within a given metropolitan statistical area (MSA) while controlling the severity of the imposed lockdown. To synthesize and evaluate lockdown policies, we develop a multiscale susceptible, infected, recovered, and deceased model that partitions a given MSA into geographic subregions, and that incorporates data on the behaviors of the populations of these subregions. This modeling approach allows for the analysis of heterogeneous lockdown policies that vary across the different types of activity sites within each subregion of the MSA. We formulate the synthesis of optimal lockdown policies as a nonconvex optimization problem and we develop an iterative algorithm that addresses this nonconvexity through sequential convex programming. 
<!-- We empirically demonstrate the effectiveness of the developed approach by applying it to six of the largest MSAs in the United States. The developed heterogeneous lockdown policies not only reduce the number of deceased individuals by up to 45 percent over a 100 day period in comparison with three baseline lockdown policies that are less heterogeneous, but they also impose lockdowns that are less severe. -->

[Read More](../_publications/2022_covid_paper.md) \| [Paper](https://www.nature.com/articles/s41598-022-07692-5) \| [Code](https://github.com/cyrusneary/multiscaleLockdownCovid19)

---

**[Reward Machines for Cooperative Multi-Agent Reinforcement Learning](../_publications/2021_rms_for_cooperative_marl.md)**

Cyrus Neary, Zhe Xu, Bo Wu, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2021*.</span>

<img 
src="/images/rm_marl.gif" 
width=550 
style="float: right; margin-left: 10px; margin-right: 20px;">

In cooperative multi-agent reinforcement learning, a collection of agents learns to interact in a shared environment to achieve a common goal. We propose the use of reward machines (RMs) to encode the team's task, which allows the team-level task to be automatically decomposed into sub-tasks for individual agents. We present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized Q-learning algorithm and demonstrate its superior sample complexity through two numerical experiments involving three agents and ten agents, respectively.

<!-- The proposed novel interpretation of RMs in the multi-agent setting explicitly encodes required teammate interdependencies, allowing the team-level task to be decomposed into sub-tasks for individual agents. We define such a notion of RM decomposition and present algorithmically verifiable conditions guaranteeing that distributed completion of the sub-tasks leads to team behavior accomplishing the original task. This framework for task decomposition provides a natural approach to decentralized learning: agents may learn to accomplish their sub-tasks while observing only their local state and abstracted representations of their teammates. We accordingly propose a decentralized q-learning algorithm. Furthermore, in the case of undiscounted rewards, we use local value functions to derive lower and upper bounds for the global value function corresponding to the team task. Experimental results in three discrete settings exemplify the effectiveness of the proposed RM decomposition approach, which converges to a successful team policy an order of magnitude faster than a centralized learner and significantly outperforms hierarchical and independent q-learning approaches. -->

[Read More](../_publications/2021_rms_for_cooperative_marl.md) \| [Paper](https://www.ifaamas.org/Proceedings/aamas2021/pdfs/p934.pdf) \| [Presentation](https://slideslive.com/38954933/reward-machines-for-cooperative-multiagent-reinforcement-learning) \| [Slides](/files/2021-01-03_RM_MARL_V2.pdf) \| [Code](https://github.com/cyrusneary/rm-cooperative-marl) 

--- 

<!--  -->

**[Smooth Convex Optimization Using Sub-Zeroth-Order Oracles](../_publications/2021_smooth_convex_opt_using.md)**

Mustafa O. Karabag, Cyrus Neary, and Ufuk Topcu<br><span style="font-size:12pt">*The AAAI Conference on Artificial Intelligence (AAAI) 2021*.</span>

<img 
src="/images/labeled_gradient_pruning.png" 
width=400 
style="float: right; margin-left: 10px; margin-right: 10px;">

We present an algorithm to minimize smooth, Lipschitz, convex functions over a compact, convex sets using sub-zeroth-order oracles: an oracle that outputs the sign of the directional derivative for a given point and a given direction, an oracle that compares the function values for a given pair of points, and an oracle that outputs a noisy function value for a given point. We show that the sample complexity of optimization using these oracles is polynomial in the relevant parameters. We also give an algorithm for the noisy-value oracle that incurs sublinear regret in the number of queries and polynomial regret in the number of dimensions.
<!-- 
<img 
src="/images/sub_zero_opt_algorithm_flowchart.png" 
width=1000 > -->

[Read More](../_publications/2021_smooth_convex_opt_using.md) \| [Paper](https://ojs.aaai.org/index.php/AAAI/article/view/16499)



<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %} -->
