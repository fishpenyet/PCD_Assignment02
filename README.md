# PCD Assignment 02 — Image Enhancement

This repository contains Digital Image Processing Assignment 02, focused on **image enhancement** techniques for degraded images. The methods implemented are listed below.

## Methods Used

### Enhancement Techniques
- **Dark Image Enhancement** — CLAHE on the LAB L-channel + gamma correction + saturation boost
- **Low-Contrast Enhancement** — Percentile contrast stretch + CLAHE (two-stage pipeline)
- **Blurred Image Enhancement** — Unsharp masking with Gaussian blur
- **Contrast Stretching** — Per-channel percentile-based linear stretch

## Files
- `PCD_Assignment02.ipynb` — implementation and experiments
- `PCD_Assignment02_ReportAnalysis.pdf` — analysis report
- `images/input/` — input images
- `images/output/` — enhanced output images

## Notes
The experiments use a single portrait image as the reference. Three degraded versions — **dark**, **blurred**, and **low-contrast** — are synthesized from it, and each is processed by a dedicated enhancement function. Results are compared side by side against both the degraded input and the original clean image. Parameters such as CLAHE `clip_limit`, `tile_grid`, `gamma`, and sharpening `amount` were tuned empirically to balance brightness recovery against noise and colour distortion.
