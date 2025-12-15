---
layout: post
title: "故障診断に向けたDeep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-15
tags: [ディープラーニング (Deep Learning), 故障診断]
mathjax: true
---

## 概要 (Abstract)：

本論文では、高ノイズの振動信号からの特徴学習能力を向上させ、高い故障診断精度を実現するために、新たなディープラーニング手法である「Deep Residual Shrinkage Networks (DRSN)」を提案する。本手法では、深層アーキテクチャ内に非線形変換層としてソフト閾値処理 (Soft Thresholding) を組み込むことで、重要でない特徴を除去する仕組みとなっている。さらに、閾値の適切な値を設定することが一般に困難であることを考慮し、提案するネットワークには、閾値を自動決定するための学習可能なモジュールとして専用のニューラルネットワークが統合されている。これにより、信号処理に関する高度な専門知識が不要となる。提案手法の有効性は、様々な種類のノイズを用いた実験により検証されている。

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="故障診断に向けたDeep Residual Shrinkage Networks" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Network" width="100%">
</p>

## 学術的インパクト (Academic Impact)

本論文は、Google Scholarにおいて1,400件以上の被引用数を記録している。

保守的な見積もりによれば、Deep Residual Shrinkage Networks (DRSN) は既に1,000以上の文献で活用されている。これらの研究は、機械工学、電力、コンピュータビジョン、ヘルスケア、音声処理、テキスト分析、レーダー、リモートセンシングといった多岐にわたる分野において、本ネットワークを直接適用、あるいは改良を加えたものである。

## 参考文献 (Reference)

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
