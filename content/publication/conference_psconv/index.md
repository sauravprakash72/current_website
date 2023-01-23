---

title: "pSConv: A pre-defined sparse kernel based convolution for deep CNNs"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Souvik Kundu
- Saurav Prakash
- Haleh Akrami
- Peter Beerel
- Keith Chugg

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2019-12-05"
doi: "10.1109/ALLERTON.2019.8919683"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *57th Annual Allerton Conference on Communication, Control, and Computing (Allerton), 2019*
publication_short: In *Allerton*

abstract: The high demand for computational and storage resources severely impedes the deployment of deep convolutional neural networks (CNNs) in limited resource devices. Recent CNN architectures have proposed reduced complexity versions (e.g,. SuffleNet and MobileNet) but at the cost of modest decreases in accuracy. This paper proposes pSConv, a pre-defined sparse 2D kernel based convolution, which promises significant improvements in the trade-off between complexity and accuracy for both CNN training and inference. To explore the potential of this approach, we have experimented with two widely accepted datasets, CIFAR-10 and Tiny ImageNet, in sparse variants of both the ResNet18 and VGG16 architectures. Our approach shows a parameter count reduction of up to 4.24× with modest degradation in classification accuracy relative to that of standard CNNs. Our approach outperforms a popular variant of ShuffleNet using a variant of ResNet18 with pSConv having 3 × 3 kernels with only four of nine elements not fixed at zero. In particular, the parameter count is reduced by 1.7× for CIFAR-10 and 2.29× for Tiny ImageNet with an increased accuracy of ~ 4%.


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/8919683'
# url_code: ''
# url_dataset: ''
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ""
  focal_point: ""
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---


<!-- {{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
