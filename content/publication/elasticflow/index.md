---
title: 'ElasticFlow: An Elastic Serverless Training Platform for Distributed Deep Learning'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Diandian Gu
  - Yihao Zhao
  - admin
  - Yifan Xiong
  - Zhenhua Han
  - Peng Cheng
  - Fan Yang
  - Gang Huang
  - Xin Jin
  - Xuanzhe Liu

# Author notes (optional)
author_notes:

date: "2023-01-01T00:00:00Z"
# doi: '10.1145/3575693.3575721'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication: In *Proceedings of the 28th ACM International Conference on Architectural Support for Programming Languages and Operating Systems*
publication_short: In *ASPLOS 2023*

abstract: 'This paper proposes ElasticFlow, an elastic serverless training platform for distributed deep learning. ElasticFlow provides a serverless interface with two distinct features: (i) users specify only the deep neural network (DNN) model and hyperparameters for a job, but not the number of GPUs; (ii) users specify the deadline for a job, but not the amount of time to occupy GPUs. In contrast to existing server-centric platforms, ElasticFlow provides performance guarantees in terms of meeting deadlines while alleviating tedious, low-level, and manual resource management for deep learning developers. The characteristics of distributed training introduce two challenges. First, the training throughput scales non-linearly with the number of GPUs. Second, the scaling efficiency is affected by worker placement. To address these challenges, we propose Minimum Satisfactory Share to capture the resource usage of training jobs to meet deadlines, and ElasticFlow performs admission control based on it. We develop a greedy algorithm that dynamically allocates resources to admitted jobs based on diminishing returns. We apply buddy allocation to worker placement to eliminate the effect of topology. Evaluation results on a cluster of 128 GPUs show that ElasticFlow increases the number of jobs that can meet their deadlines by 1.46–7.65× compared to existing solutions.'

# Summary. An optional shortened abstract.
# tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://dl.acm.org/doi/pdf/10.1145/3575693.3575721'
url_code: 'https://github.com/pkusys/ElasticFlow'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: 'https://www.youtube.com/watch?v=99SiHtckGWc'

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