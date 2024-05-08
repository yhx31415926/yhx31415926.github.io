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
![](https://yhx1415926.github.io/quote_img/mathexploration-1/1.png)
&emsp;&emsp;&emsp;&emsp;$P_{1}$任意，任何直径取法
<p>&emsp;&emsp;&emsp;&emsp;4种组合:$\{P_{21},P_{31}\}\ \{P_{21},P_{32}\}\ \{P_{22},P_{31}\}\ \{P_{22},P_{32}\}$</p>
&emsp;&emsp;&emsp;&emsp;都只有一种可行&emsp;&emsp;&emsp;&emsp;故为$\ \ \frac{1}{4}$.<br>
&emsp;&emsp;[可用线性代数规范表述:<br>
&emsp;&emsp;&emsp;&emsp;$O \in \triangle P_{1}P_{2}P_{3}\ \Longleftrightarrow\ \alpha_{1}P_{1}+\alpha_{2}P_{2}+\alpha_{3}P_{3}=O,\ \alpha_{1}+\alpha_{2}+\alpha_{3}=1,\ \alpha _{i}\ge 0$]<br>
&emsp;&emsp;则三维情况完全类似，得$\ \ \frac{1}{8}$.<br>
<p align="right">$\Box$</p><br>

### 22年中科大少创班初试试题4
一圆周上随机分布 $n$ 个点，其可被一 半圆周 覆盖的概率？<br>

同样，考虑 $n$ 条直径, $2^{n}$ 种取法中，当且仅当取出的 $n$ 个点在这 $2n$ 个待选点中连续分布才可行.<br>
易知其有 $2n$ 种.故 $Ans=\frac{2n}{2^{n}}=\frac{n}{2^{n-1}}. $
<p align="right">$\Box$</p><br>

### The 66th Putnam Mathematical Competition(2005) A6
一圆周上随机分布 $n$ 个点，其构成的凸多边形有锐角的概率？
#### Solution-1
$Lemma:\ $此多边形的锐角顶点彼此相邻
//如图所示，左文字，右图片
<div align="center">
<table rules="none">
<tr>
<td>
<img src="https://yhx1415926.github.io/quote_img/mathexploration-1/2.png" style="zoom:50%"/>
</td>
<td>
<p>asdkjhkqjwhkjndskjakdjshakjdhkjashdkjhaskjdhkjahdjhakjsdhkjahdsjhakjdshsakjdhkjahdskjhsakjdhkjahds</p>
<p>asmd</p>
<p>dlkfjdskxknxlkcvsdf,smnf,mwn</p>
</td>
</tr>
</table>    
</div>

#### Solution-2
