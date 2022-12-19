---
layout: archive
title: "Taylor-Lagrange Neural Ordinary Differential Equations: Toward Fast Training and Evaluation of Neural ODEs"
permalink: /publications/taylor_lagrange_nodes
author_profile: true
---

Franck Djeumou<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Eric Goubault, Sylvie Putot, and Ufuk Topcu<br><span style="font-size:12pt">*The International Joint Conferences on Artificial Intelligence (IJCAI) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://www.ijcai.org/proceedings/2022/0405) \| [Poster](../files/2022_ijcai_poster.pdf) \| [Code](https://github.com/wuwushrek/TayLaNets)

<img 
src="/images/tl_node_bar_charts.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** Neural ordinary differential equations (NODEs) -- parametrizations of differential equations using neural networks -- have shown tremendous promise in learning models of unknown continuous-time dynamical systems from data. However, every forward evaluation of a NODE requires numerical integration of the neural network used to capture the system dynamics, making their training prohibitively expensive. Existing works rely on off-the-shelf adaptive step-size numerical integration schemes, which often require an excessive number of evaluations of the underlying dynamics network to obtain sufficient accuracy for training. By contrast, we accelerate the evaluation and the training of NODEs by proposing a data-driven approach to their numerical integration. The proposed Taylor-Lagrange NODEs (TL-NODEs) use a fixed-order Taylor expansion for numerical integration, while also learning to estimate the expansion's approximation error. As a result, the proposed approach achieves the same accuracy as adaptive step-size schemes while employing only low-order Taylor expansions, thus greatly reducing the computational cost necessary to integrate the NODE. A suite of numerical experiments, including modeling dynamical systems, image classification, and density estimation, demonstrate that TL-NODEs can be trained more than an order of magnitude faster than state-of-the-art approaches, without any loss in performance.


<img 
src="/images/tl_node_flowchart.png" 
width=1000 >
<!-- style="float: right; margin-left: 10px; margin-right: 10px;"> -->