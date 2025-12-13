---
layout: post
title: "基于深度残差收缩网络的故障诊断"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-13
tags: [深度学习, 故障诊断]
mathjax: true
---

## 摘要：

本文提出了一种新的深度学习方法——深度残差收缩网络（Deep Residual Shrinkage Networks, DRSN），旨在提升在强噪声振动信号条件下的特征学习能力，实现较高的故障诊断准确率。该方法在深层网络结构中引入软阈值函数作为非线性变换层，用于抑制和消除不重要的特征。由于阈值参数通常难以合理设定，所提出的深度残差收缩网络将若干专用神经网络作为可训练模块进行集成，以实现阈值的自适应确定，从而无需依赖信号处理方面的专业经验。通过在多种噪声类型条件下开展实验，验证了所提出方法的有效性。

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="基于深度残差收缩网络的故障诊断" width="100%">
</p>

## 影响力情况

该论文的谷歌学术引用量已经超过1400次。

根据不完全统计，深度残差收缩网络已经被超过1000篇文献直接应用或改进后应用于机械、电力、视觉、医疗、语音、文本、雷达、遥感等众多领域。

## 参考文献

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
