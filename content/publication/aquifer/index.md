---
title: 'Aquifer: Transparent Microsecond-scale Scheduling for vRAN Workloads'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Yunshan Jia
  - admin
  - Meng Wang
  - Jiaqi Gao
  - Pengyu Zhang
  - Xuanzhe Liu
  - Xin Jin

date: "2024-03-01T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['2']

publication: In *IEEE Transactions on Services Computing* (CCF-A)
publication_short: In *TSC 2024*

abstract: 'Virtual Radio Access Network (vRAN) is an emerging approach offered by cloud providers to accelerate 5G services deployment. Despite significant microsecond-scale traffic variations, vRAN instances are provisioned based on peak load to meet strict latency requirements, leading to significant resource waste. Conceivably, vRAN can share CPUs with other applications to increase CPU utilization. Yet, existing sharing solutions require modifications to vRAN source code, hindering their deployment on public clouds. We present Aquifer, a microsecond-scale scheduler providing transparent CPU sharing for vRAN workloads. Our key observation is a common producer-consumer task execution pattern in mainstream vRAN implementations. We exploit this pattern to reclaim CPU cores from worker threads only at the boundary of processing different tasks. This guarantees run-to-completion task processing, which is critical for vRAN to achieve low latency and stability. Aquifer intercepts system calls invoked by vRAN at the OS layer to achieve transparent load monitoring and core reallocation. Aquifer employs a set of system-level optimizations on thread state detection, signal transmission and core selection, which reduces the scheduling cycle to 2 μ s. Experimental results show that Aquifer reclaims up to 88.31% of wasted CPU resources for two mainstream vRAN implementations, FlexRAN and OAI, without any source code modifications.'

# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://ieeexplore.ieee.org/document/10629201'
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