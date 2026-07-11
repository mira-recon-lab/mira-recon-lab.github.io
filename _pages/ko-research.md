---
layout: page
permalink: /ko/research/
title: 연구
lang: ko
alt_lang: /research/
description: 임상 및 뇌과학 응용을 위한 고속 MRI 획득과 물리 기반 딥러닝 재구성 연구.
nav: true
nav_order: 2
---

## 1. 딥러닝 기반 영상 재구성 (Deep Learning Reconstruction)

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_wave_modl.png" title="Wave-MoDL" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**MoDL**(model-based deep learning)은 적은 수의 파라미터만으로 CNN 기반 regularizer를 병렬 영상 재구성에 결합하는 기법입니다. 우리는 여기에 wave encoding을 더한 **Wave-MoDL**을 제안해, data consistency를 지키면서도 3D 영상을 크게 가속했습니다.

궁극적으로는 임상과 뇌과학 연구에 바로 활용할 수 있는, 빠르면서 정확한 물리 기반 재구성 기술을 목표로 합니다.

---

## 2. 고속 정량 MRI (Quantitative MRI)

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_qmri.png" title="Quantitative MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**qMRI**는 조직의 T1, T2, T2\*, proton density 같은 물성을 정량적으로 측정하는 기법입니다. 정성 영상으로는 놓치기 쉬운 미세한 변화를 잡아내고 질환을 조기에 발견할 수 있어 임상적 가치가 크지만, 고해상도로 찍으려면 촬영 시간이 길어진다는 한계가 있습니다.

우리는 **정확도를 유지하면서 촬영 시간을 줄이는** 방법을 연구합니다.

---

## 3. 움직임에 강인한 Diffusion MRI

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_dmri.png" title="Diffusion MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Diffusion MRI에는 빠른 **EPI**가 널리 쓰이고, **multi-shot EPI**(msEPI)는 왜곡과 blurring을 한층 더 줄일 수 있습니다. 다만 위상 방향 왜곡, shot 간 phase 변화, 움직임 artifact에 취약하다는 문제가 남습니다.

우리는 이를 해결하는 **VUDU**, **BUDA** 등 왜곡 없이 움직임에 강인한 고해상도 msEPI 기법을 개발합니다.

---

자세한 내용은 조재진 교수([jaejincho@sejong.ac.kr](mailto:jaejincho@sejong.ac.kr))에게 편하게 문의해 주세요.
