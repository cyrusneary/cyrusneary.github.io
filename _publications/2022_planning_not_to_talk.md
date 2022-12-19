---
layout: archive
title: "Planning Not to Talk: Multiagent Systems that are Robust to Communication Loss"
permalink: /publications/planning_not_to_talk
author_profile: true
---

Mustafa O. Karabag<sup>\*</sup>, **Cyrus Neary**<sup>\*</sup>, and Ufuk Topcu<br><span style="font-size:12pt">*The International Conference on Autonomous Agents and Multiagent Systems (AAMAS) 2022*.</span><br><span style="font-size:10pt;"> <sup>*</sup> indicates equal contribution. </span>

[Paper](https://www.ifaamas.org/Proceedings/aamas2022/pdfs/p705.pdf) \| [Code](https://github.com/cyrusneary/multi-agent-comms)

<img 
src="/images/intermittent_comms_labeled.png" 
width=500 
style="float: right; margin-left: 10px; margin-right: 10px;">

**Abstract:** In a cooperative multiagent system, a collection of agents executes a joint policy in order to achieve some common objective. The successful deployment of such systems hinges on the availability of reliable inter-agent communication. However, many sources of potential disruption to communication exist in practice, such as radio interference, hardware failure, and adversarial attacks. In this work, we develop joint policies for cooperative multiagent systems that are robust to potential losses in communication. More specifically, we develop joint policies for cooperative Markov games with reach-avoid objectives. First, we propose an algorithm for the decentralized execution of joint policies during periods of communication loss. Next, we use the total correlation of the state-action process induced by a joint policy as a measure of the intrinsic dependencies between the agents. We then use this measure to lower-bound the performance of a joint policy when communication is lost. Finally, we present an algorithm that maximizes a proxy to this lower bound in order to synthesize minimum-dependency joint policies that are robust to communication loss. Numerical experiments show that the proposed minimum-dependency policies require minimal coordination between the agents while incurring little to no loss in performance; the total correlation value of the synthesized policy is one fifth of the total correlation value of the baseline policy which does not take potential communication losses into account. As a result, the performance of the minimum-dependency policies remains consistently high regardless of whether or not communication is available. By contrast, the performance of the baseline policy decreases by twenty percent when communication is lost.

