---
title: "Proactive Image Manipulation Detection"
collection: publications
paper_figure:
  image: /images/papers/paper3-method.png
  width: 1400
  height: 443
  alt: "Proactive detection learns a template set, adds a selected template to an image, and recovers its signal to distinguish manipulation."
  caption: "Template protection happens before manipulation; the recovery network then looks for evidence of changes to that signal."
  source: https://openaccess.thecvf.com/content/CVPR2022/html/Asnani_Proactive_Image_Manipulation_Detection_CVPR_2022_paper.html
  credit: "Figure 2 from the CVPR 2022 paper"
authors: "Vishal Asnani, Xi Yin, Tal Hassner, Sijia Liu, Xiaoming Liu"
codeurl: "https://github.com/vishal3477/proactive_IMD"
permalink: /publication/paper3
date: 2022-05-01
venue: 'IEEE/CVF Conference on Computer Vision and Pattern Recognition'
paperurl: 'https://openaccess.thecvf.com/content/CVPR2022/html/Asnani_Proactive_Image_Manipulation_Detection_CVPR_2022_paper.html'
citation: 'Asnani, V., Yin, X., Hassner, T., Liu, S., & Liu, X. (2022). Proactive Image Manipulation Detection. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition.'
---

**Can images be prepared to make future manipulation easier to detect?** This work moves part of the forensic process before the edit: a learned template is added to an original image, giving the detector a signal to examine later.

### How it works

- Learn a set of low-magnitude, high-frequency templates with constraints on diversity and recoverability.
- Protect an image with a selected template before it reaches a manipulation model.
- Recover the signal from protected or manipulated images and use it for classification.

### A reported result

> **92.43% mean average precision across 12 unseen generative models**, versus **82.97%** for the Wang et al. baseline in Table 4.

The proactive model is trained using **STGAN** in this comparison. The number is an average of per-model average precision, not classification accuracy or a guarantee at a particular false-alarm rate.

### Scope

Protection must be applied before manipulation. This is not a passive detector for arbitrary unprotected images, and performance varies by manipulation model.

### Sources and resources

The numerical comparison is from **Section 4 and Table 4**.

[Published paper](https://openaccess.thecvf.com/content/CVPR2022/html/Asnani_Proactive_Image_Manipulation_Detection_CVPR_2022_paper.html)
[Supplementary](https://openaccess.thecvf.com/content/CVPR2022/supplemental/Asnani_Proactive_Image_Manipulation_CVPR_2022_supplemental.pdf)
[GitHub](https://github.com/vishal3477/proactive_IMD)
[Project Webpage](http://cvlab.cse.msu.edu/project-proactive.html)
