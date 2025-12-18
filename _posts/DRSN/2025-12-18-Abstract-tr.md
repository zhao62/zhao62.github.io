---
layout: post
title: "Arıza Teşhisi için Derin Artık Büzülme Ağları (Deep Residual Shrinkage Networks)"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Yapay Zeka, Arıza Teşhisi]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Özet:

Bu çalışmada, yoğun gürültü içeren titreşim sinyallerinden öznitelik öğrenme kabiliyetini geliştirmek ve yüksek arıza teşhis doğruluğuna ulaşmak amacıyla, derin artık büzülme ağları (Deep Residual Shrinkage Networks) adı verilen yeni derin öğrenme yöntemleri geliştirilmiştir. Önemsiz öznitelikleri elemek amacıyla, derin mimarilerin içerisine doğrusal olmayan dönüşüm katmanları olarak yumuşak eşikleme (soft thresholding) entegre edilmiştir. Ayrıca, eşik değerleri için uygun parametreleri belirlemenin genellikle zor olduğu göz önünde bulundurularak; geliştirilen bu ağlar, eşikleri otomatik olarak belirleyen ve eğitilebilir modüller olarak işlev gören bazı özelleşmiş sinir ağlarını bünyesinde barındırır. Bu sayede, sinyal işleme konusunda profesyonel bir uzmanlığa ihtiyaç duyulmaz. Geliştirilen yöntemlerin etkinliği, çeşitli gürültü türleri ile gerçekleştirilen deneylerle doğrulanmıştır.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## Akademik Etki

Bu makale, Google Scholar üzerinde 1.400'den fazla atıf almıştır.

İhtiyatlı tahminlere göre, Derin Artık Büzülme Ağları (DRSN) bugüne dek 1.000'den fazla yayında kullanılmıştır. Bu çalışmalar; makine mühendisliği, elektrik güç sistemleri, bilgisayarlı görü (computer vision), sağlık, konuşma işleme, metin analizi, radar ve uzaktan algılama dahil olmak üzere çok çeşitli alanlarda bu ağı ya doğrudan uygulamış ya da geliştirmiştir.

## Referans

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
