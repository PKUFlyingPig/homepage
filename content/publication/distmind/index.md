---
title: 'DistMind: Efficient Resource Disaggregation for Deep Learning Workloads'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Xin Jin
  - Zhihao Bai
  - Zhen Zhang
  - Yibo Zhu
  - admin
  - Xuanzhe Liu

date: "2024-01-01T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

publication: In *IEEE/ACM Transactions on Networking* (CCF-A)
publication_short: In *TON 2024*

abstract: 'Deep learning (DL) systems suffer from low resource
utilization due to (i) the monolithic server model that tightly
couples compute and memory, and (ii) the limited sharing between
different inference applications, and across inference and training,
because of strict service level objectives (SLOs). To address
this problem, we present DistMind, a disaggregated DL system
that enables efficient multiplexing of DL applications with near-
optimal resource utilization. DistMind decouples compute from
host memory, and exposes the abstractions of a GPU pool and a
memory pool, each of which can be independently provisioned.
The key challenge is to dynamically allocate GPU resources to
different applications based on their real-time demands while
meeting strict SLOs. We tackle this challenge by exploiting the
power of high-speed 100Gbps networks, and design three-stage
pipelining, cache-aware load balancing, and DNN-aware sharding
mechanisms based on the characteristics of DL workloads,
to achieve millisecond-scale application loading overhead and
improve system efficiency. We have implemented a prototype of
DistMind and integrated it with PyTorch. Experimental results
on AWS EC2 show that DistMind achieves near 100% resource
utilization, and compared with NVIDIA MPS and Ray, DistMind
improves the throughput by up to 279% and reduces the inference
latency by up to 94%.'

# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://www.computer.org/csdl/journal/nt/5555/01/10414009/1TY3Mx0FKtG'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

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