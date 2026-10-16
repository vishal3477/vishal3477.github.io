---
title: "ProMark: Proactive Diffusion Watermarking for Causal Attribution"
collection: publications
paper_figure:
  image: /images/papers/paper6-method.png
  width: 1400
  height: 572
  alt: "ProMark watermarks training images with concept-specific secrets, trains a diffusion model, and recovers secrets from its outputs."
  caption: "Concept identifiers are introduced into training data and recovered from generated content for attribution."
  source: https://openaccess.thecvf.com/content/CVPR2024/html/Asnani_ProMark_Proactive_Diffusion_Watermarking_for_Causal_Attribution_CVPR_2024_paper.html
  credit: "Figure 2 from the accepted CVPR 2024 paper"
authors: "Vishal Asnani, John Collomosse, Tu Bui, Xiaoming Liu, Shruti Agarwal"
paperurl: "https://openaccess.thecvf.com/content/CVPR2024/html/Asnani_ProMark_Proactive_Diffusion_Watermarking_for_Causal_Attribution_CVPR_2024_paper.html"
permalink: /publication/paper6
date: 2024-06-01
venue: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition'
citation: 'Asnani, V., Collomosse, J., Bui, T., Liu, X., Agarwal, S. (2024). ProMark: Proactive Diffusion Watermarking for Causal Attribution. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition.'
---

**Visual resemblance alone does not establish which training concepts influenced a generated image.** ProMark introduces concept-specific watermark signals during training and retrieves those signals from generated content.

### How it works

- Encode source concepts, such as content categories or artistic media, as bit secrets.
- Watermark the corresponding training images and train the diffusion model to retain those signals.
- Decode generated images to attribute one or more concepts rather than relying only on nearest-image similarity.

### A reported result

> **84.66% combined media-and-content attribution accuracy** on **BAM**, using two watermarks per image at **30% watermark strength**, Table 3.

That is joint attribution of both concepts, not bit accuracy. Table 3 reports **46.23%** for the AbC-CLIP comparison. ProMark's 16-bit identifier space supports **2^16 (65,536)** distinct watermarks; capacity is not a promise of perfect recovery at that scale.

### Scope

The approach assumes access to the training or fine-tuning process and watermarked source data. Stronger watermarks can improve recovery while introducing visible artifacts, so attribution and image quality must be assessed together.

### Sources and resources

See **Sections 4.2-4.3, Table 3, and Figure 5**.

[Published paper](https://openaccess.thecvf.com/content/CVPR2024/html/Asnani_ProMark_Proactive_Diffusion_Watermarking_for_Causal_Attribution_CVPR_2024_paper.html)
[Supplementary](https://openaccess.thecvf.com/content/CVPR2024/supplemental/Asnani_ProMark_Proactive_Diffusion_CVPR_2024_supplemental.pdf)
