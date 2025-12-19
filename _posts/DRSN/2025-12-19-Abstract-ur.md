---
layout: post
title: "Fault Diagnosis کے لیے Deep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-19
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## خلاصہ (Abstract)

اس مضمون میں Deep Learning کے نئے طریقے وضع کیے گئے ہیں، جنہیں Deep Residual Shrinkage Networks کا نام دیا گیا ہے۔ ان کا مقصد انتہائی نوائز (noise) والے وائبریشن سگنلز (vibration signals) سے فیچر لرننگ (feature learning) کی صلاحیت کو بہتر بنانا اور فالٹ ڈائیگنوسس (fault diagnosis) میں اعلیٰ درستگی حاصل کرنا ہے۔ غیر اہم فیچرز کو ختم کرنے کے لیے، ڈیپ آرکیٹیکچرز (deep architectures) میں نان لینیئر ٹرانسفارمیشن لیئرز (nonlinear transformation layers) کے طور پر "Soft Thresholding" کو شامل کیا گیا ہے۔ مزید برآں، یہ دیکھتے ہوئے کہ تھریشولڈز (thresholds) کے لیے مناسب ویلیوز کا تعین کرنا عام طور پر مشکل ہوتا ہے، ان نیٹ ورکس میں چند مخصوص نیورل نیٹ ورکس (neural networks) کو ٹرین ایبل ماڈیولز (trainable modules) کے طور پر ضم کیا گیا ہے۔ یہ خودکار طریقے سے تھریشولڈز کا تعین کرتے ہیں، تاکہ سگنل پروسیسنگ میں کسی خاص پیشہ ورانہ مہارت کی ضرورت نہ رہے۔ تیار کردہ طریقوں کی افادیت کی تصدیق مختلف اقسام کے نوائز (noise) کے ساتھ کیے گئے تجربات کے ذریعے کی گئی ہے۔

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## علمی اثرات (Academic Impact)

اس مقالے کو گوگل اسکالر (Google Scholar) پر 1,400 سے زائد بار حوالہ جات (citations) مل چکے ہیں۔

محتاط اندازوں کے مطابق، Deep Residual Shrinkage Networks (DRSN) کو 1,000 سے زائد اشاعتوں میں استعمال کیا گیا ہے۔ ان تحقیقی کاموں میں مکینیکل انجینئرنگ، الیکٹرک پاور، کمپیوٹر ویژن، ہیلتھ کیئر، اسپیچ پروسیسنگ، ٹیکسٹ اینالیسس، ریڈار، اور ریموٹ سینسنگ سمیت وسیع پیمانے پر شعبوں میں اس نیٹ ورک کا براہ راست اطلاق کیا گیا ہے یا اس میں مزید بہتری لائی گئی ہے۔

## حوالہ جات (Reference)

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
