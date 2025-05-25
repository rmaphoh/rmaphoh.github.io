---
title: 'MisMatch: Calibrated Segmentation via Consistency on Differential Morphological
  Feature Perturbations with Limited Labels'
authors:
- MC Xu
- Y Zhou
- C Jin
- M De Groot
- DC Alexander
- NP Oxtoby
- J Jacob
date: '2023-05-01'
publishDate: '2025-05-25T17:04:12.207211Z'
publication_types:
- article-journal
publication: '*IEEE Transactions on Medical Imaging*'
doi: 10.1109/TMI.2023.3273158
abstract: Semi-supervised learning (SSL) is a promising machine learning paradigm
  to address the ubiquitous issue of label scarcity in medical imaging. The state-of-the-art
  SSL methods in image classification utilise consistency regularisation to learn
  unlabelled predictions which are invariant to input level perturbations. However,
  image level perturbations violate the cluster assumption in the setting of segmentation.
  Moreover, existing image level perturbations are hand-crafted which could be sub-optimal.
  In this paper, we propose MisMatch, a semi-supervised segmentation framework based
  on the consistency between paired predictions which are derived from two differently
  learnt morphological feature perturbations. MisMatch consists of an encoder and
  two decoders. One decoder learns positive attention for foreground on unlabelled
  data thereby generating dilated features of foreground. The other decoder learns
  negative attention for foreground on the same unlabelled data thereby generating
  eroded features of foreground. We normalise the paired predictions of the decoders,
  along the batch dimension. A consistency regularisation is then applied between
  the normalised paired predictions of the decoders. We evaluate MisMatch on four
  different tasks. Firstly, we develop a 2D U-net based MisMatch framework and perform
  extensive cross-validation on a CT-based pulmonary vessel segmentation task and
  show that MisMatch statistically outperforms state-of-the-art semi-supervised methods.
  Secondly, we show that 2D MisMatch outperforms state-of-the-art methods on an MRI-based
  brain tumour segmentation task. We then further confirm that 3D V-net based MisMatch
  outperforms its 3D counterpart based on consistency regularisation with input level
  perturbations, on two different tasks including, left atrium segmentation from 3D
  CT images and whole brain tumour segmentation from 3D MRI images. Lastly, we find
  that the performance improvement of MisMatch over the baseline might originate from
  its better calibration. This also implies that our proposed AI system makes safer
  decisions than the previous methods.
---
