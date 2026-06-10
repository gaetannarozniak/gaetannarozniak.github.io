---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am Gaëtan, an AI PhD student at Meta and Inria, with a strong interest in AI for Mathematics.
I graduated from École Polytechnique and am currently pursuing my PhD under the supervision of [Gérard Biau](https://perso.lpsm.paris/~biau/), [Pierre Marion](https://pierremarion23.github.io/) and [Rémi Munos](https://researchers.lille.inria.fr/munos/).

I am particularly interested of Reinforcement Learning for Large Language Models, in the domain of formal mathematics.

Publications
======

June 2026: Distilling LLM Feedback for Lean Theorem Proving
------
You can access the full paper on arXiv by clicking [here](https://arxiv.org/abs/2605.30861).

Post-training for reasoning models usually combines supervised fine-tuning with reinforcement learning from verifiable rewards, often using GRPO. But GRPO can struggle with sparse rewards, limited exploration, and mode collapse. We introduce Feedback Distillation, a self-distillation-based training method that teaches a model to match its own token-level distribution when conditioned on privileged feedback from a language model. This gives richer supervision and can incorporate external knowledge. In Lean4 theorem proving, Feedback Distillation produces more diverse reasoning trajectories than GRPO, leading to higher policy entropy and stronger pass@k scaling. The two methods also complement each other: starting GRPO from a Feedback Distillation checkpoint performs better than either approach alone. Overall, the results suggest a promising direction for improving post-training in complex reasoning tasks.

June 2025: Asymmetric REINFORCE for off-Policy Reinforcement Learning
------
You can access the full paper on arXiv by clicking [here](https://arxiv.org/abs/2506.20520).

Overview: We study a simple off-policy REINFORCE method for aligning large language models, where a tunable baseline controls how strongly high- and low-reward samples are weighted.
We show that when this baseline lower-bounds the expected reward, the method has a policy improvement guarantee.
Experiments on stochastic bandits and state-of-the-art LLM reasoning tasks support the theory, suggesting that off-policy learning works best when it emphasizes positive rewards more than negative ones.

Create content & metadata
------
For site content, there is one Markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a Markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each Markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
