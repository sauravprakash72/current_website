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

date: "2018-08-16"
doi: "10.1109/ISIT.2018.8437860"

# # Schedule page publish date (NOT publication's date).
# publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *IEEE International Symposium on Information Theory (ISIT), 2018*
publication_short: In *ISIT 2018*

abstract: Many distributed graph computing systems have been  developed recently for efficient processing of massive graphs. These systems require many messages to be exchanged among computing machines at each step of the computation, making *communication bandwidth* a major performance bottleneck. We present a *coded computing* framework that systematically injects redundancy in the computation phase to enable coding opportunities in the communication phase thus reducing the communication load substantially. Specifically, we propose coded schemes that  enable an inverse-linear trade-off (asymptotically) between *computation load* and *average communication load* for Erdös-Rényi (ER) random graph. The proposed scheme for ER graph is shown to be optimal asymptotically as the graph size $n\rightarrow \infty$. For finite $n$, we demonstrate via numerical analysis that for a given computation load $r$, i.e. when each graph vertex is carefully stored at $r$ servers, the proposed scheme slashes the average communication load by (nearly) $r$. 

 


# # Summary. An optional shortened abstract.
# summary: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis posuere tellus ac convallis placerat. Proin tincidunt magna sed ex sollicitudin condimentum.

# tags: []

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://ieeexplore.ieee.org/document/8437860'
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
