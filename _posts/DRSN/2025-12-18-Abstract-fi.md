---
layout: post
title: "Deep Residual Shrinkage Networks vianmäärityksessä"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Tekoäly, vianmääritys]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Tiivistelmä

Tässä artikkelissa kehitetään uusia syväoppimismenetelmiä, ns. Deep Residual Shrinkage Network (DRSN) -verkkoja. Menetelmän tavoitteena on parantaa piirteiden oppimiskykyä voimakkaasti kohinaisista värähtelysignaaleista ja saavuttaa korkea tarkkuus vianmäärityksessä. Syviin arkkitehtuureihin on lisätty epälineaarisiksi muunnoskerroksiksi pehmeä kynnystys (soft thresholding), jonka avulla eliminoidaan epäolennaiset piirteet. Koska sopivien kynnysarvojen määrittäminen on yleensä haastavaa, kehitetyt DRSN-verkot hyödyntävät integroituja, erikoistuneita neuroverkkoja. Nämä toimivat opetettavina moduuleina, jotka määrittävät kynnysarvot automaattisesti, jolloin syvällistä signaalinkäsittelyn asiantuntemusta ei vaadita. Kehitettyjen menetelmien tehokkuus on validoitu kokeellisesti käyttämällä erityyppisiä kohinoita.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks vianmäärityksessä" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks vianmäärityksessä" width="100%">
</p>

## Tieteellinen vaikuttavuus

Tämä artikkeli on kerännyt yli 1 400 viittausta Google Scholarissa.

Varovaisen arvion mukaan Deep Residual Shrinkage Network -verkkoja (DRSN) on hyödynnetty yli 1 000 julkaisussa. Näissä töissä on joko sovellettu verkkoa suoraan tai kehitetty sitä edelleen monilla eri aloilla, joihin lukeutuvat muun muassa konetekniikka, sähkövoimatekniikka, tietokonenäkö, terveydenhuolto, puheenkäsittely, tekstianalyysi, tutkat ja kaukokartoitus.

## Viitteet

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
