---
layout: post
title: "电视剧《小欢喜》- 数学题"
subtitle: "Mathematical Exploration"
author: "yhx1415926"
header-style: text
mathjax: true
tags:
  - Mathematical Exploration
---

$N_{+}$ 可以划分成两个集合:
$f(N_{+})=\{f(n)|n\in N_{+}\}$ and $g(N_{+})=\{g(n)|n\in N_{+}\}$;
且 $f(n)$ 严格单增, $g(n)=f(f(n))+1$.
求 $f(240)$.

```python
N = 400

x = [""]*(N+1)

n = 1
m = 1
i = 1

while i<=N:
    x[i] = f"f{n}"
    n += 1
    i += 1
    while x.index(f"f{m}")>=n:
        x[i] = f"f{n}"
        n += 1
        i += 1
    k = x.index(f"f{m}")
    i = x.index(f"f{k}")+1
    x[i] = f"g{m}"
    m += 1
    i += 1

print(x.index("f240"))
```
output:
```python
388
```
