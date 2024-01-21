---
title: 'AlpaServe: Statistical Multiplexing with Model Parallelism for Deep Learning Serving'

authors:
  - Zhuohan Li
  - Lianmin Zheng
  - admin
  - Vincent Liu
  - Ying Sheng
  - Xin Jin
  - Yanping Huang
  - Zhifeng Chen
  - Hao Zhang
  - Joseph E. Gonzalez
  - Ion Stoica

author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'

date: "2023-04-01T00:00:00Z"
# doi: '10.48550/arXiv.2302.11665'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *17th USENIX Symposium on Operating Systems Design and Implementation* (CCF-A)
publication_short: In *OSDI 2023*

abstract: 'Model parallelism is conventionally viewed as a method to scale a single large deep learning model beyond the memory limits of a single device. In this paper, we demonstrate that model parallelism can be additionally used for the statistical multiplexing of multiple devices when serving multiple models, even when a single model can fit into a single device. Our work reveals a fundamental trade-off between the overhead introduced by model parallelism and the opportunity to exploit statistical multiplexing to reduce serving latency in the presence of bursty workloads. We explore the new trade-off space and present a novel serving system, AlpaServe, that determines an efficient strategy for placing and parallelizing collections of large deep learning models across a distributed cluster. Evaluation results on production workloads show that AlpaServe can process requests at up to 10x higher rates or 6x more burstiness while staying within latency constraints for more than 99% of requests.'

# Summary. An optional shortened abstract.
# tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://arxiv.org/pdf/2302.11665.pdf'
url_code: 'https://github.com/alpa-projects/mms'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://www.usenix.org/conference/osdi23/presentation/li-zhouhan'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# image:
#   caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
#   focal_point: ''
#   preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
# projects:
#   - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---