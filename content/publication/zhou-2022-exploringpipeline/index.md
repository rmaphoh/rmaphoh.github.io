---
title: Exploring Retinal Vascular Morphology via A Deep Learning Pipeline
authors:
- Y Zhou
- S Wagner
- M Chia
- P Woodward-Court
- D Alexander
- P Keane
date: '2022-05-01'
publishDate: '2025-05-25T17:04:12.260766Z'
publication_types:
- manuscript
abstract: "Purpose : Retinal vascular morphology provides valuable information for
  both ophthalmic disease and systemic disease (termed 'oculomics'), e.g., atherosclerosis
  and diabetes mellitus, in a rapid and non-invasive way. To help recognise high risk
  cases of ophthalmic and systemic disease through observing the changes of retinal
  vascular morphology, we propose a deep learning pipeline to automatically analyse
  the vascular morphology (AutoMorph) which measures 12 kinds of metrics, such as
  vessel calibre and tortuosity.  Methods : AutoMorph consists of four functional
  modules: image pre-processing, image quality grading, anatomical segmentation, including
  binary vessel, artery/vein, and optic disc/cup segmentation, and vascular morphology
  feature measurement. Image quality grading and anatomical segmentation use the most
  recent deep learning techniques and are trained on 12 public datasets, such as DRIVE,
  STARE, and CHASEDB1. We employ model ensemble strategy to achieve robust results
  and analyse the prediction confidence to rectify false gradable cases in image quality
  grading. We quantitatively validate module performance on 6 external publicly available
  datasets including EyePACS image quality dataset (EyePACS-Q), DDR, AV-WIDE, DR-HAGIS,
  IOSTAR-AV, and IDRID datasets.  Results : The EfficientNet-b4 architecture used
  in the image grading module achieves comparable performance to the state-of-the-art
  method in EyePACS-Q, with an F1-score of 0.86. The confidence analysis reduces 76%
  of false gradable images. The binary vessel segmentation module achieves an F1-score
  of 0.73 on AV-WIDE and 0.78 on DR-HAGIS. The artery/vein module scores 0.66 on IOSTAR-AV,
  and optic disc/cup module achieves 0.94 in disc segmentation in IDRID. These results
  verify that AutoMorph performs well in external validation, being quantitatively
  on par or even better than some recent work in internal validation.  Conclusions
  : AutoMorph performs well even when the external validation data shows significant
  difference to the training data, e.g., validation on ultra-wide field retinal photography.
  The fully automatic pipeline integrates recent technical work to facilitate 'oculomics'
  research."
---
