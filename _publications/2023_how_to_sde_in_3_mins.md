---
layout: archive
title: "How to Learn and Generalize From Three Minutes of Data: Physcics-Constrained and Uncertainty-Aware Neural Stochastic Differential Equations"
permalink: /publications/how_to_learn_from_three_minutes_of_data
author_profile: true
---

Franck Djeumou<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, and Ufuk Topcu<br><span style="font-size:12pt">*The Conference on Robot Learning (CORL) 2023* --- oral presentation.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://arxiv.org/abs/2306.06335) \| [Poster](../files/2023_corl_neuralSDE_poster_cyrus_neary.pdf) \| [Youtube Video](https://youtu.be/Ml_gYWTNay4?si=72k97hgsTt8xdUpy) \| [Data Collection Videos](https://tinyurl.com/29xr5vya)

<img 
src="/images/side_view_figure_8.gif"
width=400 
style="float: right; margin-left: 10px; margin-right: 10px; max-width:100%; height:auto;">

**Abstract:** We present a framework and algorithms to learn controlled dynamics models using neural stochastic differential equations (SDEs)—SDEs whose drift and diffusion terms are both parametrized by neural networks. We construct the drift term to leverage a priori physics knowledge as inductive bias, and we design the diffusion term to represent a distance-aware estimate of the uncertainty in the learned model’s predictions—it matches the system’s underlying stochasticity when evaluated on states near those from the training dataset, and it predicts highly stochastic dynamics when evaluated on states beyond the training regime. The proposed neural SDEs can be evaluated quickly enough for use in model predictive control algorithms, or they can be used as simulators for model-based reinforcement learning. Furthermore, they make accurate predictions over long time horizons, even when trained on small datasets that cover limited regions of the state space. We demonstrate these capabilities through experiments on simulated robotic systems, as well as by using them to model and control a hexacopter’s flight dynamics: A neural SDE trained using only three minutes of manually collected flight data results in a model-based control policy that accurately tracks aggressive trajectories that push the hexacopter’s velocity and Euler angles to nearly double the maximum values observed in the training dataset.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ml_gYWTNay4?si=UADFQq7R8ZATBHrG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<!-- 
<img 
src="/images/neural_sde_illustration_figure.png" 
width=1000 > -->