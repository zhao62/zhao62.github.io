---
layout: post
title: "கோளாறுகளைக் கண்டறிதலுக்கான (Fault Diagnosis) Deep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## சுருக்கம் (Abstract):

அதிக இரைச்சல் கொண்ட (highly noised) அதிர்வு சிக்னல்களிலிருந்து (vibration signals) தகவல்களைப் பிரித்தெடுக்கும் திறனை மேம்படுத்தவும், மிகத் துல்லியமாக இயந்திரக் கோளாறுகளைக் கண்டறியவும், இந்த ஆய்வுக் கட்டுரையில் "Deep Residual Shrinkage Networks" எனப்படும் புதிய Deep Learning முறைகள் உருவாக்கப்பட்டுள்ளன.

முக்கியமற்ற தகவல்களை (features) நீக்குவதற்காக, இந்த Deep architecture-களுக்குள் "Soft thresholding" எனும் முறை Nonlinear transformation layer-களாகச் சேர்க்கப்பட்டுள்ளது. மேலும், Threshold-களுக்கான சரியான மதிப்புகளை மனிதர்களால் நிர்ணயிப்பது பொதுவாகக் கடினமான ஒன்றாகும். இதைக் கருத்தில் கொண்டு, உருவாக்கப்பட்ட இந்த Deep Residual Shrinkage Network-கள், தாமாகவே Threshold-களை நிர்ணயிக்கும் வகையில், சில பிரத்யேக Neural network-களைத் தங்களுக்கிடையே கொண்டுள்ளன. இதனால், Signal processing குறித்த நிபுணர்களின் உதவி இல்லாமலே இது சிறப்பாகச் செயல்படும். பல்வேறு வகையான இரைச்சல்களைக் (noise) கொண்ட சோதனைகள் மூலம் இம்முறைகளின் செயல்திறன் உறுதிப்படுத்தப்பட்டுள்ளது.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## கல்விசார் தாக்கம் (Academic Impact):

இந்த ஆய்வுக் கட்டுரை Google Scholar-ில் 1,400-க்கும் மேற்பட்ட மேற்கோள்களைப் (citations) பெற்றுள்ளது.

குறைந்தபட்ச மதிப்பீடுகளின்படி, 1,000-க்கும் மேற்பட்ட வெளியீடுகளில் Deep Residual Shrinkage Networks (DRSN) பயன்படுத்தப்பட்டுள்ளன. மெக்கானிக்கல் இன்ஜினியரிங், மின்சக்தி (Electric Power), Computer Vision, சுகாதாரம், Speech Processing, Text Analysis, ரேடார் மற்றும் Remote Sensing உள்ளிட்ட பல்வேறு துறைகளில் இந்த நெட்வொர்க் நேரடியாகப் பயன்படுத்தப்பட்டுள்ளது அல்லது மேம்படுத்தப்பட்டுள்ளது.

## மேற்கோள் (Reference)

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
