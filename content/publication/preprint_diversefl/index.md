---
title: "Byzantine-Resilient Federated Learning with Heterogeneous Data Distribution"
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

date: "2021-07-03"
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
# publication_short: In *ICW*

abstract: For mitigating Byzantine behaviors in federated learning (FL), most state-of-the-art approaches, such as Bulyan, tend to leverage the similarity of updates from the benign clients. Typically, any update that differs from the majority of other updates is treated as a Byzantine update. However, in many practical FL scenarios, data is non-IID across clients, thus the updates received from even the benign clients are quite dissimilar. Hence, using similarity based methods result in wasted opportunities to train a model from interesting non-IID data, and also slower model convergence. We propose *DiverseFL* to overcome this challenge in heterogeneous data distribution settings. Rather than comparing each client's update with other client updates to detect Byzantine clients, DiverseFL compares each client's update with a *guiding* update of that client. Any client whose update diverges from its associated guiding update is then tagged as a Byzantine node. The FL server in DiverseFL computes the *guiding* update in every round for each client over a small sample of the client's local data that is received only once before start of the training. However, sharing even a small sample of client's data with the FL server can compromise client's data privacy needs. To tackle this challenge, DiverseFL creates a *Trusted Execution Environment* (TEE)-based enclave to receive each client's sample and to compute its guiding updates. TEE provides a hardware assisted verification and attestation to each client that its data is not leaked outside of TEE. Through experiments involving neural networks, benchmark datasets and popular Byzantine attacks, we demonstrate that DiverseFL not only performs Byzantine mitigation quite effectively, it also *almost matches the performance of OracleSGD*, where the server only aggregates the updates from the benign clients.


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/2010.07541.pdf'
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
