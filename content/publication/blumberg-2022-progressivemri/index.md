---
title: Progressive Subsampling for Oversampled Data - Application to Quantitative
  MRI
authors:
- SB Blumberg
- H Lin
- F Grussu
- Y Zhou
- M Figini
- DC Alexander
date: '2022-09-01'
publishDate: '2025-05-25T17:04:12.268630Z'
publication_types:
- paper-conference
publication: '*Lecture Notes in Computer Science (including subseries Lecture Notes
  in Artificial Intelligence and Lecture Notes in Bioinformatics)*'
doi: 10.1007/978-3-031-16446-0_40
abstract: 'We present PROSUB: PROgressive SUBsampling, a deep learning based, automated
  methodology that subsamples an oversampled data set (e.g. channels of multi-channeled
  3D images) with minimal loss of information. We build upon a state-of-the-art dual-network
  approach that won the MICCAI MUlti-DIffusion (MUDI) quantitative MRI (qMRI) measurement
  sampling-reconstruction challenge, but suffers from deep learning training instability,
  by subsampling with a hard decision boundary. PROSUB uses the paradigm of recursive
  feature elimination (RFE) and progressively subsamples measurements during deep
  learning training, improving optimization stability. PROSUB also integrates a neural
  architecture search (NAS) paradigm, allowing the network architecture hyperparameters
  to respond to the subsampling process. We show PROSUB outperforms the winner of
  the MUDI MICCAI challenge, producing large improvements &gt; 18% MSE on the MUDI
  challenge sub-tasks and qualitative improvements on downstream processes useful
  for clinical applications. We also show the benefits of incorporating NAS and analyze
  the effect of PROSUB’s components. As our method generalizes beyond MRI measurement
  selection-reconstruction, to problems that subsample and reconstruct multi-channeled
  data, our code is [7].'
---
