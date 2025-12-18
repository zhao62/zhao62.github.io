---
layout: post
title: "Deep Residual Shrinkage Networks para el diagnóstico de fallos"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Inteligencia artificial, Diagnóstico de fallos]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Resumen

Este artículo desarrolla nuevos métodos de deep learning (aprendizaje profundo), concretamente las **Deep Residual Shrinkage Networks** (Redes de contracción residual profunda), para mejorar la capacidad de aprendizaje de características a partir de señales de vibración con alto nivel de ruido y lograr una alta precisión en el diagnóstico de fallos. Se introduce el soft thresholding (umbralización suave) a modo de capas de transformación no lineal dentro de las arquitecturas profundas para eliminar características irrelevantes. Además, dado que generalmente resulta difícil establecer los valores adecuados para los umbrales, las redes desarrolladas integran algunas redes neuronales especializadas como módulos entrenables para determinar dichos umbrales de forma automática, de manera que no se requieren conocimientos expertos en procesamiento de señales. La eficacia de los métodos desarrollados queda validada a través de experimentos con diversos tipos de ruido.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="用於故障診斷的深度殘差收縮網絡" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="用於故障診斷的深度殘差收縮網絡" width="100%">
</p>

## Impacto académico

Este artículo ha recibido más de 1.400 citas en Google Scholar.

Según estimaciones conservadoras, las **Deep Residual Shrinkage Networks (DRSN)** se han utilizado en más de 1.000 publicaciones. Estos trabajos han aplicado directamente esta red o la han mejorado en una amplia variedad de campos, que incluyen la ingeniería mecánica, la energía eléctrica, la visión por computador, la medicina, el procesamiento de voz, el análisis de texto, el radar y la teledetección.

## Referencia

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
