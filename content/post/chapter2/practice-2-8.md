+++
tags = ["chapter-2"]
categories = ["probability"]
description = "The Answer of Practice 2-8"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 2-8"
date = "2019-03-22"
disable_profile = true 
disable_widgets = false 
+++

## 問8 

## A
$y = x - \mu$ とする。 確率変数 $Y$ として、$y \in Y$ とする。

$$
\begin{align}
E[X] &= E[Y + \mu] \\\\ 
&= E[Y] + \mu
\end{align}
$$

ここで、

$$
\begin{align} 
E[Y] &= \int p(y) y dy \\\\ 
&= \int\_{- \infty}^{0} p(y)ydy + \int\_{0}^{\infty} p(y)ydy \\\\ 
&= - \int\_{0}^{\infty} p(-y)ydy + \int\_{0}^{\infty} p(y)ydy \\\\ 
&= 0
\end{align}
$$

よって、 $E[X] = \mu$ が成立。