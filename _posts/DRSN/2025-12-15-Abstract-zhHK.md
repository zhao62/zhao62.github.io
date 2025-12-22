---
layout: post
title: "用於故障診斷的深度殘差收縮網絡"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-15
tags: [深度學習, 故障診斷]
mathjax: true
description: "本文開發了一種新的深度學習方法，即「深度殘差收縮網絡」(Deep Residual Shrinkage Networks, DRSN)，旨在提升從高噪音震動訊號 (vibration signals) 中學習特徵的能力，並實現高準確度的故障診斷。"
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## 摘要 (Abstract)

本文開發了一種新的深度學習方法，即「深度殘差收縮網絡」(Deep Residual Shrinkage Networks, DRSN)，旨在提升從高噪音震動訊號 (vibration signals) 中學習特徵的能力，並實現高準確度的故障診斷。我們將軟閾值化 (Soft thresholding) 作為非線性變換層嵌入到深度架構中，以剔除不重要的特徵。此外，鑑於設定合適的閾值通常具有挑戰性，所開發的 DRSN 整合了一些專門的神經網絡作為可訓練模組 (trainable modules) 來自動確定閾值，因此使用者無需具備訊號處理的專業知識。透過針對各類噪音的實驗，我們驗證了該方法的成效。

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="用於故障診斷的深度殘差收縮網絡" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="用於故障診斷的深度殘差收縮網絡" width="100%">
</p>

## 學術影響 (Academic Impact)

本文在 Google Scholar 上已錄得超過 1,400 次引用。

據保守估計，深度殘差收縮網絡 (DRSN) 已被應用於超過 1,000 篇文獻中。這些研究涵蓋機械工程、電力、電腦視覺 (Computer Vision)、醫療保健、語音處理、文本分析、雷達及遙感等廣泛領域，當中包括直接應用或對該網絡進行改良。

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
