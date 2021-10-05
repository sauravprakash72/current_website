---
# weight: 1
title: Mitigating Byzantine Attacks in Federated Learning 
summary: Proposed a novel sampling based approach that applies per client criteria for mitigating Byzantines in the general federated learning setting. 
tags:
- 'Privacy-Preserving and Robust Machine Learning at the Edge'
- 'Foundations of Coded Computing'
date: "2021-07-03T15:00:00Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: DiverseFL framework  
  focal_point: Smart

links:
- name: Preprint
  url: https://arxiv.org/abs/2010.07541v3
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

For mitigating Byzantine behaviors in federated learning (FL), most state-of-the-art approaches, such as Bulyan, tend to leverage the similarity of updates from the benign clients. Typically, any update that differs from the majority of other updates is treated as a Byzantine update. However, in many practical FL scenarios, data is non-IID across clients, thus the updates received from even the benign clients are quite dissimilar. Hence, using similarity based methods result in wasted opportunities to train a model from interesting non-IID data, and also slower model convergence. We propose *DiverseFL* to overcome this challenge in heterogeneous data distribution settings. Rather than comparing each client's update with other client updates to detect Byzantine clients, DiverseFL compares each client's update with a *guiding* update of that client. Any client whose update diverges from its associated guiding update is then tagged as a Byzantine node. The FL server in DiverseFL computes the *guiding* update in every round for each client over a small sample of the client's local data that is received only once before start of the training. However, sharing even a small sample of client's data with the FL server can compromise client's data privacy needs. To tackle this challenge, DiverseFL creates a *Trusted Execution Environment* (TEE)-based enclave to receive each client's sample and to compute its guiding updates. TEE provides a hardware assisted verification and attestation to each client that its data is not leaked outside of TEE. Through experiments involving neural networks, benchmark datasets and popular Byzantine attacks, we demonstrate that DiverseFL not only performs Byzantine mitigation quite effectively, it also *almost matches the performance of OracleSGD*, where the server only aggregates the updates from the benign clients.