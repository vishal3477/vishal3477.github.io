---
title: "Your Text Encoder Can Be An Object-Level Watermarking Controller"
collection: publications
paper_figure:
  image: /images/papers/object-level-watermarking-method.png
  width: 1400
  height: 488
  alt: "A learned watermark token conditions image generation; latent-space and attention controls steer watermark placement onto selected objects."
  caption: "A small text-embedding update controls watermark generation, with attention-based control for selected objects."
  source: https://openaccess.thecvf.com/content/ICCV2025/html/Devulapally_Your_Text_Encoder_Can_Be_An_Object-Level_Watermarking_Controller_ICCV_2025_paper.html
  credit: "Figure 2 from the accepted ICCV 2025 paper"
authors: "Naresh Kumar Devulapally, Mingzhen Huang, Vishal Asnani, Shruti Agarwal, Siwei Lyu, Vishnu Suresh Lokhande"
paperurl: "https://openaccess.thecvf.com/content/ICCV2025/html/Devulapally_Your_Text_Encoder_Can_Be_An_Object-Level_Watermarking_Controller_ICCV_2025_paper.html"
permalink: /publication/object-level-watermarking
date: 2025-10-01
venue: "IEEE/CVF International Conference on Computer Vision (ICCV)"
citation: "Naresh Kumar Devulapally, Mingzhen Huang, Vishal Asnani, Shruti Agarwal, Siwei Lyu, Vishnu Suresh Lokhande. (2025). Your Text Encoder Can Be An Object-Level Watermarking Controller."
---

**Watermarking need not apply uniformly to a whole generated image.** This work learns a text token that can control a watermark globally or steer it toward selected objects.

### How it works

- Learn a **768-dimensional watermark-token embedding** while keeping the pretrained generation components fixed.
- Train the token through an image-to-image generation objective and a pretrained watermark decoder.
- Use cross-attention maps and latent controls to target prompt-selected objects during generation.

The paper also examines compatibility with personalized models and textual-inversion concepts.

### A reported result

> **0.99 bit accuracy with a 48-bit payload** for the **MS-COCO, full-image Stable Diffusion setting without attacks**, Table 1.

That is per-bit recovery, not the probability that every message is recovered exactly. Object-level experiments and robustness after image transformations are evaluated separately.

### Scope

The clean full-image result does not imply identical recovery for every isolated or cropped object. Watermark placement and recovery depend on attention localization, selected regions, and subsequent transformations.

### Source

[Accepted paper: Sections 4-5 and Table 1](https://openaccess.thecvf.com/content/ICCV2025/html/Devulapally_Your_Text_Encoder_Can_Be_An_Object-Level_Watermarking_Controller_ICCV_2025_paper.html)
