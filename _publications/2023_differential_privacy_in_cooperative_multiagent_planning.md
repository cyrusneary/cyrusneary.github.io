---
layout: archive
title: "Differential Privacy in Cooperative Multiagent Planning"
permalink: /publications/differential_privacy_in_multiagent_planning
author_profile: true
---

Bo Chen<sup>\*</sup>, Calvin Hawkins<sup>\*</sup>, Mustafa O. Karabag<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, Matthew Hale, and Ufuk Topcu<br><span style="font-size:12pt">Under review at *The Conference on Uncertainty in Artificial Intelligence (UAI) 2023*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://arxiv.org/abs/2301.08811) \| [Code](https://github.com/cyrusneary/differential_privacy_in_mas)

<img 
src="/images/differential_privacy_results_screenshot.png" 
width=400 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** Privacy-aware multiagent systems must protect agents' sensitive data while simultaneously ensuring that agents accomplish their shared objectives. Towards this goal, we propose a framework to privatize inter-agent communications in cooperative multiagent decision-making problems. We study sequential decision-making problems formulated as cooperative Markov games with reach-avoid objectives. We apply a differential privacy mechanism to privatize agents' communicated symbolic state trajectories, and analyze tradeoffs between the strength of privacy and the team's performance. For a given level of privacy, this tradeoff is shown to depend critically upon the total correlation among agents' state-action processes. We synthesize policies that are robust to privacy by reducing the value of the total correlation. Numerical experiments demonstrate that the team's performance under these policies decreases by only 6 percent when comparing private versus non-private implementations of communication. By contrast, the team's performance decreases by 88 percent when using baseline policies that ignore total correlation and only optimize team performance.