---
title: "Basil: A Fast and Byzantine-Resilient Approach for Decentralized Training"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Ahmed Roushdy Elkordy
- Saurav Prakash
- Salman Avestimehr

# Author notes (optional)
# author_notes:
# - "Equal contribution"
# - "Equal contribution"

date: "2021-09-16"
doi: ""

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "arXiv:2109.07706"
# publication_short: In *ICW*

abstract: Decentralized (i.e., serverless) learning across a large number of distributed users (e.g., mobile users) has seen a surge of  recent interests. The key advantage of these setups is that they provide privacy for the local data of the users while not requiring a server for coordinating the training. They can, however, suffer substantially from potential Byzantine adversaries in the network who may alter the training process to their benefit. Detection and mitigation of Byzantine behaviors in a decentralized learning setting is a daunting task, especially when the data distribution at the users is heterogeneous. As our  main contribution, we propose *Basil*, a fast and computationally efficient Byzantine robust algorithm for decentralized training systems which is based on sequential training over a ring topology.  In the IID dataset distribution setting, we  experimentally  demonstrate that Basil  is robust to various common Byzantine attacks, such as sign flip and Gaussian attacks, while providing up to ~16% higher test accuracy when compared with state-of-the-art Byzantine resilient decentralized learning. We further provide the theoretical convergence guarantees of  Basil for the IID setting. In particular, we show that  Basil has a linear convergence rate. Finally,  we generalize Basil to the decentralized setting with non-IID dataset distribution. We achieve this by proposing Anonymous Cyclic Data Sharing (ACDS), a technique that allows each node to anonymously share a random fraction of its dataset with all other nodes, and integrating it into Basil. Quite interestingly, we demonstrate that even when each node shares only $5\%$ of its local data through ACDS, not only the test accuracy in the non-IID setting can be increased by up to ~10% in the absence of Byzantine nodes, but also using ACDS on top of Basil  provides  resiliency to Byzantine behaviors. 
 



# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://export.arxiv.org/pdf/2109.07706'
# url_code: ''
# url_dataset: ''
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
# image:
#   caption: 'DiverseFL Implementation Overview'
#   focal_point: ""
#   preview_only: false

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
