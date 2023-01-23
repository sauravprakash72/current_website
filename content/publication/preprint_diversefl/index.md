---
title: "Secure and Fault Tolerant Decentralized Learning"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Saurav Prakash
- Hanieh Hashemi
- Yongqin Wang 
- Murali Annavaram
- Salman Avestimehr

# Author notes (optional)
# author_notes:
# - "Equal contribution"
# - "Equal contribution"

date: "2022-09-13"
doi: ""

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "arXiv:2010.07541"
publication_short: In *Enclaved AI/ML Workshop 2021, Private AI Research Institute*

abstract: Federated learning (FL) is a promising paradigm for training a global model over data distributed across multiple data owners without centralizing clients' raw data. However, sharing of local model updates can also reveal information of clients' local datasets. Trusted execution environments (TEEs) within the FL server have been recently deployed by companies like Meta for secure aggregation. However, secure aggregation can suffer from error-prone local updates sent by clients that become faulty during training due to underlying device malfunctions. Also, data heterogeneity across clients makes fault mitigation challenging, as even updates from normal clients are dissimilar. Thus, most of the prior fault tolerant methods, which treat any local update differing from the majority of other updates as faulty, perform poorly. We propose DiverseFL to make model aggregation secure as well as robust to faults. In DiverseFL, any client whose local model update diverges from its associated guiding update is tagged as being faulty. To implement our novel per-client criteria for fault mitigation, DiverseFL creates a TEE-based secure enclave within the FL server, which in addition to performing secure aggregation for carrying out the global model update step, securely receives a small representative sample of local data from each client only once before training, and computes guiding updates for each participating client during training. Thus, DiverseFL provides security against privacy leakage as well as robustness against faulty clients. In experiments, DiverseFL consistently achieves significant improvements in absolute test accuracy over prior fault mitigation benchmarks. DiverseFL also performs closely to OracleSGD, where server combines updates only from the normal clients. We also analyze the convergence rate of DiverseFL under non-IID data and standard convexity assumptions.


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2010.07541v5.pdf'
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
