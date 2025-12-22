---
layout: post
title: "Deep Residual Shrinkage Networks för feldiagnostik"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Artificiell intelligens, feldiagnostik]
mathjax: true
description: "I denna artikel utvecklas nya metoder inom djupinlärning, närmare bestämt Deep Residual Shrinkage Networks, för att förbättra förmågan till särdragsinlärning (feature learning) från vibrationssignaler med hög brusnivå och därmed uppnå hög precision vid feldiagnostik."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Sammanfattning:

I denna artikel utvecklas nya metoder inom djupinlärning, närmare bestämt Deep Residual Shrinkage Networks, för att förbättra förmågan till särdragsinlärning (feature learning) från vibrationssignaler med hög brusnivå och därmed uppnå hög precision vid feldiagnostik. Mjuk tröskling (soft thresholding) infogas som icke-linjära transformationslager i de djupa arkitekturerna för att eliminera oviktiga särdrag. Eftersom det generellt sett är utmanande att fastställa lämpliga tröskelvärden, integrerar de utvecklade nätverken dessutom ett fåtal specialiserade neurala nätverk som träningsbara moduler. Dessa fastställer tröskelvärdena automatiskt, vilket gör att expertkunskaper inom signalbehandling inte krävs. Effektiviteten hos de utvecklade metoderna valideras genom experiment med olika typer av brus.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## Akademiskt genomslag

Denna artikel har fått över 1 400 citeringar på Google Scholar.

Enligt konservativa uppskattningar har Deep Residual Shrinkage Networks (DRSN) använts i mer än 1 000 publikationer. Dessa arbeten har antingen tillämpat nätverket direkt eller vidareutvecklat det inom ett brett spektrum av områden, inklusive maskinteknik, elkraft, datorseende (computer vision), hälso- och sjukvård, talbehandling, textanalys, radar och fjärranalys (remote sensing).

## Referens

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
