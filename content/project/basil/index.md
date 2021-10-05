---
weight: 3
title: Secure Large-Scale Serveless Training at the Edge 
summary: Developed a fast and computationally efficient Byzantine robust algorithm that leverages a sequential, memory assisted and performance criteria for training over a logical ring. 
# tags:
# - Heterogeneity
# - Coded Distributed Computing
lastmod: "2021-09-16T15:00:00Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""
# weight: 3 
image:
  caption: Basil illustration  
  focal_point: Smart

links:
- name: Preprint
  url: https://arxiv.org/abs/2109.07706v1
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

Decentralized (i.e., serverless) learning across a large number of distributed users (e.g., mobile users) has seen a surge of  recent interests. The key advantage of these setups is that they provide privacy for the local data of the users while not requiring a server for coordinating the training. They can, however, suffer substantially from potential Byzantine adversaries in the network who may alter the training process to their benefit. Detection and mitigation of Byzantine behaviors in a decentralized learning setting is a daunting task, especially when the data distribution at the users is heterogeneous. As our  main contribution, we propose *Basil*, a fast and computationally efficient Byzantine robust algorithm for decentralized training systems which is based on sequential training over a ring topology.  In the IID dataset distribution setting, we  experimentally  demonstrate that Basil  is robust to various common Byzantine attacks, such as sign flip and Gaussian attacks, while providing up to ~16% higher test accuracy when compared with state-of-the-art Byzantine resilient decentralized learning. We further provide the theoretical convergence guarantees of  Basil for the IID setting. In particular, we show that  Basil has a linear convergence rate. Finally,  we generalize Basil to the decentralized setting with non-IID dataset distribution. We achieve this by proposing Anonymous Cyclic Data Sharing (ACDS), a technique that allows each node to anonymously share a random fraction of its dataset with all other nodes, and integrating it into Basil. Quite interestingly, we demonstrate that even when each node shares only $5\%$ of its local data through ACDS, not only the test accuracy in the non-IID setting can be increased by up to ~10% in the absence of Byzantine nodes, but also using ACDS on top of Basil  provides  resiliency to Byzantine behaviors. 