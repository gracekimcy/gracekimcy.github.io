---
layout: paper
id: memorization-clip
categories: papers
permalink: papers/memorization-clip
title: "Captured by Captions: On Memorization and its Mitigation in CLIP Models"
authors: 
  - Wenhao Wang
  - Adam Dziedzic
  - Grace C. Kim
  - Michael Backes
  - Franziska Boenisch
venue: International Conference on Learning Representations
venue-shorthand: ICLR
year: 2025
pdf: https://arxiv.org/abs/2502.07830
selected: false
figure: /images/papers/25-memorization-clip.png
image: /images/papers/25-memorization-clip.png
featured: true
feature-order: 1
feature-title: CLIP Memorization
feature-description: Quantifying and mitigating memorization in CLIP models
bibtex: |-

  @misc{wang2025capturedcaptionsmemorizationmitigation,
      title={Captured by Captions: On Memorization and its Mitigation in CLIP Models}, 
      author={Wenhao Wang and Adam Dziedzic and Grace C. Kim and Michael Backes and Franziska Boenisch},
      year={2025},
      eprint={2502.07830},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2502.07830}, 
  }
  
---

Multi-modal models, such as CLIP, have demonstrated strong performance in aligning visual and textual representations, excelling in tasks like image retrieval and zero-shot classification. Despite this success, the mechanisms by which these models utilize training data, particularly the role of memorization, remain unclear. In uni-modal models, both supervised and self-supervised, memorization has been shown to be essential for generalization. However, it is not well understood how these findings would apply to CLIP, which incorporates elements from both supervised learning via captions that provide a supervisory signal similar to labels, and from self-supervised learning via the contrastive objective. To bridge this gap in understanding, we propose a formal definition of memorization in CLIP (CLIPMem) and use it to quantify memorization in CLIP models. Our results indicate that CLIP's memorization behavior falls between the supervised and self-supervised paradigms, with "mis-captioned" samples exhibiting highest levels of memorization. Additionally, we find that the text encoder contributes more to memorization than the image encoder, suggesting that mitigation strategies should focus on the text domain. Building on these insights, we propose multiple strategies to reduce memorization while at the same time improving utility--something that had not been shown before for traditional learning paradigms where reducing memorization typically results in utility decrease.