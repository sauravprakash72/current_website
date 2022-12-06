---
# weight: 3
title: Secure Large-Scale Serveless Training at the Edge 
summary: Developed a fast and computationally efficient Byzantine robust algorithm that leverages a sequential, memory assisted and performance criteria for training over a logical ring. 
tags:
- 'Privacy-Preserving and Robust Machine Learning at the Edge'
date: "2021-09-16T15:00:00Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""
# weight: 3 

image:
  caption: Basil illustration  
  focal_point: Smart

links:
- name: JSAC
  url: https://ieeexplore.ieee.org/document/9830741
- name: NeurIPS Workshop
  url: https://openreview.net/forum?id=_vj5wbUcgRB 
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
Detection and mitigation of Byzantine behaviors in a decentralized learning setting is a daunting task, especially when the data distribution at the users is heterogeneous. As our main contribution, we propose Basil, a fast and computationally efficient Byzantine robust algorithm for decentralized training systems, which leverages a novel sequential, memory assisted and performance-based criteria for training over a logical ring while filtering the Byzantine users. In the IID dataset distribution setting, we provide the theoretical convergence guarantees of Basil, demonstrating its linear convergence rate. Furthermore, for the IID setting, we experimentally demonstrate that Basil is robust to various Byzantine attacks, including the strong Hidden attack, while providing up to $∼16%$ higher test accuracy over the state-of-the-art Byzantine-resilient decentralized learning approach. Additionally, we generalize Basil to the non-IID dataset distribution setting by proposing Anonymous Cyclic Data Sharing (ACDS), a technique that allows each node to anonymously share a random fraction of its local non-sensitive dataset (e.g., landmarks images) with all other nodes. We demonstrate that Basil alongside ACDS with only $5%$ data sharing provides effective toleration of Byzantine nodes, unlike the state-of-the-art Byzantine robust algorithm that completely fails in the heterogeneous data setting. Finally, to reduce the overall latency of Basil resulting from its sequential implementation over the logical ring, we propose Basil+. In particular, Basil+ provides scalability by enabling Byzantine-robust parallel training across groups of logical rings, and at the same time, it retains the performance gains of Basil due to sequential training within each group. Furthermore, we experimentally demonstrate the scalability gains of Basil+ through different sets of experiments.

