---
layout: post
title: "Deep Residual Shrinkage Networks untuk Diagnosis Kerusakan"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-19
tags: [Kecerdasan Buatan, Diagnosis Kerusakan]
mathjax: true
description: "Artikel ini mengembangkan metode deep learning baru, yaitu Deep Residual Shrinkage Networks, untuk meningkatkan kemampuan pembelajaran fitur (feature learning) dari sinyal getaran yang memiliki tingkat noise tinggi, serta untuk mencapai akurasi diagnosis kerusakan yang tinggi."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Abstrak:

Artikel ini mengembangkan metode *deep learning* baru, yaitu *Deep Residual Shrinkage Networks*, untuk meningkatkan kemampuan pembelajaran fitur (*feature learning*) dari sinyal getaran yang memiliki tingkat *noise* tinggi, serta untuk mencapai akurasi diagnosis kerusakan yang tinggi. *Soft thresholding* disisipkan sebagai lapisan transformasi non-linear ke dalam arsitektur *deep learning* tersebut untuk mengeliminasi fitur-fitur yang tidak penting. Selain itu, mengingat bahwa umumnya sulit untuk menentukan nilai ambang batas (*threshold*) yang tepat secara manual, *Deep Residual Shrinkage Networks* yang dikembangkan ini mengintegrasikan beberapa *neural networks* khusus sebagai modul yang dapat dilatih (*trainable modules*) untuk menentukan *threshold* tersebut secara otomatis, sehingga keahlian profesional dalam pemrosesan sinyal tidak lagi diperlukan. Efektivitas metode yang dikembangkan ini telah divalidasi melalui serangkaian eksperimen menggunakan berbagai jenis *noise*.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks untuk Diagnosis Kerusakan" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks untuk Diagnosis Kerusakan" width="100%">
</p>

## Dampak Akademis

Makalah ini telah menerima lebih dari 1.400 sitasi di Google Scholar.

Menurut estimasi konservatif, *Deep Residual Shrinkage Networks* (DRSN) telah digunakan dalam lebih dari 1.000 publikasi. Karya-karya tersebut telah menerapkan secara langsung ataupun mengembangkan jaringan ini lebih lanjut di berbagai bidang, termasuk teknik mesin, ketenagalistrikan, *computer vision*, kesehatan, pemrosesan wicara (*speech processing*), analisis teks, radar, dan penginderaan jauh (*remote sensing*).

## Referensi

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
