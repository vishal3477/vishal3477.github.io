---
title: "NRGMark: Localized Watermarking for Energy Transparency in Images"
collection: publications
paper_figure:
  image: /images/papers/nrgmark-method.png
  width: 1400
  height: 620
  alt: "NRGMark embeds separate secrets into image subregions, composites them, localizes marked regions after distortion, and decodes each secret."
  caption: "Region localization allows different visual elements in one design to carry independent provenance identifiers."
  source: https://openaccess.thecvf.com/content/WACV2026/html/Agarwal_NRGMark_Localized_Watermarking_for_Energy_Transparency_in_Images_WACV_2026_paper.html
  credit: "Figure 2 from the accepted WACV 2026 paper"
authors: "Shruti Agarwal, Élie Michel, Vishal Asnani, Tania Mathern, John Collomosse"
paperurl: "https://openaccess.thecvf.com/content/WACV2026/html/Agarwal_NRGMark_Localized_Watermarking_for_Energy_Transparency_in_Images_WACV_2026_paper.html"
permalink: /publication/nrgmark
date: 2026-03-01
venue: "IEEE/CVF Winter Conference on Applications of Computer Vision (WACV)"
citation: "Shruti Agarwal, Elie Michel, Vishal Asnani, Tania Mathern, John Collomosse. (2026). NRGMark: Localized Watermarking for Energy Transparency in Images."
---

**A composite design can contain several images with different origins and energy footprints.** NRGMark gives individual visual elements independent identifiers rather than assigning one provenance payload to the whole design.

### How it works

- Watermark selected image regions with separate bit secrets.
- Train a localizer to find those regions after compositing and image transformations.
- Decode the localized regions and use their identifiers to look up provenance and environmental-impact records through a C2PA extension.

The framework is tested with five watermark encoder-decoder systems, as well as design-layout and print-scan examples.

### A reported result

> **0.94 localization IoU** for NRGMark with **TrustMark-P on noisy MIRFlickR images**, compared with **0.95 without noise**, Table 1.

IoU measures agreement between predicted and target regions. It is distinct from message bit accuracy, which the paper examines separately in Figure 5.

### Scope

NRGMark links pixels to an external record; it does **not estimate energy consumption from an image** or independently validate every value in that record. Recovery depends on the watermark, region size, and distortions.

[Paper and proceedings record](https://openaccess.thecvf.com/content/WACV2026/html/Agarwal_NRGMark_Localized_Watermarking_for_Energy_Transparency_in_Images_WACV_2026_paper.html)

The result above is from **Table 1**.
