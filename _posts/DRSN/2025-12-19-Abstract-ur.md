---
layout: post
title: "Deep Residual Shrinkage Networks for Fault Diagnosis"
subtitle: "Fault Diagnosis کے لیے Deep Residual Shrinkage Networks"
date: 2025-12-19
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
description: "اس مضمون میں Deep Learning کے نئے طریقے وضع کیے گئے ہیں، جنہیں Deep Residual Shrinkage Networks کا نام دیا گیا ہے۔ ان کا مقصد انتہائی نوائز (noise) والے وائبریشن سگنلز (vibration signals) سے فیچر لرننگ (feature learning) کی صلاحیت کو بہتر بنانا اور فالٹ ڈائیگنوسس (fault diagnosis) میں اعلیٰ درستگی حاصل کرنا ہے۔"
---

<!-- 1. 引入乌尔都语专业字体 (Noto Nastaliq Urdu) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Nastaliq+Urdu:wght@400;700&display=swap" rel="stylesheet">

<!-- 2. 注入精细化 CSS -->
<style>
  /* --- 标题区域设置 --- */
  
  /* H1 大标题：保持英文格式 (从左往右，标准字体) */
  header h1, .post-heading h1, .header-section h1 {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif !important;
    direction: ltr !important; /* 英文从左往右 */
    text-align: center !important;
    font-weight: bold !important;
  }
  
  /* 副标题：设置为乌尔都语格式 (从右往左，书法字体) */
  header .subheading, .post-heading .subheading {
    font-family: 'Noto Nastaliq Urdu', serif !important;
    direction: rtl !important; /* 强制从右往左 */
    text-align: center !important;
    font-size: 1.8em !important; /* 稍微放大一点，因为 Nastaliq 字体偏小 */
    line-height: 1.8 !important;
    margin-top: 10px !important;
  }

  /* --- 正文区域设置 --- */

  /* 定义乌尔都语正文容器 */
  .urdu-text {
    font-family: 'Noto Nastaliq Urdu', serif !important;
    direction: rtl !important;
    text-align: right !important; /* 强制靠右对齐 */
    font-size: 1.3em !important;
    line-height: 2.4 !important;   /* 增加行高，阅读更舒适 */
    margin-bottom: 2em;
  }

  /* 调整乌尔都语标题 (Abstract, Impact) */
  .urdu-text h2 {
    font-family: 'Noto Nastaliq Urdu', serif !important;
    margin-top: 1.5em;
    margin-bottom: 0.8em;
    font-weight: bold;
    font-size: 1.5em;
  }
  
  /* 调整 Reference 标题的样式 */
  .ref-header {
    margin-top: 3em !important;
    border-top: 1px solid #eee;
    padding-top: 2em;
  }
</style>

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

<!-- 乌尔都语正文区域 -->
<div class="urdu-text" markdown="1">

## خلاصہ (Abstract)

اس مضمون میں Deep Learning کے نئے طریقے وضع کیے گئے ہیں، جنہیں Deep Residual Shrinkage Networks کا نام دیا گیا ہے۔ ان کا مقصد انتہائی نوائز (noise) والے وائبریشن سگنلز (vibration signals) سے فیچر لرننگ (feature learning) کی صلاحیت کو بہتر بنانا اور فالٹ ڈائیگنوسس (fault diagnosis) میں اعلیٰ درستگی حاصل کرنا ہے۔ غیر اہم فیچرز کو ختم کرنے کے لیے، ڈیپ آرکیٹیکچرز (deep architectures) میں نان لینیئر ٹرانسفارمیشن لیئرز (nonlinear transformation layers) کے طور پر "Soft Thresholding" کو شامل کیا گیا ہے۔ مزید برآں، یہ دیکھتے ہوئے کہ تھریشولڈز (thresholds) کے لیے مناسب ویلیوز کا تعین کرنا عام طور پر مشکل ہوتا ہے، ان نیٹ ورکس میں چند مخصوص نیورل نیٹ ورکس (neural networks) کو ٹرین ایبل ماڈیولز (trainable modules) کے طور پر ضم کیا گیا ہے۔ یہ خودکار طریقے سے تھریشولڈز کا تعین کرتے ہیں، تاکہ سگنل پروسیسنگ میں کسی خاص پیشہ ورانہ مہارت کی ضرورت نہ رہے۔ تیار کردہ طریقوں کی افادیت کی تصدیق مختلف اقسام کے نوائز (noise) کے ساتھ کیے گئے تجربات کے ذریعے کی گئی ہے۔

</div>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<!-- 乌尔都语正文区域 -->
<div class="urdu-text" markdown="1">

## علمی اثرات (Academic Impact)

اس مقالے کو گوگل اسکالر (Google Scholar) پر 1,400 سے زائد بار حوالہ جات (citations) مل چکے ہیں۔

محتاط اندازوں کے مطابق، Deep Residual Shrinkage Networks (DRSN) کو 1,000 سے زائد اشاعتوں میں استعمال کیا گیا ہے۔ ان تحقیقی کاموں میں مکینیکل انجینئرنگ، الیکٹرک پاور، کمپیوٹر ویژن، ہیلتھ کیئر، اسپیچ پروسیسنگ، ٹیکسٹ اینالیسس، ریڈار، اور ریموٹ سینسنگ سمیت وسیع پیمانے پر شعبوں میں اس نیٹ ورک کا براہ راست اطلاق کیا گیا ہے یا اس میں مزید بہتری لائی گئی ہے۔

</div>

<!-- 英文参考文献区域 (保持 LTR) -->
<div class="ref-header" markdown="1">

## Reference (حوالہ جات)

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
