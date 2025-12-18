---
layout: post
title: "Deep Residual Shrinkage Networks w diagnostyce uszkodzeń"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Sztuczna inteligencja, Diagnostyka uszkodzeń]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Abstrakt

W niniejszym artykule opracowano nowe metody uczenia głębokiego (ang. *deep learning*), a mianowicie sieci typu **Deep Residual Shrinkage Networks** (DRSN), mające na celu poprawę zdolności uczenia się cech z silnie zaszumionych sygnałów drganiowych oraz osiągnięcie wysokiej dokładności w diagnostyce uszkodzeń. W architektury głębokie wbudowano mechanizm miękkiego progowania (ang. *soft thresholding*) jako warstwy przekształceń nieliniowych, co pozwala na eliminację nieistotnych cech. Ponadto, biorąc pod uwagę, że dobór odpowiednich wartości progów jest na ogół trudny, opracowane sieci DRSN integrują kilka specjalizowanych sieci neuronowych jako trenowalne moduły służące do automatycznego wyznaczania tych wartości. Dzięki temu specjalistyczna wiedza ekspercka z zakresu przetwarzania sygnałów nie jest wymagana. Skuteczność opracowanych metod została potwierdzona eksperymentalnie z wykorzystaniem sygnałów zawierających różne rodzaje szumu.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks w diagnostyce uszkodzeń" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks w diagnostyce uszkodzeń" width="100%">
</p>

## Wpływ naukowy

Niniejszy artykuł uzyskał ponad 1400 cytowań w serwisie Google Scholar.

Według ostrożnych szacunków, sieci Deep Residual Shrinkage Networks (DRSN) zostały wykorzystane w ponad 1000 publikacji. Prace te obejmowały bezpośrednie zastosowanie lub udoskonalenie tej architektury w szerokim spektrum dziedzin, w tym w inżynierii mechanicznej, energetyce, widzeniu komputerowym (ang. *computer vision*), ochronie zdrowia, przetwarzaniu mowy, analizie tekstu, technice radarowej oraz teledetekcji.

## Literatura

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
