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

## 1. 딥러닝 기반 영상 재구성

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_wave_modl.png" title="Wave-MoDL" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

최근 소개된 **모델 기반 딥러닝(MoDL, model-based deep learning)** 기법은 적은 수의 네트워크 파라미터만으로 합성곱 신경망(CNN) 기반 정규화(regularizer)를 물리 기반 병렬 영상 재구성에 성공적으로 결합합니다. 우리는 **파형 인코딩 MoDL(Wave-MoDL)** 을 제안하여, 파형 인코딩(wave-encoding) 전략과 언롤드(unrolled) 네트워크 제약을 결합함으로써 데이터 일관성(data consistency)을 유지하면서도 고배속 3D 영상을 획득합니다.

우리의 연구 목표는 임상 및 뇌과학 응용을 뒷받침할 수 있는 **고속 MR 획득**과 **높은 충실도의 물리 기반 딥러닝 영상 재구성** 기술을 개발하는 것입니다.

---

## 2. 고속 정량 자기공명영상 (Quantitative MRI)

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_qmri.png" title="Quantitative MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**정량 MRI(qMRI)** 기법은 조직의 이완(relaxation) 파라미터를 정량적으로 추정하는 것을 목표로 합니다. 이 방법들은 획득한 신호에 대한 블로흐(Bloch) 시뮬레이션을 이용해 **T1, T2, T2\*, 양성자 밀도(PD) 지도**를 정량적 단위로 계산합니다.

임상 환경에서 qMRI는 정성적 영상으로는 놓칠 수 있는 생리학적 변화를 식별하고, 병변 특성화를 위한 구체적 정보를 제공하며, 치료 반응과 회복 과정을 평가하고, 형태학적 변화가 나타나기 전에 질환을 조기에 발견하는 데 도움을 줄 수 있습니다. 그러나 고해상도 qMRI는 획득 시간이 길어 임상 MR 검사에 적용하기 어려운 경우가 많습니다.

우리의 연구 목표는 **정량 파라미터 지도의 정확도를 유지하면서 획득 속도를 가속화**하는 것입니다.

---

## 3. 확산 MRI를 위한 움직임에 강인한 다중 샷 영상

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/research_dmri.png" title="Diffusion MRI" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**에코 평면 영상(EPI, echo-planar imaging)** 은 빠른 획득 속도 덕분에 확산 MRI에 널리 사용됩니다. **다중 샷 EPI(msEPI)** 는 가속률을 높이고 에코 간격(echo-spacing) 시간을 크게 줄여 왜곡과 T2/T2\* 관련 복셀 흐림 및 신호 뭉침(pile-up)을 완화할 수 있습니다.

그러나 msEPI는 위상 인코딩 방향의 자기장 관련 영상 왜곡, 다중 샷 간의 위상 변화, 움직임에 의한 아티팩트에 취약합니다.

우리의 연구 목표는 **효율적이면서 움직임에 강인하고 왜곡이 없는 고해상도 msEPI 획득 기법**을 개발하는 것으로, VUDU(Variable flip, blip-Up and -Down Undersampling)와 BUDA(Blip-Up/Down Acquisition)가 여기에 포함됩니다.

---

자세한 내용은 조재진 교수([jaejincho@sejong.ac.kr](mailto:jaejincho@sejong.ac.kr))에게 편하게 문의해 주세요.
