---
weight: 0.5
title: Low-Latency Federated Learning in Wireless Edge Networks 
summary: Proposed CodedFedL that injects structured coding redundancy into non-linear federated learning for mitigating stragglers and speeding up training procedure in heterogeneous MEC networks. 
# tags:
# - Heterogeneity
# - Coded Distributed Computing
date: "2020-11-09T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: CodedFedL framework  
  focal_point: Smart

links:
- name: Globecom
  url: https://ieeexplore.ieee.org/document/9024521 
- name: ICML Workshop
  url: https://arxiv.org/abs/2007.03273 
- name: JSAC
  url: https://ieeexplore.ieee.org/document/9252954 

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

Federated learning enables training a global model from data located at the client nodes, without data sharing and moving client data to a centralized server. Performance of federated learning in a multi-access edge computing (MEC) network suffers from slow convergence due to heterogeneity and stochastic fluctuations in compute power and communication link qualities across clients. We propose a novel coded computing framework, CodedFedL, that injects structured coding redundancy into federated learning for mitigating stragglers and speeding up the training procedure. CodedFedL enables coded computing for non-linear federated learning by efficiently exploiting distributed kernel embedding via random Fourier features that transforms the training task into computationally favourable distributed linear regression. Furthermore, clients generate local parity datasets by coding over their local datasets, while the server combines them to obtain the global parity dataset. Gradient from the global parity dataset compensates for straggling gradients during training, and thereby speeds up convergence. For minimizing the epoch deadline time at the MEC server, we provide a tractable approach for finding the amount of coding redundancy and the number of local data points that a client processes during training, by exploiting the statistical properties of compute as well as communication delays. We also characterize the leakage in data privacy when clients share their local parity datasets with the server. Additionally, we analyze the convergence rate and iteration complexity of CodedFedL under simplifying assumptions, by treating CodedFedL as a stochastic gradient descent algorithm. Finally, for demonstrating gains that CodedFedL can achieve in practice, we conduct numerical experiments using practical network parameters and benchmark datasets, in which CodedFedL speeds up the overall training time by up to 15× in comparison to the benchmark schemes.