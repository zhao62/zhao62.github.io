---
layout: post
title: "Глубокие остаточные сети сжатия для диагностики неисправностей"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [искусственный интеллект, диагностика неисправностей]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Аннотация

В данной статье представлены новые методы глубокого обучения, а именно глубокие остаточные сети сжатия (Deep Residual Shrinkage Networks), разработанные для улучшения способности выделения признаков из сильно зашумленных вибрационных сигналов и достижения высокой точности диагностики неисправностей. Для отсеивания несущественных признаков в глубокие архитектуры в качестве слоев нелинейного преобразования внедрена функция мягкой пороговой обработки (soft thresholding). Кроме того, учитывая, что подбор правильных пороговых значений, как правило, представляет сложность, разработанные сети включают в себя несколько специализированных нейронных подсетей. Они выступают в роли обучаемых модулей для автоматического определения порогов, что исключает необходимость в экспертных знаниях в области обработки сигналов. Эффективность предложенных методов подтверждена экспериментально на данных с различными типами шума.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Глубокие остаточные сети сжатия для диагностики неисправностей" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Глубокие остаточные сети сжатия для диагностики неисправностей" width="100%">
</p>

## Академическое влияние

Данная статья набрала более 1400 цитирований в Google Scholar.

По консервативным оценкам, глубокие остаточные сети сжатия (DRSN) использовались более чем в 1000 публикаций. В этих работах данная архитектура либо применялась напрямую, либо была усовершенствована для решения задач в широком спектре областей, включая машиностроение, электроэнергетику, компьютерное зрение (computer vision), здравоохранение, обработку речи, анализ текста, радиолокацию и дистанционное зондирование.

## Литература

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
