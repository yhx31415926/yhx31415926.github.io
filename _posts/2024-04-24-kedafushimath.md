---
layout: post
title: "2024中科大少创班复试"
subtitle: "数学试题（非官方版）"
author: "yhx1415926"
header-style: text
mathjax: true
tags:
  - 中科大
---

### Defination:
1.$ R^{n}$
  <p>\begin{align}d_{1}(x,y)=\sum_{i=1}^{n}{\left | x_{i}-y_{i} \right | }\end{align}</p>
  <p>\begin{align}d_{2}(x,y)=\sqrt{\sum_{i=1}^{n}(x_{i}-y_{i})^{2}}\end{align}</p>
  <p>\begin{align}d_{\infty}(x,y)=\max_{1 \le i \le n}{\left | x_{i}-y_{i} \right | }\end{align}</p>
2.$ Q_{p}$
  <p>\begin{align}d_{p}(x,y)=|x-y|_{p}=p^{-v_{p}(|x-y|)}\end{align}</p>
3.$ A^{n}$
  <p>\begin{align}d_{H}(x,y)=\#\{1\le i\le n|x_{i}\ne y_{i}\} \end{align}</p>

----
共五大题，每题20分。（注意：**题目难度与次序无关**）

### 一、<br>
(1)求证:在 $R^{n}$ 上, $d_{2}$ 构成距离函数.  
(2)求证:在 $R^{n}$ 上，$d_{1},d_{2},d_{\infty}$ 互为等价距离.  

### 二、<br>
<p>$A=\{1,2,...,q\},X=A^{n}.$ 在$ X $上定义$Hamming$距离 $d_{H} ;x\in X;r\in Z,0\le r\le n$<br>
(1)求证：以$x$为球心，$r$为半径的闭球内含$X$的元素个数为<br>
<p>\begin{align}
  \sum_{i=0}^{r}\binom{n}{i} (q-1)^{i}
  \end{align}</p>
(2)依据上一问的结论,试证明:(其他证法不给分)
<p>\begin{align}
  \sum_{i=0}^{n}\binom{n}{i} (q-1)^{i}=q^{n}
  \end{align}</p>

### 三、<br>
(1)求证：单点集$\{x\}$是闭集.<br>
(2)求证：开集的任意并仍为开集.<br>
(3)求证：开集的有限交仍为开集.<br>
(4)在$(Q,d_{p})$下，其中 $d_{p}$为 $p-adic$ 度量.求证：$Z$为非闭集.<br>

### 四、<br>
(1)请写出 $Cauchy$ 列的定义.<br>
(2)对于在 $R$ 上的距离，若$\{x_{n}\}$为 $Cauchy$ 列，$\{y_{n}\}$为 $Cauchy$ 列.求证：$\{x_{n}y_{n}\}$也为 $Cauchy$ 列.<br>
(3)求证：在 $Hamming$ 距离下任意 $Cauchy$ 列，$\exists N,s.t.\ \forall n>N,a_{n}=a_{N}$.<br>

### 五、<br>
在$(Q,d_{p})$下，<br>
(1)求证：$p$ 过所有素数，$d_{p}$ 互不等价.<br>
(2)求证：
<p>\begin{align}
  \lim_{n \to \infty}(1+p)^{p^{n}}=1
  \end{align}</p>
