---
layout: post
title: "Deep Residual Shrinkage Networks per la diagnosi dei guasti"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Intelligenza Artificiale, Diagnosi dei guasti]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Abstract

In questo articolo vengono presentati nuovi metodi di deep learning, denominati *Deep Residual Shrinkage Networks* (DRSN), sviluppati per migliorare la capacità di apprendimento delle feature da segnali di vibrazione affetti da forte rumore e per conseguire un'elevata accuratezza nella diagnosi dei guasti. All'interno delle architetture profonde viene inserito il *soft thresholding* come strato di trasformazione non lineare, allo scopo di eliminare le feature irrilevanti. Inoltre, considerando che la definizione dei valori ottimali per le soglie (*thresholds*) risulta generalmente complessa, le *Deep Residual Shrinkage Networks* integrano alcune reti neurali specializzate come moduli addestrabili per determinare tali soglie automaticamente; in questo modo, non sono richieste competenze specialistiche nell'elaborazione dei segnali. L'efficacia dei metodi proposti è stata validata attraverso esperimenti condotti su varie tipologie di rumore.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks per la diagnosi dei guasti" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks per la diagnosi dei guasti" width="100%">
</p>

## Impatto Accademico

Questo articolo ha ricevuto oltre 1.400 citazioni su Google Scholar.

Secondo stime prudenti, le *Deep Residual Shrinkage Networks* (DRSN) sono state utilizzate in più di 1.000 pubblicazioni. Tali lavori hanno applicato direttamente o apportato miglioramenti alla rete in una vasta gamma di settori, tra cui l'ingegneria meccanica, i sistemi elettrici, la *computer vision*, il settore sanitario, l'elaborazione del segnale vocale, l'analisi del testo, i sistemi radar e il telerilevamento.

## Riferimenti

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
