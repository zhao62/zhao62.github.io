---
layout: post
title: "Deep Residual Shrinkage Networks zur Fehlerdiagnose"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Künstliche Intelligenz, Fehlerdiagnose]
mathjax: true
description: "Dieser Artikel entwickelt neue Deep-Learning-Methoden, konkret Deep Residual Shrinkage Networks, um die Fähigkeit zum Erlernen von Merkmalen (Feature Learning) aus stark verrauschten Vibrationssignalen zu verbessern und eine hohe Genauigkeit bei der Fehlerdiagnose zu erzielen."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Zusammenfassung

Dieser Artikel entwickelt neue Deep-Learning-Methoden, konkret Deep Residual Shrinkage Networks, um die Fähigkeit zum Erlernen von Merkmalen (Feature Learning) aus stark verrauschten Vibrationssignalen zu verbessern und eine hohe Genauigkeit bei der Fehlerdiagnose zu erzielen. Soft Thresholding wird dabei als nichtlineare Transformationsschicht in die tiefen Architekturen integriert, um irrelevante Merkmale zu eliminieren. Da es zudem generell schwierig ist, geeignete Werte für die Schwellenwerte festzulegen, integrieren die entwickelten Deep Residual Shrinkage Networks einige spezialisierte neuronale Netze als trainierbare Module. Diese bestimmen die Schwellenwerte automatisch, sodass kein Expertenwissen im Bereich der Signalverarbeitung erforderlich ist. Die Wirksamkeit der entwickelten Methoden wird durch Experimente mit verschiedenen Arten von Rauschen validiert.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks zur Fehlerdiagnose" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks zur Fehlerdiagnose" width="100%">
</p>

## Akademischer Einfluss

Diese Arbeit verzeichnet über 1.400 Zitationen auf Google Scholar.

Nach konservativen Schätzungen wurden Deep Residual Shrinkage Networks (DRSN) bereits in mehr als 1.000 Publikationen eingesetzt. Diese Arbeiten haben das Netzwerk in einem breiten Spektrum von Anwendungsfeldern entweder direkt angewandt oder weiterentwickelt, darunter Maschinenbau, Energietechnik, Computer Vision, Gesundheitswesen, Sprachverarbeitung, Textanalyse, Radar und Fernerkundung.

## Referenz

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
