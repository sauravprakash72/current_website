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

date: "2022-07-15"
doi: "10.1109/JSAC.2022.3191347"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE Journal on Selected Areas in Communications*
publication_short: In *IEEE Journal on Selected Areas in Communications*

abstract: Detection and mitigation of Byzantine behaviors in a decentralized learning setting is a daunting task, especially when the data distribution at the users is heterogeneous. As our main contribution, we propose Basil, a fast and computationally efficient Byzantine robust algorithm for decentralized training systems, which leverages a novel sequential, memory assisted and performance-based criteria for training over a logical ring while filtering the Byzantine users. In the IID dataset distribution setting, we provide the theoretical convergence guarantees of Basil, demonstrating its linear convergence rate. Furthermore, for the IID setting, we experimentally demonstrate that Basil is robust to various Byzantine attacks, including the strong Hidden attack, while providing up to  ∼ 16% higher test accuracy over the state-of-the-art Byzantine-resilient decentralized learning approach. Additionally, we generalize Basil to the non-IID dataset distribution setting by proposing Anonymous Cyclic Data Sharing (ACDS), a technique that allows each node to anonymously share a random fraction of its local non-sensitive dataset (e.g., landmarks images) with all other nodes. We demonstrate that Basil alongside ACDS with only 5% data sharing provides effective toleration of Byzantine nodes, unlike the state-of-the-art Byzantine robust algorithm that completely fails in the heterogeneous data setting. Finally, to reduce the overall latency of Basil resulting from its sequential implementation over the logical ring, we propose Basil+. In particular, Basil+ provides scalability by enabling Byzantine-robust parallel training across groups of logical rings, and at the same time, it retains the performance gains of Basil due to sequential training within each group. Furthermore, we experimentally demonstrate the scalability gains of Basil+ through different sets of experiments.




# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/9830741'
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
