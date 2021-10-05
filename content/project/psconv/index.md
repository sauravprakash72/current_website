---
title: Pre-defined Sparsity for Convolutional Neural Networks
summary: Proposed the first approach to reduce footprint of convolutional neural networks via pre-defined sparsity. 
tags:
- 'Other'
# - Coded Distributed Computing
date: "2019-12-05T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Proposed sparsity  
  focal_point: Smart

links:
- name: Allerton
  url: https://ieeexplore.ieee.org/document/8919683 
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

The high demand for computational and storage resources severely impedes the deployment of deep convolutional neural networks (CNNs) in limited resource devices. Recent CNN architectures have proposed reduced complexity versions (e.g,. SuffleNet and MobileNet) but at the cost of modest decreases in accuracy. This paper proposes pSConv, a pre-defined sparse 2D kernel based convolution, which promises significant improvements in the trade-off between complexity and accuracy for both CNN training and inference. To explore the potential of this approach, we have experimented with two widely accepted datasets, CIFAR-10 and Tiny ImageNet, in sparse variants of both the ResNet18 and VGG16 architectures. Our approach shows a parameter count reduction of up to 4.24× with modest degradation in classification accuracy relative to that of standard CNNs. Our approach outperforms a popular variant of ShuffleNet using a variant of ResNet18 with pSConv having 3 × 3 kernels with only four of nine elements not fixed at zero. In particular, the parameter count is reduced by 1.7× for CIFAR-10 and 2.29× for Tiny ImageNet with an increased accuracy of ~ 4%.
