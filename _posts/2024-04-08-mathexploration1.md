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
### The 53rd Putnam Mathematical Competition(1992) A-6
Four points are chosen at random on the surface of a sphere. What is the probability that the center of the sphere lies inside the tetrahedron whose vertices are at the four points? (It is understood that each point is independently chosen relative to a uniform distribution on the sphere.)  

3Blue1Brown讲解 **key:**<br>
<center><b>将随机取点 看作 随机取直径后取一端点</b></center><br>
&emsp;&emsp;考虑二维简化情况：
<div align="center"><table rules="none"><tr><td>
<p>&emsp;&emsp;&emsp;&emsp;$P_{1}$任意，任何直径取法</p>
<p>&emsp;&emsp;&emsp;&emsp;4种组合:$\{P_{21},P_{31}\}\ \{P_{21},P_{32}\}\ \{P_{22},P_{31}\}\ \{P_{22},P_{32}\}$</p>
<p>&emsp;&emsp;&emsp;&emsp;都只有一种可行&emsp;&emsp;&emsp;&emsp;故为$\ \ \frac{1}{4}$.</p>
</td><td>
<img src="https://yhx1415926.github.io/quote_img/mathexploration-1/1.png" style="zoom:50%"/>
</td></tr></table></div>
&emsp;&emsp;[可用线性代数规范表述:<br>
&emsp;&emsp;&emsp;&emsp;$O \in \triangle P_{1}P_{2}P_{3}\ \Longleftrightarrow\ \alpha_{1}P_{1}+\alpha_{2}P_{2}+\alpha_{3}P_{3}=O,\ \alpha_{1}+\alpha_{2}+\alpha_{3}=1,\ \alpha _{i}\ge 0$]<br>
&emsp;&emsp;则三维情况完全类似，得$\ \ \frac{1}{8}$.<br>
<p align="right">$\Box$</p>

### 22年中科大少创班初试试题4
一圆周上随机分布 $n$ 个点，其可被一 半圆周 覆盖的概率？<br>

同样，考虑 $n$ 条直径, $2^{n}$ 种取法中，当且仅当取出的 $n$ 个点在这 $2n$ 个待选点中连续分布才可行.<br>
易知其有 $2n$ 种.故 $Ans=\frac{2n}{2^{n}}=\frac{n}{2^{n-1}}. $
<p align="right">$\Box$</p>

### The 66th Putnam Mathematical Competition(2005) A6
一圆周上随机分布 $n$ 个点，其构成的凸多边形有锐角的概率？
#### Solution-1
$Lemma:\ $此多边形的锐角顶点彼此相邻<br>
&emsp;&emsp;(可反证.  $\bacause$ 锐角 $\Longleftrightarrow$ 开的半圆  若不相邻，两开的半圆之并为整圆，矛盾.)<br>
因此，有且仅有一顶点 $Q_{1}$ ，使 $\angle Q_{1}$ 为非锐角,但 $\angle Q_{2}$ 为锐角.$^{(\star)}$(序:逆时针)<br>
$\angle Q_{1}OQ_{2}/2\pi:=x\ \ \ \ $ 为使 $\angle Q_{2}$ 为锐角,$Q_{3}\in \overset{\LARGE{\frown}}{Q_{1}^{'}OQ_{1}} $ <br>
<div align="center"><table rules="none"><tr><td>
<p>为使 $\angle Q_{1}$ 为非锐角, $Q_{n}\in \overset{\LARGE{\frown}}{Q_{2}^{'}OQ_{1}}$ 且 $x\le \frac{1}{2}$ </p>
<p>此时概率为 $\left (\frac{1}{2}\right )^{n-2}-x^{n-2}$ (后一项为其余点均落在 $\overset{\LARGE{\frown}}{Q_{1}^{'}OQ_{2}^{'}}$)</p><br>
<p>总概率为 $\int_{0}^{\frac{1}{2}} \left [\left (\frac{1}{2}\right )^{n-2}-x^{n-2}\right]dx=\frac{n-2}{n-1}\cdot \frac{1}{2^{n-1}}$</p>
</td><td>
<img src="https://yhx1415926.github.io/quote_img/mathexploration-1/2.png" style="zoom:50%"/>
</td></tr></table></div>
又 $Q_{1},Q_{2}$ 取法有 $n(n-1)$ 种&emsp;&emsp;&emsp;&emsp;$Ans=n(n-2)\cdot 2^{1-n}$
<p align="right">$\Box$</p>

#### Solution-2

