---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am Gaëtan, an PhD student at Meta and Inria, with a strong interest in AI for Mathematics.
I graduated from École Polytechnique and am currently pursuing my PhD under the supervision of [Gérard Biau](https://perso.lpsm.paris/~biau/), [Pierre Marion](https://pierremarion23.github.io/) and [Rémi Munos](https://researchers.lille.inria.fr/munos/).

I am particularly interested of Reinforcement Learning for Large Language Models, in the domain of formal mathematics.

Publications
======

June 2026: Distilling LLM Feedback for Lean Theorem Proving
------
You can access the full paper on arXiv by clicking [here](https://arxiv.org/abs/2605.30861).

Overview: Post-training for reasoning models usually combines supervised fine-tuning with reinforcement learning from verifiable rewards, often using GRPO. But GRPO can struggle with sparse rewards, limited exploration, and mode collapse. We introduce Feedback Distillation, a self-distillation-based training method that teaches a model to match its own token-level distribution when conditioned on privileged feedback from a language model. This gives richer supervision and can incorporate external knowledge. In Lean4 theorem proving, Feedback Distillation produces more diverse reasoning trajectories than GRPO, leading to higher policy entropy and stronger pass@k scaling. The two methods also complement each other: starting GRPO from a Feedback Distillation checkpoint performs better than either approach alone. Overall, the results suggest a promising direction for improving post-training in complex reasoning tasks.

June 2025: Asymmetric REINFORCE for off-Policy Reinforcement Learning (Neurips 2025)
------
You can access the full paper on arXiv by clicking [here](https://arxiv.org/abs/2506.20520).

Overview: We study a simple off-policy REINFORCE method for aligning large language models, where a tunable baseline controls how strongly high- and low-reward samples are weighted.
We show that when this baseline lower-bounds the expected reward, the method has a policy improvement guarantee.
Experiments on stochastic bandits and state-of-the-art LLM reasoning tasks support the theory, suggesting that off-policy learning works best when it emphasizes positive rewards more than negative ones.

