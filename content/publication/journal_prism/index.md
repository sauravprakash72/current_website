---
title: "Overcoming Resource Constraints in Federated Learning: Large Models Can Be Trained with only Weak Clients"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Yue Niu
- Saurav Prakash
- Souvik Kundu
- Sunwoo Lee
- Salman Avestimehr

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2023-10-08"
doi: ""

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *Transactions on Machine Learning Research*
publication_short: In *FL-NeurIPS Workshop, 2022*

abstract: Federated Learning (FL) is emerging as a popular, promising decentralized learning framework that enables collaborative training among clients, with no need to share private data between them or to a centralized server. However, considering many edge clients do not have sufficient computing, memory, or communication  capabilities, federated learning of large models still faces significant bottlenecks. To keep such weak but crucial clients in the loop, prior works either consider a heterogeneous-client setting where clients train models
with different sizes; or offload training to the server. However, the heterogeneous-client setting requires some  clients to train full model, which is not aligned with the resourceconstrained setting; while the latter ones break privacy promises in FL when sharing intermediate representations or labels with the server. To overcome these limitations, in this work, we formulate a realistic, but much less explored, cross-device FL setting in which no client can train a full large model nor is willing to share any intermediate information with the remote server. Under such a formulation, we develop a principal sub-model (PriSM) training methodology to collaboratively train a full large model, while assigning each client a small sub-model that is a probabilistic low-rank approximation to the full server model. When creating sub-models, PriSM first performs a principal kernel analysis in the orthogonal kernel space to obtain importance of each kernel. Then, PriSM adopts a novel importance-aware sampling process to select a subset of kernels (i.e., a kernel with high importance is assigned with a higher sampling probability). This sampling process ensures each sub-model is still a low-rank approximation to the full model, while all sub-models together achieve nearly full coverage on the principal kernels. To further improve memory efficiency while still preserving accuracy, PriSM also exploits low-rank structure in intermediate representations and allows each sub-model to learn only a subset of them. Our evaluations on various datasets and models (CNNs, LSTMs, Transformers) under different resource-constrained settings demonstrate that PriSM yields an accuracy improvement of up to 10% compared to existing works. More importantly, PriSM does not incur significant accuracy degradation compared to full-model training (e.g., only ~2% accuracy drops for ResNet-18/CIFAR-10 when clients train only 0.2x sub-models).  

# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://openreview.net/forum?id=lx1WnkL9fk'
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
