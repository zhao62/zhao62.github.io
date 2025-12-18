---
layout: post
title: "Deep Residual Shrinkage Networks til fejldiagnosticering"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Kunstig intelligens, fejldiagnosticering]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Resumé:

Denne artikel præsenterer nye deep learning-metoder, specifikt *Deep Residual Shrinkage Networks*, der har til formål at forbedre evnen til feature-læring fra stærkt støjfyldte vibrationssignaler og dermed opnå høj nøjagtighed i fejldiagnosticering. *Soft thresholding* indsættes som ikke-lineære transformationslag i de dybe arkitekturer for at eliminere uvæsentlige features. Da det generelt kan være udfordrende at fastsætte korrekte værdier for tærsklerne (thresholds), integrerer de udviklede Deep Residual Shrinkage Networks desuden en række specialiserede neurale netværk som trænbare moduler. Disse moduler bestemmer automatisk tærskelværdierne, således at ekspertviden inden for signalbehandling ikke er påkrævet. De udviklede metoders effektivitet er valideret gennem eksperimenter med forskellige typer støj.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks til fejldiagnosticering" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks til fejldiagnosticering" width="100%">
</p>

## Akademisk indflydelse

Denne artikel har modtaget over 1.400 citationer på Google Scholar.

Ifølge konservative estimater er Deep Residual Shrinkage Networks (DRSN) blevet anvendt i mere end 1.000 publikationer. Disse arbejder har enten anvendt netværket direkte eller bygget videre på det inden for en bred vifte af fagområder, herunder maskinteknik, elkraft, computer vision, sundhedsvæsen, talebehandling, tekstanalyse, radar og remote sensing.

## Referencer

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
