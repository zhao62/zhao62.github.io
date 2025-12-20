---
layout: post
title: "考慮熱-流-固因素的船用柴油機活塞環數值模擬：從正常到漏氣狀態"
subtitle: "Numerical simulation of piston rings in marine diesel engines considering thermal-fluid-structure factors: From normal to gas leakage conditions"
date: 2025-12-20
tags: [故障診斷, 船用柴油機, 熱流固耦合分析]
mathjax: true
---

<p align="center" style="color: gray; font-style: italic;">
  <strong>Congcong Luo, <a href="https://homepage.hit.edu.cn/zhaominghang?lang=zh" target="_blank">Minghang Zhao</a>, Song Fu, Yan Zhang, Yan Han, Qingqing Huang, Zhiquan Cui</strong>
</p>

針對大型船用柴油機難以進行破壞性試驗的局限，數值模擬（Numerical Simulation）已成為揭示活塞環故障機理及彌補實驗數據缺失的關鍵手段。本文針對活塞環、活塞及氣缸壁系統，建立了一個融合二維流體域與三維活塞環結構的耦合模型，並在考慮熱-流-固（Thermal-Fluid-Structure）多物理場因素的條件下進行求解。相比單一的流體分析，該模型將氣體黏度隨溫度和壓力的變化規律、k-𝜖 湍流模型，以及受力後的活塞環結構變形納入統一計算框架，以模擬氣缸內複雜的物理環境。

<p align="center">
  <img src="/assets/img/LuoNum/Fig1.png" alt="Gas leakage fluid domain" width="90%">
</p>

首先，通過對比活塞環在未磨損與磨損狀態下的工作表現，研究了其微觀變形與燃氣洩漏流場的演變規律，並探討了流體動力學方面的非線性特徵。仿真結果顯示，在正常狀態下的最大爆發壓力時刻，活塞環的截面輪廓仍會產生較為顯著的彈性變形；當活塞環因潤滑失效發生磨損時，隨著磨損間隙增加，儘管洩漏通道變寬導致密封性能下降，但仿真顯示的局部氣體洩漏速度和壓力卻呈下降趨勢，且下降速率逐漸減緩。這一發現透過可視化的速度與壓力雲圖（Contour Map）進行了直觀展示，為理解由磨損引致的洩漏機理提供了新視角。

<p align="center">
  <img src="/assets/img/LuoNum/Fig2.png" alt="Deformation of piston ring" width="90%">
</p>

<p align="center">
  <img src="/assets/img/LuoNum/Fig3.png" alt="Results of piston ring wear" width="100%">
</p>

其次，活塞環黏著（Sticking）可能是導致缸內局部壓力異常升高的主因，其破壞性遠超磨損。當高溫積碳導致活塞環在環槽內受阻無法自由移動時，氣體流動通道被阻塞，致使環間壓力急劇上升。仿真數據顯示，黏著狀態下的氣體最大壓力從正常值的 5.27 MPa 激增至 11.92 MPa，這種劇烈的壓力波動和壓降增加是誘發氣缸套（Cylinder Liner）失效的重要因素。該研究開展了缸內流場的可視化分析，為船用柴油機的故障診斷提供了初步的理論數據支撐。

<p align="center">
  <img src="/assets/img/LuoNum/Fig4.png" alt="Results of piston ring sticking" width="100%">
</p>

參考文獻：

Congcong Luo, Minghang Zhao, Song Fu, Yan Zhang, Yan Han, Qingqing Huang, Zhiquan Cui. Numerical simulation of piston rings in marine diesel engines considering thermal-fluid-structure factors: From normal to gas leakage conditions. In 2024 International Conference on Industrial Automation and Robotics (IAR 2024), October 18–20, 2024, Singapore, Singapore. ACM, New York, NY, USA, 7 pages.

[https://dl.acm.org/doi/10.1145/3707402.3707412](https://dl.acm.org/doi/10.1145/3707402.3707412)

BibTeX:
```bibtex
@inproceedings{Luo2024,
  author    = {Congcong Luo and Minghang Zhao and Song Fu and Yan Zhang and Yan Han and Qingqing Huang and Zhiquan Cui},
  title     = {Numerical simulation of piston rings in marine diesel engines considering thermal-fluid-structure factors: From normal to gas leakage conditions},
  booktitle = {2024 International Conference on Industrial Automation and Robotics (IAR)},
  year      = {2024},
  pages     = {51--57},
  publisher = {ACM},
  doi       = {10.1145/3707402.3707412}
}
```
