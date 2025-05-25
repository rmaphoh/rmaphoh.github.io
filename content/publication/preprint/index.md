---
title: "Revealing the Impact of Pre-training Data on Medical Foundation Models"
authors:
- Y Zhou
date: "2025-04-03"
doi: "10.21203/rs.3.rs-6080254/v1"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-04-03"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: ""
publication_short: ""

abstract: Medical foundation models (FM), pre-trained on large-scale unlabelled data, have demonstrated robust performance and high efficiency when fine-tuned to various clinically relevant applications. However, the impact of pre-training data on medical FM performance such as generalisability and fairness, which form the foundation in fine-tuned models, remains unexplored. To address this, we sampled two large cohorts from two sites, Moorfields Eye Hospital (UK) and the Shanghai Diabetes Prevention Program (China), each containing 904,170 retinal images for FM pre-training. We developed parallel FMs using identical processes and compared their fairness and generalisability on downstream tasks with publicly available datasets and held-out data from each site. Our results demonstrate that, despite strong generalisability, medical FMs perform significantly better on downstream data that align with the pre-training data in approximately one-third of tasks. Additionally, age is a key metadata factor impacting FM fairness and generalisability in retinal images, whereas sex and ethnicity show no such impact. These findings advocate for an evidence-based approach to pre-training data selection and highlight the importance of transparency even for pre-training data, ultimately enhancing FM capabilities and guiding FM development and customised application in healthcare.

# Summary. An optional shortened abstract.

tags:
- Foundation Model

featured: True

links:
- name: URL
  url: https://www.researchsquare.com/article/rs-6080254/v1



# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: ''
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: example
---

