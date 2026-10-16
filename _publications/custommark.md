---
title: "CustomMark: Customization of Diffusion Models for Proactive Attribution"
collection: publications
paper_figure:
  image: /images/papers/custommark-method.png
  width: 1400
  height: 591
  alt: "CustomMark encodes concept secrets into token embeddings and noise, customizes diffusion attention, and decodes watermarked outputs."
  caption: "Concept and noise perturbations work with customized attention weights to produce attributable images."
  source: https://openaccess.thecvf.com/content/ICCV2025W/APAI/html/Asnani_CustomMark_Customization_of_Diffusion_Models_for_Proactive_Attribution_ICCVW_2025_paper.html
  credit: "Figure 2 from the accepted ICCV 2025 APAI Workshop paper"
authors: "Vishal Asnani, John Collomosse, Xiaoming Liu, Shruti Agarwal"
paperurl: "https://openaccess.thecvf.com/content/ICCV2025W/APAI/html/Asnani_CustomMark_Customization_of_Diffusion_Models_for_Proactive_Attribution_ICCVW_2025_paper.html"
permalink: /publication/custommark
date: 2025-10-01
venue: "IEEE/CVF International Conference on Computer Vision, APAI Workshop (ICCV Workshop)"
citation: "Vishal Asnani, John Collomosse, Xiaoming Liu, Shruti Agarwal. (2025). CustomMark: Customization of Diffusion Models for Proactive Attribution."
---

**Can attribution be added to a pretrained generator without retraining the full model?** CustomMark selectively customizes concepts so that generated images carry identifiers for relevant objects, styles, or other concepts.

### How it works

- A concept encoder and secret mapper perturb a concept's token embedding and the input noise using its bit secret.
- Training **fine-tunes the diffusion model's attention weights**; the model is not entirely fixed.
- Style-preservation and decoding objectives balance recognizable concepts with recoverable attribution.

New concepts can be introduced sequentially. Textual inversion extends the approach to concepts not already represented by suitable tokens.

### A reported result

> **89.25% attribution accuracy on WikiArt**, versus **87.19% for ProMark**, in the conditional-generation comparison in Table 1.

This is concept-attribution accuracy, not per-bit recovery. The same table gives broadly comparable ImageNet results, so the WikiArt comparison should not be generalized into a universal advantage.

### Scope

CustomMark requires a customized generation pipeline and concept-specific signals. It does not retroactively prove the training-data membership of an arbitrary unwatermarked image.

### Source

[Accepted workshop paper: Section 3.2 and Table 1](https://openaccess.thecvf.com/content/ICCV2025W/APAI/html/Asnani_CustomMark_Customization_of_Diffusion_Models_for_Proactive_Attribution_ICCVW_2025_paper.html)
