---
layout: post
title: "Deep Residual Shrinkage Networks for Fault Diagnosis"
subtitle: "شبكات الانكماش المتبقية العميقة لتشخيص الأعطال"
date: 2025-12-20
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
---

<!-- 1. 引入阿拉伯语专业字体 (Noto Naskh Arabic) -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@400;700&display=swap" rel="stylesheet">

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
  
  /* 副标题：设置为阿拉伯语格式 (从右往左，标准 Naskh 字体) */
  header .subheading, .post-heading .subheading {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important; /* 强制从右往左 */
    text-align: center !important;
    font-size: 1.6em !important; 
    line-height: 1.6 !important;
    margin-top: 10px !important;
  }

  /* --- 正文区域设置 --- */

  /* 定义阿拉伯语正文容器 */
  .arabic-text {
    font-family: 'Noto Naskh Arabic', serif !important;
    direction: rtl !important;
    text-align: right !important; /* 强制靠右对齐 */
    font-size: 1.2em !important;
    line-height: 2.0 !important;   /* 阿拉伯语 Naskh 字体不需要像乌尔都语那么大的行高，2.0 很舒适 */
    margin-bottom: 2em;
  }

  /* 调整阿拉伯语标题 */
  .arabic-text h2 {
    font-family: 'Noto Naskh Arabic', serif !important;
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

<!-- 英文参考文献区域 (保持 LTR) -->
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
