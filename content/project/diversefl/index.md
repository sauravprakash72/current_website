---
# weight: 1
title: Secure and Fault Tolerant Decentralized Learning 
summary: Proposed a novel sampling based approach that applies per client criteria for mitigating faults in the general federated learning setting. 
tags:
- 'Privacy-Preserving and Robust Machine Learning at the Edge'
- 'Foundations of Coded Computing'
date: "2022-09-13T15:00:00Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: DiverseFL framework  
  focal_point: Smart

links:
- name: Preprint
  url: https://arxiv.org/abs/2010.07541v5
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

Federated learning (FL) is a promising paradigm for training a global model over data distributed across multiple data owners without centralizing clients' raw data. However, sharing of local model updates can also reveal information of clients' local datasets. Trusted execution environments (TEEs) within the FL server have been recently deployed by companies like Meta for secure aggregation. However, secure aggregation can suffer from error-prone local updates sent by clients that become faulty during training due to underlying device malfunctions. Also, data heterogeneity across clients makes fault mitigation challenging, as even updates from normal clients are dissimilar. Thus, most of the prior fault tolerant methods, which treat any local update differing from the majority of other updates as faulty, perform poorly. We propose DiverseFL to make model aggregation secure as well as robust to faults. In DiverseFL, any client whose local model update diverges from its associated guiding update is tagged as being faulty. To implement our novel per-client criteria for fault mitigation, DiverseFL creates a TEE-based secure enclave within the FL server, which in addition to performing secure aggregation for carrying out the global model update step, securely receives a small representative sample of local data from each client only once before training, and computes guiding updates for each participating client during training. Thus, DiverseFL provides security against privacy leakage as well as robustness against faulty clients. In experiments, DiverseFL consistently achieves significant improvements in absolute test accuracy over prior fault mitigation benchmarks. DiverseFL also performs closely to OracleSGD, where server combines updates only from the normal clients. We also analyze the convergence rate of DiverseFL under non-IID data and standard convexity assumptions.