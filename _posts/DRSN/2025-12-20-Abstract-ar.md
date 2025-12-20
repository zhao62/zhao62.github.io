---
layout: post
title: "شبكات الانكماش المتبقية العميقة لتشخيص الأعطال"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-20
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
---

<!-- 1. 引入阿拉伯语专业字体 (Noto Naskh Arabic) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;700&display=swap" rel="stylesheet">

<!-- 2. 注入修正后的 CSS -->
<style>
  /* --- 标题区域设置 (关键修正) --- */
  
  /* H1 主标题：内容是阿拉伯语，必须强制 RTL 和阿拉伯字体 */
  header h1, .post-heading h1, .header-section h1 {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important; /* 修正：从右向左 */
    text-align: center !important;
    font-weight: 700 !important;
    line-height: 1.4 !important;
  }
  
  /* 副标题：内容是英语，必须强制 LTR 和英文系统字体 */
  header .subheading, .post-heading .subheading {
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif !important;
    direction: ltr !important; /* 修正：从左向右 */
    text-align: center !important;
    font-size: 1.1em !important; 
    font-weight: 300 !important;
    margin-top: 15px !important;
    color: #e0e0e0; /* 适配深色/浅色背景，或保持默认 */
  }

  /* --- 正文区域设置 --- */

  /* 定义阿拉伯语正文容器 */
  .arabic-text {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important;
    text-align: justify !important; /* 建议：两端对齐让阿拉伯文排版更像正式文章 */
    text-align-last: right !important; /* 最后一行靠右 */
    font-size: 1.3em !important; /* 稍微调大字号，提升可读性 */
    line-height: 2.2 !important;  /* 增加行高，适应阿拉伯语的元音符号 */
    margin-bottom: 2em;
  }

  /* 调整阿拉伯语小标题 */
  .arabic-text h2, .arabic-text h3 {
    font-family: 'Noto Naskh Arabic', serif !important;
    margin-top: 1.5em;
    margin-bottom: 0.6em;
    font-weight: 700;
  }
  
  /* 调整 Reference 标题区域 */
  .ref-header {
    margin-top: 3em !important;
    border-top: 1px solid #eee;
    padding-top: 2em;
    direction: ltr !important; /* 参考文献主要是英文，保持 LTR */
    text-align: left !important;
  }
</style>

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

<!-- 阿拉伯语正文区域 -->
<div class="arabic-text" markdown="1">

## الملخص (Abstract)

تتناول هذه المقالة تطوير طرق جديدة في التعلم العميق (Deep Learning)، وتحديداً "شبكات الانكماش المتبقية العميقة" (Deep Residual Shrinkage Networks)، بهدف تحسين القدرة على تعلم السمات (feature learning) من إشارات الاهتزاز المشوبة بضوضاء عالية، وتحقيق دقة فائقة في تشخيص الأعطال (fault diagnosis). تم إدراج تقنية "العتبة الناعمة" (Soft Thresholding) كطبقات تحويل غير خطية داخل البنى العميقة للشبكة للتخلص من السمات غير المهمة. وعلاوة على ذلك، ونظراً للتحدي المتمثل في تحديد القيم المناسبة للعتبات يدوياً، تدمج الشبكات المطورة بضع شبكات عصبية متخصصة كوحدات قابلة للتدريب لتحديد العتبات تلقائياً، مما يلغي الحاجة إلى الخبرة التخصصية في معالجة الإشارات. وقد تم التحقق من فعالية الطرق المبتكرة من خلال تجارب أجريت على أنواع مختلفة من الضوضاء.

</div>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<!-- 阿拉伯语正文区域 -->
<div class="arabic-text" markdown="1">

## الأثر الأكاديمي (Academic Impact)

حصلت هذه الورقة البحثية على أكثر من 1400 استشهاد على Google Scholar.

ووفقاً لتقديرات متحفظة، تم استخدام شبكات (DRSN) في أكثر من 1000 منشور علمي. وقد قامت هذه الأعمال إما بتطبيق الشبكة بشكل مباشر أو البناء عليها لتحسينها في مجموعة واسعة من المجالات، بما في ذلك الهندسة الميكانيكية، والطاقة الكهربائية، والرؤية الحاسوبية (Computer Vision)، والرعاية الصحية، ومعالجة الكلام، وتحليل النصوص، والرادار، والاستشعار عن بعد.

</div>

<!-- 英文参考文献区域 -->
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
