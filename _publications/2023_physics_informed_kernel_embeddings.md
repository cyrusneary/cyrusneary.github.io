---
layout: archive
title: "Physics-Informed Kernel Embeddings: Integrating Prior System Knowledge with Data-Driven Control"
permalink: /publications/physics_informed_kernel_embeddings
author_profile: true
---

Adam J. Thorpe<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Franck Djeumou<sup>\*</sup>, Meeko M. K. Oishi, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The American Control Conference (ACC) 2024*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://arxiv.org/abs/2301.03565) \| [Code](https://github.com/ajthor/socks)

<img 
src="/images/rkhs_intro_figure.png" 
width=600 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** Data-driven control algorithms use observations of system dynamics to construct an implicit model for the purpose of control. However, in practice, data-driven techniques often require excessive sample sizes, which may be infeasible in real-world scenarios where only limited observations of the system are available. Furthermore, purely data-driven methods often neglect useful a priori knowledge, such as approximate models of the system dynamics. We present a method to incorporate such prior knowledge into data-driven control algorithms using kernel embeddings, a nonparametric machine learning technique based in the theory of reproducing kernel Hilbert spaces. Our proposed approach incorporates prior knowledge of the system dynamics as a bias term in the kernel learning problem. We formulate the biased learning problem as a least-squares problem with a regularization term that is informed by the dynamics, that has an efficiently computable, closed-form solution. Through numerical experiments, we empirically demonstrate the improved sample efficiency and out-of-sample generalization of our approach over a purely data-driven baseline. We demonstrate an application of our method to control through a target tracking problem with nonholonomic dynamics, and on spring-mass-damper and F-16 aircraft state prediction tasks.

<img 
src="/images/rkhs_results_plot.png" 
width=1000 >