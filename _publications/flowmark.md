---
title: "FlowMark: Mask-Guided Video Watermarking"
collection: publications
authors: "Vishal Asnani, Shruti Agarwal, John Collomosse"
permalink: /publication/flowmark
date: 2026-07-01
status: preprint
paper_figure:
  image: /images/papers/flowmark-method.png
  width: 1120
  height: 407
  alt: "FlowMark architecture: learned mask prediction, region-aware watermark embedding, simulated distortions, and mask and message recovery."
  caption: "A learned mask guides where the watermark is embedded, while decoder branches recover the mask and message after distortion."
  source: https://arxiv.org/abs/2607.05261v1
  credit: "Figure 2 from the FlowMark preprint, version 1"
venue: "arXiv preprint"
paperurl: "https://arxiv.org/abs/2607.05261"
citation: "Vishal Asnani, Shruti Agarwal, John Collomosse. (2026). FlowMark: Mask-Guided Video Watermarking. arXiv:2607.05261."
---

**Where should a watermark go in a video frame?** FlowMark learns content-adaptive embedding regions rather than relying on manually supplied or random masks. The goal is to preserve visual quality and temporal consistency while keeping provenance signals recoverable.

### How it works

- A mask predictor identifies suitable regions; a message-conditioned encoder embeds the watermark.
- Perceptual modulation and a temporal-consistency objective help limit visible distortion and flicker.
- Training progressively introduces image distortions and video codecs. Separate decoder branches recover the embedding mask and message.

### A reported result

> **50.41 dB PSNR with a 128-bit payload** in the clean, no-augmentation SA-V evaluation in Table 1. Reported bit accuracy is **1.00** in that setting.

The paper evaluates on the SA-V test set of **155 videos at 24 fps**. These clean-setting numbers should not be read as perfect recovery after every edit: Table 2 reports **0.80 bit accuracy under combined video distortions**.

### Scope

This is a **preprint**, not a peer-reviewed proceedings paper. Its results cover the datasets, codecs, and editing conditions tested; they are not a guarantee for every distribution pipeline.

### Source

[Preprint v1: Section 4.1 and Tables 1–2](https://arxiv.org/abs/2607.05261v1)
