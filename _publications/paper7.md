---
title: "Reverse Engineering of Deceptions on Machine- and Human-Centric Attacks"
collection: publications
paper_figure:
  image: /images/papers/paper7-overview.png
  width: 734
  height: 500
  alt: "Adversarial detection returns a binary decision, while reverse engineering also estimates clean content, labels, and attack evidence."
  caption: "One chapter contrasts detecting an adversarial example with recovering information about how it was constructed."
  source: https://doi.org/10.1561/3300000039
  credit: "Figure 2.1 from the authors' full manuscript; this link opens the official publication record"
authors: "Yuguang Yao, Xiao Guo, Vishal Asnani, Yifan Gong, Jiancheng Liu, Xue Lin, Xiaoming Liu, Sijia Liu"
permalink: /publication/paper7
date: 2024-01-01
venue: 'Foundations and Trends in Privacy and Security'
paperurl: 'https://doi.org/10.1561/3300000039'
citation: 'Yao, Y., Guo, X., Asnani, V., Gong, Y., Liu, J., Lin, X., ... & Liu, S. (2024). Reverse Engineering of Deceptions on Machine-and Human-Centric Attacks. Foundations and Trends® in Privacy and Security, 6(2), 53-152.'
---

**Detecting deception is only one part of understanding it.** This tutorial monograph connects attacks on machine-learning systems with synthetic media intended to mislead people, asking what their outputs reveal about the underlying toolchain.

### What it covers

- **Machine-centric attacks:** recovering perturbation evidence, saliency information, and victim-model attributes from adversarial examples.
- **Human-centric attacks:** inferring generative-model properties and localizing manipulated image regions.
- Technical formulations, example pipelines, experiments, and open challenges across those distinct problems.

### A research takeaway

> **Detection, localization, and model parsing answer different questions.** A real-or-fake decision does not by itself identify the altered region or explain the generator and attack process.

The published **Introduction and chapter organization** provide this framing. The figure illustrates the adversarial-example chapter, not one unified method for every deception type.

### Scope and source version

This is a survey/tutorial spanning multiple methods, not a single detector with one meaningful headline accuracy. The figure comes from the **authors' full manuscript, not the publisher-typeset version**. The reading link points to the official published monograph.

### Source

[Published paper](https://doi.org/10.1561/3300000039)
