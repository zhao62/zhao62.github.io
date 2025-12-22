---
layout: post
title: "고장 진단을 위한 Deep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-15
tags: [딥러닝, 고장 진단]
mathjax: true
description: "본 논문은 잡음이 심한 진동 신호로부터 특징(Feature) 학습 능력을 향상시키고 높은 고장 진단 정확도를 달성하기 위해, 새로운 딥러닝 기법인 Deep Residual Shrinkage Networks를 제안한다."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## 초록 (Abstract)

본 논문은 잡음이 심한 진동 신호로부터 특징(Feature) 학습 능력을 향상시키고 높은 고장 진단 정확도를 달성하기 위해, 새로운 딥러닝 기법인 Deep Residual Shrinkage Networks를 제안한다. 중요하지 않은 특징들을 제거하기 위해 심층 아키텍처 내에 비선형 변환 레이어(Layer)로서 Soft Thresholding을 삽입하였다. 또한, 일반적으로 적절한 Threshold 값을 설정하는 것이 어렵다는 점을 고려하여, 제안된 네트워크는 별도의 특화된 신경망을 학습 가능한 모듈로 통합함으로써 Threshold를 자동으로 결정하도록 설계되었다. 이를 통해 신호 처리에 대한 전문적인 지식이 요구되지 않는다. 제안된 기법의 유효성은 다양한 유형의 잡음 환경에서의 실험을 통해 검증되었다.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="고장 진단을 위한 Deep Residual Shrinkage Networks" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="고장 진단을 위한 Deep Residual Shrinkage Networks" width="100%">
</p>

## 학술적 영향 (Academic Impact)

본 논문은 Google Scholar에서 1,400회 이상 인용되었다.

보수적인 추산에 따르면, Deep Residual Shrinkage Networks (DRSN)는 1,000편 이상의 논문에서 활용되었다. 이러한 연구들은 기계 공학, 전력, 컴퓨터 비전, 헬스케어, 음성 처리, 텍스트 분석, 레이더 및 원격 탐사(Remote Sensing) 등 광범위한 분야에 걸쳐 해당 네트워크를 직접 적용하거나 개선하였다.

## 참고 문헌 (Reference)

Minghang Zhao, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht, Deep residual shrinkage networks for fault diagnosis, IEEE Transactions on Industrial Informatics, 2020, 16(7): 4681-4690.

[https://ieeexplore.ieee.org/document/8850096](https://ieeexplore.ieee.org/document/8850096)

## BibTeX
```bibtex
@article{Zhao2020,
  author    = {Minghang Zhao and Shisheng Zhong and Xuyun Fu and Baoping Tang and Michael Pecht},
  title     = {Deep Residual Shrinkage Networks for Fault Diagnosis},
  journal   = {IEEE Transactions on Industrial Informatics},
  year      = {2020},
  volume    = {16},
  number    = {7},
  pages     = {4681-4690},
  doi       = {10.1109/TII.2019.2943898}
}
```
