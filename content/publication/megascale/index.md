---
title: 'MegaScale: Scaling Large Language Model Training to More Than 10,000 GPUs'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Ziheng Jiang
  - Haibin Lin
  - admin 
  - Qi Huang
  - Yangrui Chen
  - Zhi Zhang
  - Yanghua Peng
  - Xiang Li
  - Cong Xie
  - Shibiao Nong
  - Yulu Jia
  - Sun He
  - Hongmin Chen
  - Zhihao Bai
  - Qi Hou
  - Shipeng Yan 
  - Ding Zhou
  - Yiyao Sheng
  - Zhuo Jiang
  - Haohan Xu
  - Haoran Wei
  - Zhang Zhang
  - Pengfei Nie
  - Leqi Zou
  - Sida Zhao
  - Liang Xiang
  - Zherui Liu
  - Zhe Li
  - Xiaoying Jia
  - Jianxi Ye
  - Xin Jin
  - Xin Liu

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
  - 'Equal contribution'

date: "2024-01-02T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

publication: In *21th USENIX Symposium on Networking Systems Design and Implementation* (CCF-A)
publication_short: In *NSDI 2024*

abstract: 'We present the design, implementation and engineering experience in building and deploying Optimus, a production system for training large language models (LLMs) at the scale of more than 10,000 GPUs. Training LLMs at this scale brings unprecedented challenges to training efficiency and stability. We take a full-stack approach that co-designs the algorithmic and system components across operator optimization, model block and optimizer design, computation and communication overlapping, data pipeline, and network performance tuning. Maintaining high train efficiency throughout the training process (i.e., stability) is an important consideration in production given the long extent of LLM training jobs. Many hard stability issues only emerge at large scale, and deep observability is the key to address them. We develop a set of diagnosis tools to monitor system components and events deep in the stack, identify root causes, and derive effective techniques to achieve fault tolerance and mitigate stragglers. Optimus achieves 55.2% Model FLOPs Utilization (MFU) when training a 175B LLM model on 12,288 GPUs, improving the MFU by 1.34× compared to Megatron-LM. We share our operational experience in identifying and fixing failures and stragglers. We hope by articulating the problems and sharing our experience from a systems perspective, this work can inspire future LLM systems research.'
 
# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://arxiv.org/pdf/2402.15627'
url_code: 'https://github.com/volcengine/veScale'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: 'https://www.usenix.org/system/files/nsdi24_slides-jiang_ziheng.pdf'
url_source: ''
url_video: 'https://www.youtube.com/watch?v=qa6q7J0hVUI'

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