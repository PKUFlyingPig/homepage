---
title: 'RLHFuse: Efficient RLHF Training for Large Language Models with Inter- and Intra-Stage Fusion'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Zili Zhang
  - Bingyang Wu
  - Shengyu Liu
  - Yukun Chen
  - Changyi Wan
  - Hanpeng Hu
  - Lei Xia
  - Ranchen Ming
  - Yibo Zhu
  - Xin Jin

date: "2024-09-02T00:00:00Z"
# doi: '10.48550/arXiv.2305.05920'

# Schedule page publish date (NOT publication's date).
# publishDate: '2023'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['3']

publication_short: In *Preprint*

abstract: 'Reinforcement Learning from Human Feedback (RLHF) enhances the alignment between LLMs and human preference. The workflow of RLHF typically involves several models and tasks in a series of distinct stages. Existing RLHF training systems view each task as the smallest execution unit thus overlooking the opportunities for subtask-level optimizations. Due to the intrinsic nature of RLHF training, i.e., the data skewness in the generation stage, and the pipeline bubbles in the training stage, existing RLHF systems suffer from low GPU utilization in production deployments.
RLHFuse breaks the traditional view of RLHF workflow as a composition of individual tasks, splitting each task into finer-grained subtasks, and performing stage fusion to improve GPU utilization. RLHFuse contains two key ideas. First, for generation and inference tasks, RLHFuse splits them into sample-level subtasks, enabling efficient inter-stage fusion to mitigate the original generation bottleneck dominated by long-tailed samples. Second, for training tasks, RLHFuse breaks them into subtasks of micro-batches. By leveraging the intuition that pipeline execution can be essentially complemented by another pipeline, RLHFuse performs intra-stage fusion to concurrently execute these subtasks in the training stage with a fused pipeline schedule, resulting in fewer pipeline bubbles. In addition, RLHFuse incorporates a series of system optimizations tailored for each stage of RLHF, making it efficient and scalable for our internal product usage. We evaluate RLHFuse on various popular LLMs and the results show that RLHFuse increases the training throughput by up to 3.7x, compared to existing state-of-the-art systems.'

# Summary. An optional shortened abstract.
tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org
url_pdf: 'https://www.arxiv.org/pdf/2409.13221'
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