---
# weight: 1
title: Federated Classification in Hyperbolic Spaces via Secure Aggregation of Convex Hulls 
summary: Proposed the first approach to enable privacy-preserving classification in hyperbolic geometry in the federated setting. 
tags:
- 'Privacy-Preserving and Robust Machine Learning at the Edge'
# - 'Foundations of Coded Computing'
date: "2023-08-14T02:25:48Z"
# date: "2020-08-17T19:02:09-04:00"
# date_end: "2020-04-10T15:00:00Z"
# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Hyperbolic Federated Learning  
  focal_point: Smart

links:
- name: Preprint
  url: https://arxiv.org/abs/2308.06895
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

Hierarchical and tree-like data sets arise in many relevant applications, including language processing, graph data mining, phylogeny and genomics. It is known that tree-like data cannot be embedded into Euclidean spaces of finite dimension with small distortion, and that this problem can be mitigated through the use of hyperbolic spaces. When such data also has to be processed in a distributed and privatized setting, it becomes necessary to work with new federated learning methods tailored to hyperbolic spaces. As an initial step towards the development of the field of federated learning in hyperbolic spaces, we propose the first known approach to federated classification in hyperbolic spaces. Our contributions are as follows. First, we develop distributed versions of convex SVM classifiers for Poincar\'e discs. In this setting, the information conveyed from clients to the global classifier are convex hulls of clusters present in individual client data. Second, to avoid label switching issues, we introduce a number-theoretic approach for label recovery based on the so-called integer $B_h$ sequences. Third, we compute the complexity of the convex hulls in hyperbolic spaces to assess the extent of data leakage; at the same time, in order to limit the communication cost for the hulls, we propose a new quantization method for the Poincar\'e disc coupled with Reed-Solomon-like encoding. Fourth, at the server level, we introduce a new approach for aggregating convex hulls of the clients based on balanced graph partitioning. We test our method on a collection of diverse data sets, including hierarchical single-cell RNA-seq data from different patients distributed across different repositories that have stringent privacy constraints. The classification accuracy of our method is up to ~11\% better than its Euclidean counterpart, demonstrating the importance of privacy-preserving learning in hyperbolic spaces.