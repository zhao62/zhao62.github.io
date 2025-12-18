---
layout: post
title: "Deep Residual Shrinkage Networks สำหรับการวินิจฉัยความผิดปกติ (Fault Diagnosis)"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [ปัญญาประดิษฐ์, การวินิจฉัยความผิดปกติ]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## บทคัดย่อ:

บทความวิจัยนี้ได้พัฒนาวิธีการเรียนรู้เชิงลึก (Deep Learning) รูปแบบใหม่ที่เรียกว่า "Deep Residual Shrinkage Networks" เพื่อยกระดับความสามารถในการเรียนรู้คุณลักษณะ (Feature Learning) จากสัญญาณการสั่นสะเทือนที่มีสัญญาณรบกวนสูง และเพื่อให้ได้ความแม่นยำในการวินิจฉัยความผิดปกติในระดับสูง

โดยมีการนำฟังก์ชัน Soft Thresholding มาแทรกไว้ในชั้นการแปลงแบบไม่เชิงเส้น (Nonlinear Transformation Layers) ภายในสถาปัตยกรรมโครงข่ายเชิงลึก เพื่อกำจัดคุณลักษณะที่ไม่สำคัญออกไป นอกจากนี้ เนื่องจากโดยทั่วไปการกำหนดค่า Threshold ที่เหมาะสมทำได้ยาก โครงข่าย Deep Residual Shrinkage Networks ที่พัฒนาขึ้นนี้จึงได้ผนวกโครงข่ายประสาทเทียมเฉพาะทางเข้ามาเป็นโมดูลที่สามารถเรียนรู้ได้ (Trainable Modules) เพื่อกำหนดค่า Threshold โดยอัตโนมัติ ทำให้ไม่จำเป็นต้องอาศัยความเชี่ยวชาญเฉพาะด้านการประมวลผลสัญญาณแต่อย่างใด ทั้งนี้ ประสิทธิภาพของวิธีการที่พัฒนาขึ้นได้รับการยืนยันผลผ่านการทดลองกับสัญญาณรบกวนรูปแบบต่างๆ

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## ผลกระทบทางวิชาการ:

บทความวิจัยนี้ได้รับการอ้างอิง (Citations) มากกว่า 1,400 ครั้งบน Google Scholar

จากการประเมินขั้นต่ำ พบว่า Deep Residual Shrinkage Networks (DRSN) ถูกนำไปประยุกต์ใช้ในผลงานตีพิมพ์ทางวิชาการมากกว่า 1,000 ฉบับ ซึ่งงานวิจัยเหล่านี้ได้นำเครือข่ายดังกล่าวไปประยุกต์ใช้โดยตรงหรือนำไปพัฒนาต่อยอดในหลากหลายสาขา อาทิ วิศวกรรมเครื่องกล, ระบบไฟฟ้ากำลัง, คอมพิวเตอร์วิทัศน์ (Computer Vision), การดูแลสุขภาพ, การประมวลผลเสียงพูด, การวิเคราะห์ข้อความ, เรดาร์ และการสำรวจระยะไกล (Remote Sensing)

## เอกสารอ้างอิง

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
