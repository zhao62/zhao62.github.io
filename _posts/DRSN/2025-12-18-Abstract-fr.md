---
layout: post
title: "Deep Residual Shrinkage Networks pour le diagnostic de défauts"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [intelligence artificielle, diagnostic de panne]
mathjax: true
description: "Cet article présente de nouvelles méthodes d'apprentissage profond, baptisées Deep Residual Shrinkage Networks (réseaux résiduels profonds à seuillage), visant à améliorer la capacité d'apprentissage de caractéristiques (feature learning) à partir de signaux vibratoires fortement bruités et à atteindre une grande précision dans le diagnostic de défauts."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Résumé

Cet article présente de nouvelles méthodes d'apprentissage profond, baptisées Deep Residual Shrinkage Networks (réseaux résiduels profonds à seuillage), visant à améliorer la capacité d'apprentissage de caractéristiques (feature learning) à partir de signaux vibratoires fortement bruités et à atteindre une grande précision dans le diagnostic de défauts. Le seuillage doux (soft thresholding) est inséré sous forme de couches de transformation non linéaire au sein des architectures profondes afin d'éliminer les caractéristiques non pertinentes. De plus, étant donné qu'il est généralement délicat de définir des valeurs de seuil adéquates, les Deep Residual Shrinkage Networks intègrent des réseaux de neurones spécialisés sous forme de modules apprenables (trainable modules). Ces derniers permettent de déterminer automatiquement les seuils, rendant ainsi superflue toute expertise pointue en traitement du signal. L'efficacité des méthodes proposées est validée par des expériences impliquant divers types de bruits.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks pour le diagnostic de défauts" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks pour le diagnostic de défauts" width="100%">
</p>

## Impact académique

Cet article comptabilise plus de 1 400 citations sur Google Scholar.

Selon des estimations prudentes, les Deep Residual Shrinkage Networks (DRSN) ont été utilisés dans plus de 1 000 publications. Ces travaux ont soit appliqué directement ce réseau, soit l'ont amélioré, et ce dans un large éventail de domaines incluant le génie mécanique, l'énergie électrique, la vision par ordinateur, la santé, le traitement de la parole, l'analyse textuelle, le radar et la télédétection.

## Références

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
