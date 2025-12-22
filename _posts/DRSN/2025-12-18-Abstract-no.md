---
layout: post
title: "Deep Residual Shrinkage Networks for feildiagnostikk"
subtitle: "Deep Residual Shrinkage Networks for Fault Diagnosis"
date: 2025-12-18
tags: [Kunstig intelligens, feildiagnostikk]
mathjax: true
description: "Denne artikkelen presenterer nye metoder innen dyp læring, nærmere bestemt Deep Residual Shrinkage Networks, for å forbedre evnen til å hente ut egenskaper (feature learning) fra svært støyende vibrasjonssignaler og dermed oppnå høy nøyaktighet ved feildiagnostikk."
---

<p align="center" style="color: gray; font-style: italic;">
  <strong><a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Shisheng Zhong, Xuyun Fu, Baoping Tang, Michael Pecht</strong>
</p>

## Sammendrag

Denne artikkelen presenterer nye metoder innen dyp læring, nærmere bestemt *Deep Residual Shrinkage Networks*, for å forbedre evnen til å hente ut egenskaper (feature learning) fra svært støyende vibrasjonssignaler og dermed oppnå høy nøyaktighet ved feildiagnostikk. *Soft thresholding* implementeres som ikke-lineære transformasjonslag i de dype arkitekturene for å eliminere irrelevante egenskaper.

Videre, ettersom det generelt er utfordrende å fastsette korrekte terskelverdier, integrerer de utviklede nettverkene noen spesialiserte nevrale nettverk som trenbare moduler. Disse bestemmer terskelverdiene automatisk, slik at det ikke kreves inngående ekspertise innen signalbehandling. Metodenes effektivitet er validert gjennom eksperimenter med ulike typer støy.

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_Paper.png" alt="Deep Residual Shrinkage Networks for feildiagnostikk" width="100%">
</p>

<p align="center">
  <img src="/assets/img/DRSN/2025-11-25-DRSN-en/DRSN_en.png" alt="Deep Residual Shrinkage Networks for feildiagnostikk" width="100%">
</p>

## Akademisk innflytelse

Denne artikkelen har mottatt over 1 400 siteringer på Google Scholar.

Ifølge konservative estimater har *Deep Residual Shrinkage Networks* (DRSN) blitt benyttet i mer enn 1 000 publikasjoner. Disse arbeidene har enten anvendt nettverket direkte eller videreutviklet det innen en rekke fagfelt, inkludert maskinteknikk, elkraft, datasyn (computer vision), helse, talebehandling, tekstanalyse, radar og fjernmåling.

## Referanse

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
