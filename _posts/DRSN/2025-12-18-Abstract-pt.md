---
layout: post
title: "Deep Residual Shrinkage Networks para Diagnóstico de Falhas"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Inteligência Artificial, Diagnóstico de Falhas]
mathjax: true
description: "Este artigo desenvolve novos métodos de deep learning, especificamente as Deep Residual Shrinkage Networks (Redes Residuais Profundas de Contração), para aprimorar a capacidade de aprendizado de características (feature learning) a partir de sinais de vibração altamente ruidosos e alcançar uma elevada precisão no diagnóstico de falhas."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Resumo

Este artigo desenvolve novos métodos de deep learning, especificamente as Deep Residual Shrinkage Networks (Redes Residuais Profundas de Contração), para aprimorar a capacidade de aprendizado de características (feature learning) a partir de sinais de vibração altamente ruidosos e alcançar uma elevada precisão no diagnóstico de falhas. A técnica de soft thresholding é inserida como camadas de transformação não linear nas arquiteturas profundas para eliminar características irrelevantes. Além disso, considerando que geralmente é desafiador definir valores adequados para os limiares (thresholds), as redes desenvolvidas integram sub-redes neurais especializadas como módulos treináveis para determinar os limiares automaticamente, dispensando a necessidade de conhecimento especializado em processamento de sinais. A eficácia dos métodos desenvolvidos é validada por meio de experimentos com diversos tipos de ruído.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks para Diagnóstico de Falhas" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks para Diagnóstico de Falhas" width="100%">
</p>

## Impacto Acadêmico

Este artigo recebeu mais de 1.400 citações no Google Scholar.

Segundo estimativas conservadoras, as Deep Residual Shrinkage Networks (DRSN) foram utilizadas em mais de 1.000 publicações. Estes trabalhos aplicaram diretamente ou aprimoraram a rede numa vasta gama de campos, incluindo engenharia mecânica, setor elétrico, visão computacional, saúde, processamento de fala, análise de texto, radar e sensoriamento remoto.

## Referência

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
