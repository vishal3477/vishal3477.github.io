---
title: "MaLP: Manipulation Localization Using a Proactive Scheme"
collection: publications
paper_figure:
  image: /images/papers/malp-method.png
  width: 1400
  height: 558
  alt: "MaLP encryption, detection, and localization modules, combining a learned template with CNN and transformer branches."
  caption: "The template-protected image supports both manipulation detection and a pixel-level fakeness map."
  source: https://openaccess.thecvf.com/content/CVPR2023/html/Asnani_MaLP_Manipulation_Localization_Using_a_Proactive_Scheme_CVPR_2023_paper.html
  credit: "Figure 2 from the accepted CVPR 2023 paper"
authors: "Vishal Asnani, Xi Yin, Tal Hassner, Xiaoming Liu"
codeurl: "https://github.com/vishal3477/pro_loc"
permalink: /publication/paper4
date: 2023-06-01
venue: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition'
paperurl: 'https://openaccess.thecvf.com/content/CVPR2023/html/Asnani_MaLP_Manipulation_Localization_Using_a_Proactive_Scheme_CVPR_2023_paper.html'
citation: 'Asnani, V., Yin, X., Hassner, T., & Liu, X. (2023). MaLP: Manipulation Localization Using a Proactive Scheme. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition.'
---

**Knowing an image is fake does not tell us where it changed.** MaLP adds a learned template before manipulation and uses that signal to estimate a pixel-level fakeness map.

### How it works

- An encryption module adds a template to the original image.
- CNN and transformer branches learn local and global features during training.
- At inference, the shallow CNN branch provides localization without running the transformer. A detection module also supports real-versus-fake classification.

### A reported result

> **0.9394 cosine similarity** for localization in the paper's CelebA/STGAN comparison in Table 2, versus **0.8831** for the stronger comparison method in that table.

This is a localization metric, **not detection accuracy**. The same comparison reports an SSIM trade-off: **0.7312 for MaLP versus 0.7876** for that baseline. Generalization is examined separately across **22 unseen generative models**.

### Scope

The approach requires template protection before manipulation. It does not assume that arbitrary, previously unprotected images already contain the required signal.

### Sources and resources

[Published paper](https://openaccess.thecvf.com/content/CVPR2023/html/Asnani_MaLP_Manipulation_Localization_Using_a_Proactive_Scheme_CVPR_2023_paper.html)
[Supplementary](https://openaccess.thecvf.com/content/CVPR2023/supplemental/Asnani_MaLP_Manipulation_Localization_CVPR_2023_supplemental.pdf)
[GitHub](https://github.com/vishal3477/pro_loc)
