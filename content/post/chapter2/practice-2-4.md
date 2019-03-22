+++
tags = ["chapter-2"]
categories = ["probability"]
description = "The Answer of Practice 2-4"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 2-4"
date = "2019-03-22"
disable_profile = true
disable_widgets = true
+++

## 問4 
連続型確率変数 $X$ について、$E[(X - t)^2], E[\mid X - t \mid]$ をそれぞれ最小にする $t$ を求めよ

## A
- $E[(X-t)^2]$ を最小にする $t$

$$
\begin{align}
f(t) &= E[(X-t)^2] \\\\ 
&= \int p(x) (x - t)^2 dx \\\\ 
&= t^2 -2 t \int p(x) x dx + \int p(x) x^2 dx 
\end{align}
$$

とする。このとき $f(t)$ は凸関数であり、 $ \frac{d}{dt} f(t) = 2t - 2 \int p(x) x dx = 0 $ とすると、解は $t= \int p(x) x dx = E[X]$ 

- $E[\mid X - t \mid]$ を最小にする $t$ 

1. $\mid X - t \mid = X - t$ の場合、

$$ \begin{eqnarray}
E[\mid X - t \mid] &= E[X - t] \\\\ 
&= E[X] - t 
\end{eqnarray}
$$

より、$t = E[X]$

2. $\mid X - t \mid = t - X$ の場合、

$$ \begin{eqnarray}
E[\mid X - t \mid] &= E[t - X] \\\\ 
&= t - E[X] 
\end{eqnarray}
$$

より、$t = E[X]$
