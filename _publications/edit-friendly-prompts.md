---
title: "Interpretable Prompts made Edit-Friendly: Token-to-Token Similarity Reduction in dLLMs for Edit-Friendly Hard Prompt Inversion"
collection: publications
paper_figure:
  image: /images/papers/edit-friendly-prompts-results.png
  width: 1400
  height: 961
  alt: "Reference images, reconstructed images, and the discrete prompts produced by captioning, BLIP-2, CLIP Interrogator, PEZ, VGD, and the proposed method."
  caption: "The paper compares reconstruction quality and interpretable prompts; downstream editability is evaluated separately."
  source: https://openaccess.thecvf.com/content/CVPR2026/html/Devulapally_Interpretable_Prompts_made_Edit-Friendly_Token-to-Token_Similarity_Reduction_in_dLLMs_for_CVPR_2026_paper.html
  credit: "Figure 2 from the accepted CVPR 2026 paper"
authors: "Naresh Kumar Devulapally, Shruti Agarwal, Vishal Asnani, Vishnu Suresh Lokhande"
paperurl: "https://openaccess.thecvf.com/content/CVPR2026/html/Devulapally_Interpretable_Prompts_made_Edit-Friendly_Token-to-Token_Similarity_Reduction_in_dLLMs_for_CVPR_2026_paper.html"
permalink: /publication/edit-friendly-prompts
date: 2026-06-01
venue: "IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)"
citation: "Naresh Kumar Devulapally, Shruti Agarwal, Vishal Asnani, Vishnu Suresh Lokhande. (2026). Interpretable Prompts made Edit-Friendly: Token-to-Token Similarity Reduction in dLLMs for Edit-Friendly Hard Prompt Inversion."
---

**An image-reconstruction prompt is more useful if a person can understand and edit it.** This work inverts reference images into discrete prompts designed for later word substitutions and additions.

### How it works

- A discrete diffusion language model refines prompt tokens in parallel.
- Image alignment guides the prompt toward the reference image.
- Token-similarity steering reduces coupling between token positions, aiming to make localized concept edits more reliable.

Neither the text-to-image model nor the language model requires fine-tuning.

### A reported result

> **10.50 seconds versus 104.20 seconds for VGD** at a **77-token budget on one A6000 GPU**, Table 2.

In that comparison, CLIP-image similarity is **0.74 versus 0.68**. These are inversion timings, not the total time for an arbitrary editing workflow. Faster captioning methods are also reported but have different reconstruction scores.

### Scope

Reconstruction similarity, readable text, and editability are different objectives. The paper evaluates token swaps and appends separately with semantic metrics and user studies; an editable prompt is not a pixel-exact inverse of an image.

### Source

[Accepted paper: Section 6, Table 2, and Figures 3-5](https://openaccess.thecvf.com/content/CVPR2026/html/Devulapally_Interpretable_Prompts_made_Edit-Friendly_Token-to-Token_Similarity_Reduction_in_dLLMs_for_CVPR_2026_paper.html)
