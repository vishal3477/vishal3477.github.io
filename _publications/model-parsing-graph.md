---
title: "Tracing Hyperparameter Dependencies for Model Parsing via Learnable Graph Pooling Network"
collection: publications
paper_figure:
  image: /images/papers/model-parsing-graph-method.png
  width: 1320
  height: 430
  alt: "LGPN extracts generation traces and uses graph pooling and unpooling to predict connected model-hyperparameter attributes."
  caption: "Hyperparameters are treated as related graph nodes rather than independent prediction targets."
  source: https://proceedings.neurips.cc/paper_files/paper/2024/hash/d412468559da4e2ac41a0285b3a079cd-Abstract-Conference.html
  credit: "Figure 2 from the NeurIPS 2024 proceedings paper"
authors: "Xiao Guo, Vishal Asnani, Sijia Liu, Xiaoming Liu"
paperurl: "https://proceedings.neurips.cc/paper_files/paper/2024/hash/d412468559da4e2ac41a0285b3a079cd-Abstract-Conference.html"
permalink: /publication/model-parsing-graph
date: 2024-12-01
venue: "Advances in Neural Information Processing Systems (NeurIPS)"
citation: "Xiao Guo, Vishal Asnani, Sijia Liu, Xiaoming Liu. (2024). Tracing Hyperparameter Dependencies for Model Parsing via Learnable Graph Pooling Network."
---

**Generator attributes are not independent: architecture and training choices often have structure.** This work uses that structure to improve model parsing from generated images.

### How it works

- A Generation Trace Capturing Network extracts cues left by the generating model.
- The Learnable Graph Pooling Network represents hyperparameter values as nodes and dependencies as edges.
- Pooling and unpooling refine those relationships before predicting loss functions and discrete or continuous architecture attributes.

The task covers **37 hyperparameters**: 10 loss-function attributes, 18 discrete architecture attributes, and 9 continuous attributes.

### A reported result

> **79.5% F1 for discrete architecture attributes**, versus **73.0% for FEN-PN**, on **RED140**, Table 1.

The benchmark contains **140,000 generated images from 140 models**. Scores are averaged across the paper's model-held-out evaluations. Loss-function F1 and continuous-attribute error are separate metrics.

### Scope

The predictions concern the attributes defined by the benchmark. They do not recover an arbitrary model's exact weights or complete implementation, and learned dependencies are not proof of causal relationships.

### Source

[Proceedings paper: Sections 3-4 and Table 1](https://proceedings.neurips.cc/paper_files/paper/2024/hash/d412468559da4e2ac41a0285b3a079cd-Abstract-Conference.html)
