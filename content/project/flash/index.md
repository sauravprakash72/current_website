---
# weight: 3
title: Lottery Aware Sparse Federated Learning 
summary: Presented methodologies for sparse federated learning for resource constrained edge (both homogeneous and heterogeneous compute budget). 
tags:
- 'Privacy-Preserving and Robust Machine Learning at the Edge'
date: "2022-10-25T15:00:00Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""
# weight: 3 

image:
  caption: FLASH illustration  
  focal_point: Smart

links:
- name: Preprint
  url: https://arxiv.org/abs/2208.13092
- name: NeurIPS Workshop
  url: https://openreview.net/forum?id=XEQSP1zL2gx
# url_code: ""
# url_pdf: ""
# url_slides: ""
# url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

Limited computation and communication capabilities of clients pose significant challenges in federated learning (FL) over resource-limited edge nodes. A potential solution to this problem is to deploy off-the-shelf sparse learning algorithms that train a binary sparse mask on each client with the expectation of training a consistent sparse server mask yielding sparse weight tensors. However, as we investigate in this paper, such naive deployments result in a significant drop in accuracy compared to FL with dense models, especially for clients with limited resource budgets. In particular, our investigations reveal a serious lack of consensus among the trained sparsity masks on clients, which prevents convergence for the server mask and potentially leads to a substantial drop in model performance. Based on such key observations, we propose federated lottery aware sparsity hunting (FLASH), a unified sparse learning framework to make the server win a lottery in terms of yielding a sparse sub-model, able to maintain classification performance under highly resource-limited client settings. Moreover, to support FL on different devices requiring different parameter density, we leverage our findings to present hetero-FLASH, where clients can have different target sparsity budgets based on their device resource limits. Experimental evaluations with multiple models on various datasets (both IID and non-IID) show superiority of our models in closing the gap with unpruned baseline while yielding up to ∼ 10.1% improved accuracy with ∼ 10.26x fewer communication costs, compared to existing alternatives, at similar hyperparameter settings.