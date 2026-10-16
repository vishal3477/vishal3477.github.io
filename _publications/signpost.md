---
title: "Signpost Watermarking: Joint Optimization for Visual Watermark Coexistence"
collection: publications
authors: "Shruti Agarwal, Vishal Asnani, John Collomosse"
permalink: /publication/signpost
date: 2026-10-01
status: accepted
paper_figure:
  image: /images/papers/signpost-method.png
  width: 1150
  height: 414
  alt: "A signpost encoder and decoder train with frozen secondary watermarking systems to optimize coexistence."
  caption: "Training explicitly exposes the signpost to other watermark systems instead of relying on accidental compatibility."
  source: https://arxiv.org/abs/2608.10091v1
  credit: "Figure 1 from the public manuscript, version 1"
venue: "ECCV 2026 LifegenIP Workshop"
paperurl: "https://arxiv.org/abs/2608.10091"
paper_label: "Public manuscript"
citation: "Shruti Agarwal, Vishal Asnani, John Collomosse. (2026). Signpost Watermarking: Joint Optimization for Visual Watermark Coexistence. Accepted to the ECCV 2026 LifegenIP Workshop."
---

**How can one watermark help discover another without disrupting it?** Signpost watermarking investigates a lightweight routing signal that indicates which independently deployed provenance watermark should be decoded.

### How it works

- A U-Net encoder adds a residual carrying a **32-bit secret**; a ResNet-50 decoder recovers it.
- Frozen secondary watermark systems are applied during training.
- Decoder-aware objectives optimize coexistence in both image and video settings, rather than assuming independently trained signals will not interfere.

### A reported result

> **0.988 bit accuracy for TrustMark-P when the signpost is added on top**, in the **clean image-coexistence setting**, Table 2.

The table reports a **0.008 decrease** relative to TrustMark-P alone. This measures recovery of the first watermark, not the signpost's own accuracy, and does not describe performance after every distortion.

### Scope and source version

Coexistence remains pairing- and order-dependent. The manuscript includes cases with greater interference, so this is not universal interoperability.

**Accepted to the ECCV 2026 LifegenIP Workshop.** The figure and results use the **August 2026 public manuscript, version 1**; an official workshop proceedings link has not yet been verified.

[Public manuscript: Section 3 and Table 2](https://arxiv.org/abs/2608.10091v1)
