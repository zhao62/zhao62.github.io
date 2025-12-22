---
layout: post
title: "شبكات الانكماش المتبقية العميقة لتشخيص الأعطال"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-20
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
description: "تتناول هذه المقالة تطوير طرق جديدة في التعلم العميق (Deep Learning)، وتحديداً شبكات الانكماش المتبقية العميقة (Deep Residual Shrinkage Networks)، بهدف تحسين القدرة على تعلم السمات (feature learning) من إشارات الاهتزاز المشوبة بضوضاء عالية، وتحقيق دقة فائقة في تشخيص الأعطال (fault diagnosis)."
---

<!-- 1. 引入谷歌字体 (Noto Naskh Arabic) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;700&display=swap" rel="stylesheet">

<!-- 2. 在这里直接写 CSS，它只会影响这一篇文章 -->
<style>
  /* --- 标题区域设置 --- */
  
  /* H1 主标题：强制使用阿拉伯字体和从右向左排版 */
  header h1, .post-heading h1, .header-section h1, h1.post-title {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important;
    text-align: center !important;
    font-weight: 700 !important;
    line-height: 1.4 !important;
  }
  
  /* 副标题：强制使用英文字体和从左向右排版 */
  header .subheading, .post-heading .subheading, .header-section .subheading {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif !important;
    direction: ltr !important;
    text-align: center !important;
    font-size: 1.1em !important; 
    font-weight: 300 !important;
    margin-top: 15px !important;
    color: #555555 !important; /* 修正：使用深灰色，防止在白底上看不见 */
  }

  /* --- 正文区域设置 --- */

  /* 定义阿拉伯语段落样式 */
  .arabic-text {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important;
    text-align: justify !important; /* 两端对齐 */
    text-align-last: right !important;
    font-size: 1.3em !important; /* 字号加大 */
    line-height: 2.2 !important;  /* 行高加大 */
    margin-bottom: 2em;
  }

  /* 阿拉伯语区域内的小标题 */
  .arabic-text h2, .arabic-text h3 {
    font-family: 'Noto Naskh Arabic', serif !important;
    margin-top: 1.5em;
    margin-bottom: 0.6em;
    font-weight: 700;
  }
  
  /* 英文参考文献区域样式 */
  .ref-header {
    margin-top: 3em !important;
    border-top: 1px solid #eee;
    padding-top: 2em;
    direction: ltr !important;
    text-align: left !important;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif !important;
  }
  
  /* 图片容器样式 */
  .img-container {
    text-align: center;
    margin: 20px 0;
  }
  .img-container img {
    max-width: 100%;
    height: auto;
    border: 1px solid #f0f0f0; /* 给图片加个极淡的边框，更精致 */
  }
</style>

<!-- 作者栏 -->
<div style="text-align: center; color: gray; font-style: italic; margin-bottom: 30px; direction: ltr;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</div>

<!-- 阿拉伯语摘要部分 -->
<div class="arabic-text" markdown="1">

## الملخص (Abstract)

تتناول هذه المقالة تطوير طرق جديدة في التعلم العميق (Deep Learning)، وتحديداً "شبكات الانكماش المتبقية العميقة" (Deep Residual Shrinkage Networks)، بهدف تحسين القدرة على تعلم السمات (feature learning) من إشارات الاهتزاز المشوبة بضوضاء عالية، وتحقيق دقة فائقة في تشخيص الأعطال (fault diagnosis). تم إدراج تقنية "العتبة الناعمة" (Soft Thresholding) كطبقات تحويل غير خطية داخل البنى العميقة للشبكة للتخلص من السمات غير المهمة. وعلاوة على ذلك، ونظراً للتحدي المتمثل في تحديد القيم المناسبة للعتبات يدوياً، تدمج الشبكات المطورة بضع شبكات عصبية متخصصة كوحدات قابلة للتدريب لتحديد العتبات تلقائياً، مما يلغي الحاجة إلى الخبرة التخصصية في معالجة الإشارات. وقد تم التحقق من فعالية الطرق المبتكرة من خلال تجارب أجريت على أنواع مختلفة من الضوضاء.

</div>

<!-- 图片部分 -->
<div class="img-container">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis">
</div>

<div class="img-container">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis">
</div>

<!-- 阿拉伯语影响部分 -->
<div class="arabic-text" markdown="1">

## الأثر الأكاديمي (Academic Impact)

حصلت هذه الورقة البحثية على أكثر من 1400 استشهاد على Google Scholar.

ووفقاً لتقديرات متحفظة، تم استخدام شبكات (DRSN) في أكثر من 1000 منشور علمي. وقد قامت هذه الأعمال إما بتطبيق الشبكة بشكل مباشر أو البناء عليها لتحسينها في مجموعة واسعة من المجالات، بما في ذلك الهندسة الميكانيكية، والطاقة الكهربائية، والرؤية الحاسوبية (Computer Vision)، والرعاية الصحية، ومعالجة الكلام، وتحليل النصوص، والرادار، والاستشعار عن بعد.

</div>

<!-- 英文参考文献部分 -->
<div class="ref-header" markdown="1">

## Reference (المراجع)

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
