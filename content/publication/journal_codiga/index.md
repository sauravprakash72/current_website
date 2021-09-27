---
title: "Coded computing for distributed graph analytics"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Saurav Prakash
- Amirhossein Reisizadeh
- Ramtin Pedarsani
- Salman Avestimehr

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2020-06-03"
doi: "10.1109/TIT.2020.2999675"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE Transactions on Information Theory*
publication_short: In *IEEE Transactions on Information Theory*

abstract: Many distributed computing systems have been developed recently for implementing graph based algorithms such as PageRank over large-scale graph-structured datasets such as social networks. Performance of these systems significantly suffers from *communication bottleneck* as a large number of messages are exchanged among servers at each step of the computation. Motivated by graph based MapReduce, we propose a coded computing framework that leverages computation redundancy to alleviate the communication bottleneck in distributed graph processing. As a key contribution of this work, we develop a novel *coding* scheme that systematically injects structured redundancy in the computation phase to enable *coded* multicasting opportunities during message exchange between servers, reducing the communication load substantially in large-scale graph processing. For theoretical analysis, we consider random graph models, and focus on schemes in which subgraph allocation and Reduce allocation are only dependent on vertex ID while the Shuffle design varies with graph connectivity. Specifically, we prove that our proposed scheme enables an (asymptotically) inverse-linear trade-off between *computation load* and *average communication load* for two popular random graph models -- Erdös-Rényi model, and power law model. Particularly, for a given computation load $r$, (i.e. when each graph vertex is carefully stored at $r$ servers), the proposed scheme slashes the average communication load by (nearly) a multiplicative factor of $r$. Furthermore, for the Erdös-Rényi model, we prove that our proposed scheme is optimal asymptotically as the graph size increases by providing an information-theoretic converse. To illustrate the benefits of our scheme in practice, we implement PageRank over Amazon EC2, using artificial as well as real-world datasets, demonstrating gains of up to 50.8\% in comparison to the conventional PageRank implementation. Additionally, we specialize our coded scheme and extend our theoretical results to two other random graph models -- random bi-partite model, and stochastic block model. Our specialized schemes asymptotically enable inverse-linear trade-offs between computation and communication loads in distributed graph processing for these popular random graph models as well. We complement the achievability results with converse bounds for both of these models.

 


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://arxiv.org/pdf/1801.05522.pdf'
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
