---
title: 'Continuous Soft Pseudo-Labeling in ASR '
abstract: Continuous pseudo-labeling (PL) algorithms such as slimIPL have recently
  emerged as a powerful strategy for semi-supervised learning in speech recognition.
  In contrast with earlier strategies that alternated between training a model and
  generating pseudo-labels (PLs) with it, here PLs are generated in end-to-end manner
  as training proceeds, improving training speed and the accuracy of the final model.  PL
  shares a common theme with teacher-student models such as distillation in that a
  teacher model generates targets that need to be mimicked by the student model being
  trained. However, interestingly, PL strategies in general use hard-labels, whereas
  distillation uses the distribution over labels as the target to mimic. Inspired
  by distillation we expect that specifying the whole distribution (aka soft-labels)
  over sequences as the target for unlabeled data, instead of a single best pass pseudo-labeled
  transcript (hard-labels) should improve PL performance and convergence. Surprisingly
  and unexpectedly, we find that soft-labels targets can lead to training divergence,
  with the model collapsing to a degenerate token distribution per frame. We hypothesize
  that the reason this does not happen with hard-labels is that training loss on hard-labels
  imposes sequence-level consistency that keeps the model from collapsing to the degenerate
  solution.  In this paper, we show several experiments that support this hypothesis,
  and experiment with several regularization approaches that can ameliorate the degenerate
  collapse when using soft-labels. These approaches can bring the accuracy of soft-labels
  closer to that of hard-labels, and while they are unable to outperform them yet,
  they serve as a useful framework for further improvements.
layout: inproceedings
series: Proceedings of Machine Learning Research
publisher: PMLR
issn: 2640-3498
id: likhomanenko23a
month: 0
tex_title: 'Continuous Soft Pseudo-Labeling in ASR '
firstpage: 65
lastpage: 84
page: 65-84
order: 65
cycles: false
bibtex_author: Likhomanenko, Tatiana and Collobert, Ronan and Jaitly, Navdeep and
  Bengio, Samy
author:
- given: Tatiana
  family: Likhomanenko
- given: Ronan
  family: Collobert
- given: Navdeep
  family: Jaitly
- given: Samy
  family: Bengio
date: 2023-02-28
address:
container-title: Proceedings on ``I Can't Believe It's Not Better!  - Understanding
  Deep Learning Through Empirical Falsification'' at NeurIPS 2022 Workshops
volume: '187'
genre: inproceedings
issued:
  date-parts:
  - 2023
  - 2
  - 28
pdf: https://proceedings.mlr.press/v187/likhomanenko23a/likhomanenko23a.pdf
extras: []
# Format based on Martin Fenner's citeproc: https://blog.front-matter.io/posts/citeproc-yaml-for-bibliographies/
---
