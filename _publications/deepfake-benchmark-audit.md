---
title: "What Do Deepfake Benchmarks Measure? An Audit Using Frozen Self-Supervised Representations"
collection: publications
authors: "Samuel Pagon, Yixuan Shen, Vishal Asnani, Feng Liu"
permalink: /publication/deepfake-benchmark-audit
date: 2026-06-01
status: preprint
paper_figure:
  image: /images/papers/deepfake-benchmark-audit-results.png
  width: 1320
  height: 634
  alt: "AIGVDBench AUC varies by frozen V-JEPA2 layer, with ridge and logistic-regression probes compared against reported detector scores."
  caption: "Strong linear-probe performance is used to question what the benchmark rewards, not to claim a universal detector."
  source: https://arxiv.org/abs/2606.26384v1
  credit: "Figure 1 from the June 2026 preprint, version 1"
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2606.26384"
citation: "Samuel Pagon, Yixuan Shen, Vishal Asnani, Feng Liu. (2026). What Do Deepfake Benchmarks Measure? An Audit Using Frozen Self-Supervised Representations. arXiv:2606.26384."
---

**Does a high deepfake-detection score necessarily demonstrate forensic understanding?** This audit asks how much benchmark performance is already available in general-purpose, frozen representations.

### How it works

- Fit linear probes to frozen self-supervised video, image, and audio representations.
- Examine layer-wise and generator-wise performance on contemporary deepfake benchmarks.
- Analyze representation-space geometry to investigate why some target generators are easier to distinguish than others.

The framework is a benchmark diagnostic rather than a proposal for another specialized detector.

### A reported result

> **88.51 macro-average per-generator AUC on AIGVDBench** for a ridge probe on **V-JEPA2 layer 22**, Figure 1 and Section 4.1.1.

AUC is reported on a **0-100 scale**, not as classification accuracy. The figure places this beside the benchmark's reported detector scores, including **89.82 for Effort**; those baseline scores are reported comparisons, not new reruns.

### Scope

This is a **preprint**. Representation geometry is diagnostic, not a causal explanation of detection or evidence of deployment reliability. The MLAAD audio target set is spoof-only, so its metric is spoof recall, not full real-versus-fake accuracy.

### Source

[Preprint v1: Section 4.1.1, Figure 1, and Discussion](https://arxiv.org/abs/2606.26384v1)

[Read the preprint](https://arxiv.org/abs/2606.26384)
