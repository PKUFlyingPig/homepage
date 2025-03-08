---
title: 'DistTrain: Addressing Model and Data Heterogeneity with Disaggregated Training for Multimodal Large Language Models'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Zili Zhang
  - admin
  - Ranchen Ming
  - Hanpeng Hu
  - Jianjian Sun
  - Zheng Ge
  - Yibo Zhu
  - Xin Jin

date: "2024-05-01T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

publication_short: In *Preprint*

abstract: 'Multimodal large language models (LLMs) have demonstrated significant potential in a wide range of AI applications. Yet, training multimodal LLMs suffers from low efficiency and scalability, due to the inherent model heterogeneity and data heterogeneity across different modalities.
We present DistTrain, an efficient and adaptive framework to reform the training of multimodal large language models on large-scale clusters. The core of DistTrain is the disaggregated training technique that exploits the characteristics of multimodal LLM training to achieve high efficiency and scalability. Specifically, it leverages disaggregated model orchestration and disaggregated data reordering to address model and data heterogeneity respectively. We also tailor system optimization for multimodal LLM training to overlap GPU communication and computation. We evaluate DistTrain across different sizes of multimodal LLMs on a large-scale production cluster with thousands of GPUs. The experimental results show that DistTrain achieves 54.7% Model FLOPs Utilization (MFU) when training a 72B multimodal LLM on 1172 GPUs and outperforms Megatron-LM by up to 2.2× on throughput. The ablation study shows the main techniques of DistTrain are both effective and lightweight.'

# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://arxiv.org/pdf/2408.04275'
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