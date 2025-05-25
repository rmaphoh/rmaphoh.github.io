---
title: 'AutoMorph: Automated Retinal Vascular Morphology Quantification Via a Deep
  Learning Pipeline'
authors:
- Y Zhou
- SK Wagner
- MA Chia
- A Zhao
- P Woodward-Court
- M Xu
- R Struyven
- DC Alexander
- PA Keane
date: '2022-07-01'
publishDate: '2025-05-25T17:04:12.246420Z'
publication_types:
- article-journal
publication: '*Translational Vision Science & Technology*'
doi: 10.1167/tvst.11.7.12
abstract: 'Purpose: To externally validate a deep learning pipeline (AutoMorph) for
  automated analysis of retinal vascular morphology on fundus photographs. AutoMorph
  has been made publicly available, facilitating widespread research in ophthalmic
  and systemic diseases. Methods: AutoMorph consists of four functional modules: image
  preprocessing, image quality grading, anatomical segmentation (including binary
  vessel, artery/vein, and optic disc/cup segmentation), and vascular morphology feature
  measurement. Image quality grading and anatomical segmentation use the most recent
  deep learning techniques. We employ a model ensemble strategy to achieve robust
  results and analyze the prediction confidence to rectify false gradable cases in
  image quality grading. We externally validate the performance of each module on
  several independent publicly available datasets. Results: The EfficientNet-b4 architecture
  used in the image grading module achieves performance comparable to that of the
  state of the art for EyePACS-Q, with an F1-score of 0.86. The confidence analysis
  reduces the number of images incorrectly assessed as gradable by 76%. Binary vessel
  segmentation achieves an F1-score of 0.73 on AV-WIDE and 0.78 on DR HAGIS. Artery/vein
  scores are 0.66 on IOSTAR-AV, and disc segmentation achieves 0.94 in IDRID. Vascular
  morphology features measured from the AutoMorph segmentation map and expert annotation
  show good to excellent agreement. Conclusions: AutoMorph modules perform well even
  when external validation data show domain differences from training data (e.g.,
  with different imaging devices). This fully automated pipeline can thus allow detailed,
  efficient, and comprehensive analysis of retinal vascular morphology on color fundus
  photographs. Translational Relevance: By making AutoMorph publicly available and
  open source, we hope to facilitate ophthalmic and systemic disease research, particularly
  in the emerging field of oculomics.'
links:
- name: URL
  url: https://doi.org/10.1167/tvst.11.7.12
---
