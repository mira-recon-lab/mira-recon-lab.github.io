---
layout: page
permalink: /research/
title: Research
lang: en
alt_lang: /ko/research/
description: Rapid MRI acquisition and physics-guided deep learning reconstruction for clinical and neuroscientific applications.
nav: true
nav_order: 2
---

## 1. Deep Learning Based Image Reconstruction

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_wave_modl.png" title="Wave-MoDL" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The recently introduced **model-based deep learning (MoDL)** technique successfully incorporates convolutional neural network (CNN)-based regularizers into physics-based parallel imaging reconstruction using a small number of network parameters. We propose **wave-encoded MoDL (Wave-MoDL)** — combining the wave-encoding strategy with unrolled network constraints for highly accelerated 3D imaging while enforcing data consistency.

Our research interest is to develop rapid MR acquisition and high-fidelity physics-guided deep-learning-based image reconstruction that may facilitate clinical and neuroscientific applications.

---

## 2. Rapid Quantitative Magnetic Resonance Imaging

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_qmri.png" title="Quantitative MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Quantitative MRI (qMRI)** techniques aim to provide quantitative estimates of tissue relaxation parameters. These methods use Bloch simulations of the acquired signals to calculate **T1, T2, T2\*, or proton density (PD) maps** in quantitative units.

In clinical settings, qMRI can help identify physiological changes undetected by qualitative imaging, provide specific information to characterize pathologies, assess treatment response and repair processes, and detect disease before morphological changes appear. However, high-resolution qMRI is often less suitable for clinical MR exams due to long acquisition times.

Our research interest is **accelerating the acquisition while preserving the accuracy of quantitative parameter maps**.

---

## 3. Motion-Robust Multi-shot Imaging for Diffusion MRI

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_dmri.png" title="Diffusion MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Echo-planar imaging (EPI)** is widely used for diffusion MRI due to its fast acquisition. **Multi-shot EPI (msEPI)** can mitigate distortion and T2/T2\*-related voxel blurring and pile-ups by increasing acceleration and reducing echo-spacing time significantly.

However, msEPI suffers from magnetic field-related image distortion in the phase-encoding direction, phase variation between multi shots, and motion-related artifacts.

Our research interest is to develop **efficient, motion-robust, distortion-free, and high-resolution msEPI acquisition methods** — including VUDU (Variable flip, blip-Up and -Down Undersampling) and BUDA (Blip-Up/Down Acquisition).

---

Please feel free to contact Dr. Jaejin Cho at [jaejincho@sejong.ac.kr](mailto:jaejincho@sejong.ac.kr) for more information.
