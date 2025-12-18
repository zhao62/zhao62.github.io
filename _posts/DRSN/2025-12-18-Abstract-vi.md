---
layout: post
title: "Mạng Deep Residual Shrinkage ứng dụng trong Chẩn đoán Lỗi"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Trí tuệ nhân tạo, Chẩn đoán lỗi]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Tóm tắt:

Bài báo này phát triển các phương pháp học sâu (deep learning) mới, cụ thể là mạng **Deep Residual Shrinkage Networks**, nhằm nâng cao khả năng học đặc trưng từ các tín hiệu rung động bị nhiễu nặng, đồng thời đạt được độ chính xác cao trong chẩn đoán lỗi. Kỹ thuật **Soft thresholding** được đưa vào các kiến trúc sâu như những lớp biến đổi phi tuyến để loại bỏ các đặc trưng không quan trọng. Hơn nữa, nhận thấy việc thiết lập giá trị ngưỡng (thresholds) phù hợp thường gặp nhiều khó khăn, mạng Deep Residual Shrinkage được phát triển để tích hợp một số mạng nơ-ron chuyên dụng đóng vai trò là các mô-đun có thể huấn luyện (trainable modules) nhằm tự động xác định các ngưỡng này. Nhờ đó, phương pháp này không đòi hỏi kiến thức chuyên môn sâu về xử lý tín hiệu. Hiệu quả của các phương pháp đề xuất đã được kiểm chứng thông qua các thực nghiệm với nhiều loại nhiễu khác nhau.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## Tác động học thuật:

Bài báo này đã nhận được hơn 1.400 lượt trích dẫn trên Google Scholar.

Theo ước tính thận trọng, Deep Residual Shrinkage Networks (DRSN) đã được sử dụng trong hơn 1.000 công trình công bố. Các công trình này đã áp dụng trực tiếp hoặc cải tiến mạng DRSN trên nhiều lĩnh vực đa dạng, bao gồm kỹ thuật cơ khí, điện lực, thị giác máy tính (computer vision), y tế, xử lý tiếng nói, phân tích văn bản, radar và viễn thám (remote sensing).

## Tài liệu tham khảo

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
