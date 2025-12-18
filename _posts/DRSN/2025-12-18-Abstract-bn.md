---
layout: post
title: "ফল্ট ডায়াগনসিসের জন্য ডিপ রেসিডুয়াল শ্রিংকেজ নেটওয়ার্কস"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [আর্টিফিশিয়াল ইন্টেলিজেন্স, ফল্ট ডায়াগনসিস]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## সারাংশ (Abstract)

এই গবেষণাপত্রে 'ডিপ রেসিডুয়াল শ্রিংকেজ নেটওয়ার্কস' নামে নতুন এক ধরণের ডিপ লার্নিং মেথড তৈরি করা হয়েছে। এর মূল লক্ষ্য হলো অত্যধিক নয়েজযুক্ত (highly noised) ভাইব্রেশন সিগন্যাল থেকে ফিচার লার্নিংয়ের সক্ষমতা বৃদ্ধি করা এবং অত্যন্ত নির্ভুলভাবে ফল্ট ডায়াগনসিস নিশ্চিত করা। অপ্রয়োজনীয় ফিচারগুলো বাদ দেওয়ার জন্য এই ডিপ আর্কিটেকচারের মধ্যে নন-লিনিয়্যার ট্রান্সফরমেশন লেয়ার হিসেবে 'Soft thresholding' যুক্ত করা হয়েছে। 

তাছাড়া, থ্রেশহোল্ডের সঠিক মান নির্ধারণ করা সাধারণত বেশ কঠিন একটি কাজ। তাই, এই নেটওয়ার্কটিতে কিছু বিশেষায়িত নিউরাল নেটওয়ার্ককে 'trainable modules' হিসেবে অন্তর্ভুক্ত করা হয়েছে, যা স্বয়ংক্রিয়ভাবে থ্রেশহোল্ড নির্ধারণ করতে পারে। ফলে, এটি ব্যবহারের জন্য সিগন্যাল প্রসেসিংয়ের ওপর বিশেষ কোনো পূর্ব-অভিজ্ঞতার প্রয়োজন হয় না। বিভিন্ন ধরণের নয়েজের ওপর পরীক্ষার মাধ্যমে এই পদ্ধতির কার্যকারিতা প্রমাণ করা হয়েছে।

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for Fault Diagnosis" width="100%">
</p>

## একাডেমিক ইমপ্যাক্ট বা প্রভাব:

গুগল স্কলারে (Google Scholar) এই পেপারটি ১,৪০০ বারেরও বেশি সাইটেশন (citation) লাভ করেছে।

রক্ষণশীল হিসাব অনুযায়ী, ১,০০০-এরও বেশি প্রকাশনায় Deep Residual Shrinkage Networks (DRSN) ব্যবহার করা হয়েছে। মেকানিক্যাল ইঞ্জিনিয়ারিং, ইলেকট্রিক পাওয়ার, কম্পিউটার ভিশন, স্বাস্থ্যসেবা (Healthcare), স্পিচ প্রসেসিং, টেক্সট অ্যানালাইসিস, রাডার এবং রিমোট সেন্সিং-সহ বিচিত্র সব ক্ষেত্রে গবেষকরা হয় সরাসরি এই নেটওয়ার্কটি প্রয়োগ করেছেন, নতুবা এর ওপর ভিত্তি করে আরও উন্নত সংস্করণ তৈরি করেছেন।

## রেফারেন্স (Reference)

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
