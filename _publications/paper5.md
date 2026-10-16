---
title: "PrObeD: Proactive Object Detection Wrapper"
collection: publications
paper_figure:
  image: /images/papers/paper5-method.png
  width: 1340
  height: 614
  alt: "PrObeD generates an image-dependent template, applies it to the image, recovers the template, and fine-tunes an object detector."
  caption: "An encoder-decoder wrapper learns task-relevant image changes alongside the object detector."
  source: https://proceedings.neurips.cc/paper_files/paper/2023/hash/f5846131aa6a72d1df3bd6d43a4a960b-Abstract-Conference.html
  credit: "Figure 2 from the NeurIPS 2023 proceedings paper"
authors: "Vishal Asnani, Abhinav Kumar, Suya You, Xiaoming Liu"
permalink: /publication/paper5
date: 2023-09-22
venue: 'Thirty-seventh Conference on Neural Information Processing Systems 2023'
paperurl: 'https://proceedings.neurips.cc/paper_files/paper/2023/hash/f5846131aa6a72d1df3bd6d43a4a960b-Abstract-Conference.html'
citation: 'Asnani V., Kumar A., You S., Liu X., (2023). PrObeD: Proactive Object Detection Wrapper. In Thirty-seventh Conference on Neural Information Processing Systems.'
---

**Instead of only changing the detector, can we also learn a better input?** PrObeD wraps object detectors with an image-dependent template generator, aiming to make useful scene information easier to exploit.

### How it works

- An encoder predicts a template for each image rather than sharing one fixed template across all scenes.
- The template transforms the input; a decoder learns to recover it.
- Joint training combines template objectives with the detector's own task loss.

The framework is evaluated for both generic bounding-box detection and camouflaged-object segmentation.

### A reported result

> **38.5 AP with PrObeD versus 37.3 AP without it** for Faster R-CNN + FPN on the **MS-COCO 2017 validation split**, Table 2.

This AP averages over IoU thresholds from 0.50 to 0.95. It is not AP50 or classification accuracy. Camouflaged-object experiments use CAMO, COD10K, and NC4K with separate segmentation metrics.

### Scope

The wrapper requires learned preprocessing and detector fine-tuning; it is not a claim that adding an arbitrary perturbation improves an unchanged detector.

### Sources and resources

The result and protocol are detailed in **Section 4 and Table 2**.

[Published paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/f5846131aa6a72d1df3bd6d43a4a960b-Abstract-Conference.html)
[Supplementary](https://proceedings.neurips.cc/paper_files/paper/2023/file/f5846131aa6a72d1df3bd6d43a4a960b-Supplemental-Conference.pdf)
