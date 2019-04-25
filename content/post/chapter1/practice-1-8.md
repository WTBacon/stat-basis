+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-8"
menu = ""
images = []
title = "The Answer of Practice 1-8"
date = "2019-03-19"
disable_profile = true 
disable_widgets = false 
+++

## 問
$p\left(\bigcap\_{k=1}^{\infty}A\_k\right) \geq 1 - \sum^{\infty}\_{k=1}p(A_k^c)$を示せ．

## A.
$\Omega = \left(\bigcap\_{k=1}^{\infty}A_k\right) \cup \left(\bigcap^{\infty}\_{k=1} A_k\right)^c$
であることに注意する．  
$\left(\bigcap\_{k=1}^{\infty}A_k\right)$と$\left(\bigcap\_{k=1}^{\infty}A_k\right)^c$
は互いに排反であるから，  
\begin{align}
1 = p\left(\bigcap\_{k=1}^{\infty}A_k\right) +
 p\left(\left(\bigcap^{\infty}\_{k=1} A_k\right)^c\right)
\end{align}

ここで，$\left(\bigcap^{\infty}\_{k=1} A_k\right)^c = \left(\bigcup^{\infty}\_{k=1} A_k^c\right)$，
確率の性質 $p\left(\bigcup^{\infty}\_{k=1} A_k\right) \leq \sum^{\infty}\_{k=1}p\left(A_k\right)$より，  
\begin{align}
p\left(\left(\bigcap^{\infty}\_{k=1} A_k\right)^c\right)
 = p\left(\bigcup^{\infty}\_{k=1} A_k^c\right) \leq \sum^{\infty}\_{k=1}p(A_k^c)
\end{align}

よって，
\begin{align}
1 = p\left(\bigcap\_{k=1}^{\infty}A_k\right) +
 p\left(\left(\bigcap^{\infty}\_{k=1} A_k\right)^c\right)
 \leq p\left(\bigcap\_{k=1}^{\infty}A\_k\right) +
   \sum^{\infty}\_{k=1}p(A_k^c)
\end{align}

したがって，
\begin{align}
p\left(\bigcap\_{k=1}^{\infty}A\_k\right) \geq
   1 - \sum^{\infty}\_{k=1}p(A_k^c)
\end{align}