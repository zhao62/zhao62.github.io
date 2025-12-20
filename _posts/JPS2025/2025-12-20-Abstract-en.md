---
layout: post
title: "Deep transfer learning enabled online state-of-health estimation of lithium-ion batteries under small samples across different cathode materials, ambient temperature and charge-discharge protocols"
date: 2025-12-20
tags: ["SOH Estimation", "Lithium-ion Batteries", "Deep Transfer Learning", "Battery Degradation", "Cross-domain Generalization"]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong>Xiaopeng Li, <a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Junfu Li, Zhiquan Cui, Song Fu, Zhiqi Yan</strong>
</p>

## Abstract

State-of-health (SOH) estimation of lithium-ion batteries is crucial for ensuring their efficient and safe operation. However, the accurate SOH estimation under low temperatures and high discharge rates is still a challenging problem especially when facing insufficient early-stage data. To tackle this problem, this paper proposes a self-attention-based deep transfer learning (SDTL) approach that can be flexibly updated in response to diverse cathode materials and varied operation conditions. First, an efficient self-attention-based feature learning model is constructed to capture diverse degradation patterns of batteries under different operating conditions. Second, deep transfer learning techniques are employed to achieve adaptable SOH estimation using previously learned degradation knowledge and the limited data of a new battery. To comprehensively validate the proposed approach, full life cycle tests on nickel cobalt manganese (NCM) batteries under 1C/2C conditions are conducted to supplement the nickel cobalt aluminum (NCA) public battery datasets. All the prepared battery datasets cover different cathode materials, charge-discharge rates, and ambient temperatures. Afterwards, eighteen health indicators are extracted and selected with Pearson correlation coefficient (PCC) to comprehensively characterize the statistical, electrochemical, and dynamic properties of batteries. Through comparisons with classical models that are directly trained using state-of-the-art deep learning algorithms and other widely used deep transfer learning methods, the proposed SOH estimation approach has shown wide generalizability as well as a positive accuracy improvement.

<p align="center">
  <img src="/assets/img/JPS2025/JPS2025.png" alt="Deep transfer learning enabled online state-of-health estimation of lithium-ion batteries" width="100%">
</p>

## Reference

X. Li, M. Zhao, S. Zhong, et al. Deep transfer learning enabled online state-of-health estimation of lithium-ion batteries under small samples across different cathode materials, ambient temperature and charge-discharge protocols [J]. Journal of Power Sources, 2025, 650: 237503.

[Article Page](https://www.sciencedirect.com/science/article/pii/S0378775325013394)

## BibTeX
```bibtex
@article{Li2025Deep,
  author = {Li, Xiaopeng and Zhao, Minghang and Zhong, Shisheng and Li, Junfu and Cui, Zhiquan and Fu, Song and Yan, Zhiqi},
  title = {Deep transfer learning enabled online state-of-health estimation of lithium-ion batteries under small samples across different cathode materials, ambient temperature and charge-discharge protocols},
  journal = {Journal of Power Sources},
  volume = {650},
  pages = {237503},
  year = {2025},
  issn = {0378-7753},
  doi = {10.1016/j.jpowsour.2025.237503},
  url = {https://doi.org/10.1016/j.jpowsour.2025.237503}
}
```
