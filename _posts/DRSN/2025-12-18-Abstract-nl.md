---
layout: post
title: "Deep Residual Shrinkage Networks voor Foutdiagnose"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Kunstmatige Intelligentie, Foutdiagnose]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Samenvatting:

Dit artikel introduceert nieuwe *deep learning*-methoden, namelijk *Deep Residual Shrinkage Networks*, om het vermogen om kenmerken te leren uit zwaar verruiste trillingssignalen te verbeteren en een hoge nauwkeurigheid bij foutdiagnose te realiseren. Er is *soft thresholding* toegevoegd als niet-lineaire transformatielaag binnen de diepe architecturen om onbelangrijke kenmerken te elimineren. Aangezien het over het algemeen lastig is om de juiste waarden voor deze drempels (*thresholds*) vast te stellen, integreren de ontwikkelde *Deep Residual Shrinkage Networks* enkele gespecialiseerde neurale netwerken als trainbare modules. Hiermee worden de drempelwaarden automatisch bepaald, waardoor specialistische expertise op het gebied van signaalverwerking niet vereist is. De effectiviteit van de ontwikkelde methoden is gevalideerd door middel van experimenten met verschillende soorten ruis.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks voor Foutdiagnose" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks voor Foutdiagnose" width="100%">
</p>

## Academische Impact

Dit artikel is meer dan 1.400 keer geciteerd op Google Scholar.

Volgens conservatieve schattingen zijn *Deep Residual Shrinkage Networks* (DRSN) in meer dan 1.000 publicaties gebruikt. In deze werken is het netwerk direct toegepast of verder verbeterd binnen een breed scala aan vakgebieden, waaronder werktuigbouwkunde, energietechniek, *computer vision*, gezondheidszorg, spraakverwerking, tekstanalyse, radar en *remote sensing*.

## Referentie

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
