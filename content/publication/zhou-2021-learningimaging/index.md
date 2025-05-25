---
title: Learning to Address Intra-segment Misclassification in Retinal Imaging
authors:
- Y Zhou
- M Xu
- Y Hu
- H Lin
- J Jacob
- PA Keane
- DC Alexander
date: '2021-09-01'
publishDate: '2025-05-25T17:04:12.275842Z'
publication_types:
- paper-conference
publication: '*Lecture Notes in Computer Science (including subseries Lecture Notes
  in Artificial Intelligence and Lecture Notes in Bioinformatics)*'
doi: 10.1007/978-3-030-87193-2_46
abstract: 'Accurate multi-class segmentation is a long-standing challenge in medical
  imaging, especially in scenarios where classes share strong similarity. Segmenting
  retinal blood vessels in retinal photographs is one such scenario, in which arteries
  and veins need to be identified and differentiated from each other and from the
  background. Intra-segment misclassification, i.e. veins classified as arteries or
  vice versa, frequently occurs when arteries and veins intersect, whereas in binary
  retinal vessel segmentation, error rates are much lower. We thus propose a new approach
  that decomposes multi-class segmentation into multiple binary, followed by a binary-to-multi-class
  fusion network. The network merges representations of artery, vein, and multi-class
  feature maps, each of which are supervised by expert vessel annotation in adversarial
  training. A skip-connection based merging process explicitly maintains class-specific
  gradients to avoid gradient vanishing in deep layers, to favor the discriminative
  features. The results show that, our model respectively improves F1-score by 4.4%,
  5.1%, and 4.2% compared with three state-of-the-art deep learning based methods
  on DRIVE-AV, LES-AV, and HRF-AV data sets. Code: https://github.com/rmaphoh/Learning-AVSegmentation'
---
