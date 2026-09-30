---
layout: paper
id: transformer-explainer-v2
categories: papers
permalink: papers/transformer-explainer-v2
title: "Transformer Explainer: Learning LLM Transformers with Interactive Visual Explanation and Experimentation"
authors: 
  - Aeree Cho
  - Grace C. Kim
  - Alexander Karpekov
  - Seongmin Lee
  - Alec Helbling
  - Benjamin Hoover
  - Zijie J. Wang
  - Minsuk Kahng
  - Duen Horng Chau

venue: ACM CHI Conference on Human Factors in Computing Systems. 2026.
venue-shorthand: CHI
year: 2026
pdf: https://arxiv.org/abs/2408.04619v2
recording: https://www.youtube.com/watch?v=TFUc41G2ikY
selected: false
figure: 
image: 
featured: false
feature-order: 
feature-title: 
feature-description: 
bibtex: |-

  @inproceedings{cho2026transformer,
      title={Transformer Explainer: Learning LLM Transformers with Interactive Visual Explanation and Experimentation},
      author={Cho, Aeree and Kim, Grace C and Karpekov, Alexander and Lee, Seongmin and Helbling, Alec and Hoover, Benjamin and Wang, Zijie J and Kahng, Minsuk and Chau, Duen Horng},
      booktitle={Proceedings of the 2026 CHI Conference on Human Factors in Computing Systems},
      pages={1--21},
  year={2026}
  }
  
---

The Transformer architecture underpins modern large language models powering state-of-the-art text generation and AI applications. However, its complexity makes it difficult for non-experts to learn. Existing resources often lack interactivity, rely on static descriptions of simplified architectures, or fail to reflect models' behavior with real data. To address this gap, we introduce Transformer Explainer, an interactive visualization tool for non-experts to learn Transformers. The tool integrates an overview illustrating the Transformer's data flow with on-demand explanations that gradually reveal mathematical details. Smooth transitions across abstraction levels highlight the interplay between high-level structures and low-level operations. Running a live GPT-2 instance directly in the browser, Transformer Explainer empowers learners to experiment with custom input and hyperparameters without setup, observing next-token predictions in real time. A 90-participant user study showed that our tool offered significant advantages in improving user understanding and engagement. Transformer Explainer has attracted over 490,000 users.
