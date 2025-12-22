---
layout: post
title: "फॉल्ट डायग्नोसिस (Fault Diagnosis) के लिए Deep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [आर्टिफिशियल इंटेलिजेंस, फॉल्ट डायग्नोसिस]
mathjax: true
description: "यह लेख अत्यधिक शोर (noise) वाले वाइब्रेशन सिग्नल्स (vibration signals) से फीचर लर्निंग (feature learning) की क्षमता को बेहतर बनाने और उच्च फॉल्ट डायग्नोसिस एक्यूरेसी (accuracy) प्राप्त करने के लिए 'Deep Residual Shrinkage Networks' नामक नई डीप लर्निंग विधियां विकसित करता है। महत्वहीन फीचर्स को हटाने के लिए डीप आर्किटेक्चर (deep architectures) में 'नॉन-लीनियर ट्रांसफॉर्मेशन लेयर्स' (nonlinear transformation layers) के रूप में 'सॉफ्ट थ्रेशोल्डिंग' (Soft thresholding) को शामिल किया गया है।"
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## एब्स्ट्रैक्ट (Abstract):

यह लेख अत्यधिक शोर (noise) वाले वाइब्रेशन सिग्नल्स (vibration signals) से फीचर लर्निंग (feature learning) की क्षमता को बेहतर बनाने और उच्च फॉल्ट डायग्नोसिस एक्यूरेसी (accuracy) प्राप्त करने के लिए 'Deep Residual Shrinkage Networks' नामक नई डीप लर्निंग विधियां विकसित करता है। महत्वहीन फीचर्स को हटाने के लिए डीप आर्किटेक्चर (deep architectures) में 'नॉन-लीनियर ट्रांसफॉर्मेशन लेयर्स' (nonlinear transformation layers) के रूप में 'सॉफ्ट थ्रेशोल्डिंग' (Soft thresholding) को शामिल किया गया है।

इसके अलावा, चूंकि थ्रेशोल्ड (thresholds) के लिए सही मान (values) निर्धारित करना आमतौर पर चुनौतीपूर्ण होता है, इसलिए विकसित किए गए Deep Residual Shrinkage Networks में कुछ विशेष न्यूरल नेटवर्क्स को 'ट्रेनेबल मॉड्यूल' (trainable modules) के रूप में एकीकृत किया गया है। ये मॉड्यूल अपने आप थ्रेशोल्ड निर्धारित करते हैं, जिससे सिग्नल प्रोसेसिंग (signal processing) में पेशेवर विशेषज्ञता की आवश्यकता नहीं पड़ती। विकसित विधियों की प्रभावकारिता (efficacy) को विभिन्न प्रकार के शोर (noise) के साथ किए गए प्रयोगों के माध्यम से सत्यापित (validate) किया गया है।

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## अकादमिक प्रभाव (Academic Impact)

इस पेपर को Google Scholar पर 1,400 से अधिक साइटेशन (citations) प्राप्त हुए हैं।

अनुमानों के अनुसार, 1,000 से अधिक प्रकाशनों में Deep Residual Shrinkage Networks (DRSN) का उपयोग किया गया है। इन कार्यों ने मैकेनिकल इंजीनियरिंग, इलेक्ट्रिक पावर, कंप्यूटर विज़न, हेल्थकेयर, स्पीच प्रोसेसिंग, टेक्स्ट एनालिसिस, रडार और रिमोट सेंसिंग सहित कई क्षेत्रों में इस नेटवर्क को या तो सीधे लागू किया है या इसमें सुधार किया है।

## संदर्भ (Reference)

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
