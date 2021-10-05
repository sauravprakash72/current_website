---
title: Optimal Resource Allocation for Cloud Computing
summary: Developed an efficient approach for load allocation in heterogeneous cloud clusters.
# tags:
# - Heterogeneity
# - Coded Distributed Computing
date: "2019-03-08T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Gains over Amazon Cloud
  focal_point: Smart

links:
- name: ISIT
  url: https://ieeexplore.ieee.org/document/8006961
- name: T-IT
  url: https://ieeexplore.ieee.org/document/8663353 
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

In large-scale distributed computing clusters, such as Amazon EC2, there are several types of "system noise" that can result in major degradation of performance: system failures, bottlenecks due to limited communication bandwidth, latency due to straggler nodes, and so on. There have been recent results that demonstrate the impact of coding for efficient utilization of computation and storage redundancy to alleviate the effect of stragglers and communication bottlenecks in homogeneous clusters. In this paper, we focus on general heterogeneous distributed computing clusters consist of a variety of computing machines with different capabilities. We propose a coding framework for speeding up distributed computing in heterogeneous clusters by trading redundancy for reducing the latency of computation. In particular, we propose heterogeneous coded matrix multiplication (HCMM) algorithm for performing distributed matrix multiplication over heterogeneous clusters that are provably asymptotically optimal for a broad class of processing time distributions. Moreover, we show that HCMM is unboundedly faster than any uncoded scheme that partitions the total workload among the workers. 

To demonstrate how the proposed HCMM scheme can be applied in practice, we provide results from numerical studies and Amazon EC2 experiments comparing HCMM with three benchmark load allocation schemes-uniform uncoded, load-balanced uncoded, and uniform coded. In particular, in our numerical studies, HCMM achieves speedups of up to 73%, 56%, and 42%, respectively, over the three benchmark schemes mentioned earlier. Furthermore, we carry out experiments over Amazon EC2 clusters and demonstrate how HCMM can be combined with rateless codes with nearly linear decoding complexity. In particular, we show that HCMM combined with the Luby transform codes can significantly reduce the overall execution time. HCMM is found to be up to 61%, 46%, and 36% faster than the aforementioned three benchmark schemes, respectively. Additionally, we provide a generalization to the problem of optimal load allocation in heterogeneous settings, where we take into account the monetary costs associated with distributed computing clusters. We argue that HCMM is asymptotically optimal for budget-constrained scenarios as well. In particular, we characterize the minimum possible expected cost associated with a computation task over a given cluster of machines. Furthermore, we develop a heuristic algorithm for (HCMM) load allocation for the distributed implementation of budget-limited computation tasks.