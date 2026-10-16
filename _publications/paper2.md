---
title: "Reverse Engineering of Generative Models: Inferring Model Hyperparameters from Generated Images"
collection: publications
paper_figure:
  image: /images/papers/reverse-engineering-method.png
  width: 840
  height: 753
  alt: "Model parsing goes beyond real-or-fake detection and source attribution to infer model hyperparameters using fingerprint estimation and parsing networks."
  caption: "Model parsing estimates properties of an unseen generator from its output, rather than only classifying an image as real or fake."
  source: https://arxiv.org/abs/2106.07873v3
  credit: "Figure 1 from the authors' July 2023 manuscript accompanying the TPAMI article"
authors: "Vishal Asnani, Xi Yin, Tal Hassner, Xiaoming Liu"
codeurl: "https://github.com/vishal3477/Reverse_Engineering_GMs"
permalink: /publication/paper2
date: 2023-12-01
venue: 'IEEE Transactions on Pattern Analysis and Machine Intelligence'
paperurl: 'https://doi.org/10.1109/TPAMI.2023.3301451'
citation: 'Asnani, V., Yin, X., Hassner, T., & Liu, X. (2023). Reverse engineering of generative models: Inferring model hyperparameters from generated images. Transactions on Pattern Analysis and Machine Intelligence, vol. 45, no. 12, pp. 15477-15493.'
---

**What can a generated image reveal about the model behind it?** This work defines model parsing: estimating generator architecture and training-loss attributes from generated images, including images from models unseen during training.

### How it works

- A Fingerprint Estimation Network learns traces associated with the image's generator.
- A Parsing Network uses those fingerprints to predict architecture and loss-function attributes.
- Evaluation holds out entire generative models, rather than only holding out images from models already used in training.

### A reported result

> **0.813 ± 0.019 F1** for loss-function prediction in Table 5 of the authors' July 2023 manuscript, versus **0.751 ± 0.027** for the mean/mode baseline.

The result is averaged over **four model-held-out splits**, each training on 104 models and testing on 12. Section 4.1 describes a benchmark of **116,000 images from 116 generative models**.

### Scope and source version

Model parsing estimates selected attributes; it does **not reconstruct a generator's exact weights or complete source code**. The figure and quantitative details here come from the [authors' July 2023 manuscript, version 3](https://arxiv.org/abs/2106.07873v3). The primary reading link remains the official TPAMI record.

### Sources and resources

[Published paper](https://doi.org/10.1109/TPAMI.2023.3301451)
[Supplementary](https://ieeexplore.ieee.org/ielx7/34/10308548/10202583/supp1-3301451.pdf?arnumber=10202583)
[GitHub](https://github.com/vishal3477/Reverse_Engineering_GMs)
[Dataset](https://drive.google.com/drive/folders/1ZKQ3t7_Hip9DO6uwljZL4rYAn5viSRhu)
