---
title: "PiVoT: Proactive Video Templates for Enhancing Video Task Performance"
collection: publications
paper_figure:
  image: /images/papers/pivot-method.png
  width: 1400
  height: 591
  alt: "PiVoT generates spatiotemporal templates with a 3D U-Net and adapts a frozen video backbone using LoRA."
  caption: "Video templates and low-rank adapters are learned together for action recognition and spatiotemporal action detection."
  source: https://openaccess.thecvf.com/content/CVPR2026W/CV4Smalls/html/Asnani_PiVoT_Proactive_Video_Templates_for_Enhancing_Video_Task_Performance_CVPRW_2026_paper.html
  credit: "Figure 2 from the accepted CVPR 2026 Workshops paper"
authors: "Vishal Asnani, Shruti Agarwal, Xiaoming Liu"
paperurl: "https://openaccess.thecvf.com/content/CVPR2026W/CV4Smalls/html/Asnani_PiVoT_Proactive_Video_Templates_for_Enhancing_Video_Task_Performance_CVPRW_2026_paper.html"
permalink: /publication/pivot
date: 2026-06-01
venue: "IEEE/CVF Conference on Computer Vision and Pattern Recognition Workshops (CVPR Workshops)"
citation: "Vishal Asnani, Shruti Agarwal, Xiaoming Liu. (2026). PiVoT: Proactive Video Templates for Enhancing Video Task Performance."
---

**Can a learned change to video frames make motion easier for a model to understand?** PiVoT extends proactive templates to video, pairing temporal input adaptation with parameter-efficient model adaptation.

### How it works

- A 3D U-Net creates frame-specific templates that capture temporal information.
- The templates alter the video frames supplied to the downstream model.
- The pretrained backbone stays frozen while the template generator and **rank-4 LoRA adapters** are trained.

Experiments cover action recognition on Kinetics-400 and Something-Something-v2, and spatiotemporal action detection on AVA2.1.

### A reported result

> **27.12% mAP with PiVoT versus 24.11% for the reproduced SlowFast baseline** on **AVA2.1**, Table 3.

This is action-detection mAP, not recognition Top-1 accuracy. The comparison uses the paper's reproduced baseline rather than substituting the original reported score.

### Scope

PiVoT adds template-generation and adapter computation. Its templates are not constrained to be imperceptible, so performance improvement should not be read as a claim of visually unchanged input video.

### Source

[Accepted workshop paper: Sections 3-4 and Table 3](https://openaccess.thecvf.com/content/CVPR2026W/CV4Smalls/html/Asnani_PiVoT_Proactive_Video_Templates_for_Enhancing_Video_Task_Performance_CVPRW_2026_paper.html)
