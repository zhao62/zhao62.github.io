---
layout: post
title: "Fault Diagnosis కోసం Deep Residual Shrinkage Networks"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Artificial Intelligence, Fault Diagnosis]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## సారాంశం (Abstract):

తీవ్రమైన నాయిస్ (noise) ఉన్న వైబ్రేషన్ సిగ్నల్స్ నుండి ఫీచర్లను నేర్చుకునే సామర్థ్యాన్ని మెరుగుపరచడానికి మరియు అత్యంత కచ్చితత్వంతో లోపాలను గుర్తించడానికి (high accuracy), ఈ వ్యాసం "Deep Residual Shrinkage Networks" అనే కొత్త డీప్ లెర్నింగ్ పద్ధతులను అభివృద్ధి చేసింది. ప్రాముఖ్యత లేని ఫీచర్లను తొలగించడానికి, డీప్ ఆర్కిటెక్చర్‌లలో "Soft thresholding"ని నాన్-లీనియర్ ట్రాన్స్‌ఫర్మేషన్ లేయర్‌లుగా జతచేశారు.

అంతేకాకుండా, థ్రెషోల్డ్ (threshold) విలువలను సరిగ్గా నిర్ణయించడం సాధారణంగా కష్టంతో కూడుకున్న పని. అందుకే, ఈ నెట్‌వర్క్‌లలో కొన్ని ప్రత్యేకమైన న్యూరల్ నెట్‌వర్క్‌లను "trainable modules"గా పొందుపరిచారు. ఇవి థ్రెషోల్డ్ విలువలను వాటంతట అవే (automatically) నిర్ణయిస్తాయి. దీనివల్ల సిగ్నల్ ప్రాసెసింగ్‌లో ప్రత్యేక నైపుణ్యం అవసరం ఉండదు. వివిధ రకాల నాయిస్‌లతో చేసిన ప్రయోగాల ద్వారా ఈ పద్ధతుల పనితీరు సమర్థవంతమైనదిగా నిర్ధారించబడింది.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## అకడమిక్ ప్రభావం (Academic Impact):

Google Scholarలో ఈ పరిశోధనా పత్రానికి 1,400 కంటే ఎక్కువ సైటేషన్లు (citations) వచ్చాయి.

సాధారణ అంచనాల ప్రకారం, 1,000కి పైగా ప్రచురణలలో Deep Residual Shrinkage Networks (DRSN) ఉపయోగించబడ్డాయి. మెకానికల్ ఇంజనీరింగ్, ఎలక్ట్రిక్ పవర్, కంప్యూటర్ విజన్, హెల్త్‌కేర్, స్పీచ్ ప్రాసెసింగ్, టెక్స్ట్ అనాలిసిస్, రాడార్ మరియు రిమోట్ సెన్సింగ్ వంటి అనేక రంగాలలో ఈ నెట్‌వర్క్‌ను నేరుగా వాడటం లేదా మరింత మెరుగుపరచడం జరిగింది.

## రిఫరెన్స్ (Reference)

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
