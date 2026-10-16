---
title: "TokenTrace: Multi-Concept Attribution through Watermarked Token Recovery"
collection: publications
paper_figure:
  image: /images/papers/tokentrace-method.png
  width: 1400
  height: 493
  alt: "TokenTrace concept encoding and query-based decoding, with frozen image and text encoders and trainable projection and attention layers."
  caption: "Concept-specific secrets condition generation, and a textual query helps recover the secret associated with a selected concept."
  source: https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_TokenTrace_Multi-Concept_Attribution_through_Watermarked_Token_Recovery_CVPR_2026_paper.html
  credit: "Figure 2 from the accepted CVPR 2026 paper"
authors: "Li Zhang, Shruti Agarwal, John Collomosse, Pengtao Xie, Vishal Asnani"
paperurl: "https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_TokenTrace_Multi-Concept_Attribution_through_Watermarked_Token_Recovery_CVPR_2026_paper.html"
permalink: /publication/tokentrace
date: 2026-06-01
venue: "IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)"
citation: "Li Zhang, Shruti Agarwal, John Collomosse, Pengtao Xie, Vishal Asnani. (2026). TokenTrace: Multi-Concept Attribution through Watermarked Token Recovery."
---

**One generated image can contain several creative influences.** TokenTrace asks how to verify each influence separately, rather than treating the entire image as one attribution target.

### How it works

- Concept secrets perturb both the relevant text-token embedding and the initial latent noise used for generation.
- At verification time, the generated image and a textual query identify the concept to retrieve.
- Frozen image and text encoders work with trainable projection and attention layers to recover a concept embedding and decode its secret.

### A reported result

> **88.62% attribution accuracy**, compared with **85.14% for CustomMark**, for the two-customized-concept setting in Table 2.

That setting combines an object and a style from a pool of **20 customized concepts**. The paper uses Stable Diffusion 1.5 and a default **16-bit secret**. Attribution accuracy measures exact secret recovery, not the fraction of individual bits recovered.

The result above refers to the base TokenTrace method. The prompt-weighted variant, **TokenTraceP**, is reported separately; its higher numbers are not substituted here.

### Scope

This is proactive attribution: secrets must be embedded through the generation pipeline. It is not a post-hoc ownership test for arbitrary images generated without those signals.

### Source

[Accepted CVPR 2026 paper: Sections 3–4 and Table 2](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_TokenTrace_Multi-Concept_Attribution_through_Watermarked_Token_Recovery_CVPR_2026_paper.html)
