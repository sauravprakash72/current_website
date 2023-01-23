---

title: "Hierarchical coded gradient aggregation for learning at the edge"
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

date: "2020-08-24"
doi: "10.1109/ISIT44484.2020.9174077"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE International Symposium on Information Theory (ISIT), 2020*
publication_short: In *ISIT 2020*

abstract: Client devices at the edge are generating increasingly large amounts of rich data suitable for learning powerful statistical models. However, privacy concerns and heavy communication load make it infeasible to move the client data to a centralized location for training. In many distributed learning setups, client nodes carry out gradient computations on their local data while the central master server receives the local gradients and aggregates them to take the global model update step. To guarantee robustness against *straggling* communication links, we consider a hierarchical setup with $n_e$ clients and $n_h$ reliable helper nodes that are available to aid in gradient aggregation at the master. To achieve resiliency against straggling client-to-helpers links, we propose two approaches leveraging *coded redundancy*. First is the Aligned Repetition Coding (ARC) that repeats gradient components on the helper links, allowing  significant partial aggregations at the helpers, resulting in a helpers-to-master communication load ($C_{HM}$) of $\mathcal{O}(n_h)$. ARC however results in a client-to-helpers communication load ($C_{EH}$) of $\Theta(n_h)$, which is prohibitive for client nodes due to limited and costly bandwidth. We thus propose Aligned Minimum Distance Separable Coding (AMC) that achieves optimal $C_{EH}$ of $\Theta(1)$ for a given resiliency threshold by using MDS code over the gradient components, while achieving a $C_{HM}$ of $\mathcal{O}(n_e)$. 
 


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/abstract/document/9174077'
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
