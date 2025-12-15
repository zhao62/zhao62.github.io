---
layout: post
title: "用於故障診斷的深度殘差收縮網路"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-15
tags: [深度學習, 故障診斷]
mathjax: true
---

## 摘要 (Abstract)

本文發展出全新的深度學習方法，稱作「深度殘差收縮網路」（Deep Residual Shrinkage Networks, DRSN），藉此提升處理高雜訊震動訊號時的特徵學習能力，並達到高精度的故障診斷。研究中將軟門檻值（Soft Thresholding）導入至深度架構中，作為非線性轉換層，以排除掉不重要的特徵。此外，由於門檻值（thresholds）的一般設定相當具挑戰性，所開發的深度殘差收縮網路整合了數個專門的神經網路作為可訓練的模組，來自動決定門檻值，如此一來，便不再需要訊號處理方面的專業知識。本文所發展的方法，其有效性已透過針對各種不同類型雜訊的實驗驗證。

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="用於故障診斷的深度殘差收縮網路" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="用於故障診斷的深度殘差收縮網路" width="100%">
</p>

## 學術影響 (Academic Impact)

本文在 Google Scholar 上已獲得超過 1,400 次引用。

根據保守估計，「深度殘差收縮網路」（DRSN）已應用於超過 1,000 篇的學術文獻中。這些研究工作均直接採用本網路或對其進行改進，廣泛地被運用在下列各種領域，包含：機械工程、電力工程、電腦視覺、醫療照護（Healthcare）、語音處理、文字分析、雷達、以及遙測（Remote Sensing）。

## 參考文獻 (Reference)

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
