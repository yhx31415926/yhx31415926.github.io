---
layout: post
title: "D维球 N个点 半球覆盖 概率"
subtitle: "Mathematical Exploration"
author: "yhx1415926"
header-style: text
mathjax: true
tags:
  - Mathematical Exploration
---

## Introduction
### The 53rd Putnam Mathematical Competition A-6
Four points are chosen at random on the surface of a sphere. What is the probability that the center of the sphere lies inside the tetrahedron whose vertices are at the four points? (It is understood that each point is independently chosen relative to a uniform distribution on the sphere.)  

3Blue1Brown讲解 **key:**<br>
<center><b>将随机取点 看作 随机取直径后取一端点</b></center><br>
&emsp;&emsp;考虑二维简化情况：
![](https://yhx1415926.github.io/quote_img/mathexploration-1/1.png)
&emsp;&emsp;&emsp;&emsp;$P_{1}$任意，任何直径取法<br>
<p>&emsp;&emsp;&emsp;&emsp;4种组合:$\{P_{21},P_{31}\}\ \{P_{21},P_{32}\}\ \{P_{22},P_{31}\}\ \{P_{22},P_{32}\}$</p><br>
&emsp;&emsp;&emsp;&emsp;都只有一种可行&emsp;&emsp;&emsp;&emsp;故为$\ \ \frac{1}{4}$<br>
&emsp;&emsp;可用线性代数规范表述:<br>
&emsp;&emsp;&emsp;&emsp;$O \in \triangle P_{1}P_{2}P_{3}\ \Longleftrightarrow\ \alpha_{1}P_{1}+\alpha_{2}P_{2}+\alpha_{3}P_{3}=O,\ \alpha_{1}+\alpha_{2}+\alpha_{3}=1,\ \alpha _{i}\ge 0$<br>
&emsp;&emsp;则三维情况完全类似，得$\ \ \frac{1}{8}$<br>
<p align="right">$\Box$</p><br>
