---
title: "Tree gradient coding"
# draft: true
# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Amirhossein Reisizadeh
- Saurav Prakash
- Ramtin Pedarsani
- Salman Avestimehr

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2019-09-26"
doi: "10.1109/ISIT.2018.8437860"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE International Symposium on Information Theory (ISIT), 2019*
publication_short: In *ISIT 2019*

abstract: Scaling up distributed machine learning systems face two major bottlenecks -- delays due to stragglers and limited communication bandwidth. Recently, a number of coding theoretic strategies have been proposed for mitigating these bottlenecks. In particular, the Gradient Coding (*GC*) scheme was proposed to speed up distributed gradient descent algorithm in a synchronous master-worker setting by providing robustness to stragglers. A major drawback of the master-worker architecture for distributed learning is however, the bandwidth contention at the master, which can significantly deteriorate the performance as the cluster size increases. In this paper, we propose a new framework named Tree Gradient Coding (*TGC*) for distributed gradient aggregation, which parallelizes communication over a tree topology while providing straggler robustness. As our main contribution, we characterize the minimum computation load for *TGC* for a given tree topology and straggler resiliency, and design a tree gradient coding algorithm that achieves this optimal computation load. Furthermore, we provide results from experiments over Amazon EC2, where *TGC* speeds up the training time by up to $18.8\times$ in comparison to *GC*. 
 


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/8849431'
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
