+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-9"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-9"
date = "2019-03-19"
disable_profile = true 
disable_widgets = false 
+++

## 問9
集合の列$A_k \in \mathfrak{B}, k = 1,2,\cdots,$に対して，上極限集合と下極限集合をそれぞれ

$$ \begin{align}
\limsup _ {n \to \infty} A _ n &= \bigcap _ {n = 1}^{\infty} \bigcup _ {k=n}^{\infty} A _ k, \\\\\
\liminf _ {n \to \infty} A _ n &= \bigcup _ {n = 1}^{\infty} \bigcap _ {k=n}^{\infty} A _ k
\end{align} $$
で定義する．
$\limsup _ {n \to \infty} A _ n = \liminf _ {n \to \infty} A _ n$が成り立つとき，この集合を$\lim _ {n \to \infty} A _ n$とかく．
$A _ k$が単調増大列のとき，$\lim _ {n \to \infty} A _ k = \bigcup _ {n = 1} ^{\infty} A _ n$となることを示せ．
また$A _ k$が単調減少列のとき，$\lim _ {n \to \infty} A _ n = \bigcap _ {n =1} ^{\infty} A _ n$となることを示せ．


## A.

### $A _ k$が単調増大列のとき
$A _ k \subset A _ {k+1}, k=1,\cdots,$のとき，$\bigcup _ {k=m}^{\infty}$は全ての$m$について等しくなるので，
$$ \begin{align}
\limsup _ {n \to \infty} A _ n &= \bigcap _ {n = 1}^{\infty} \bigcup _ {k=n}^{\infty} A _ k = \bigcup _ {n=1}^{\infty} A _ n.
\end{align} $$

また，$\bigcap _ {k=m}^{\infty} A _ k = A _ m$より，$\liminf _ {n \to \infty} A _ n = \bigcup _ {n = 1}^{\infty} \bigcap _ {k=n}^{\infty} A _ k = \bigcup _ {n=1}^{\infty} A _ n$.
よって，上極限集合と下極限集合が等しくなり，
$$ \begin{align}
  \lim _ {n \to \infty} A _ k = \bigcup _ {n = 1} ^{\infty} A _ n.
\end{align} $$

### $A _ k$が単調減少列のとき
$A _ {k+1} \subset A _ {k}, k=1,\cdots,$のとき，全ての$k$について$\bigcap _ {k=m}^{\infty} A _ k$は全ての$m$について等しくなるので，
$$ \begin{align}
  \liminf _ {n \to \infty} A _ n &= \bigcup _ {n = 1}^{\infty} \bigcap _ {k=n}^{\infty} A _ k = \bigcap _ {n = 1}^{\infty} A _ n.
\end{align} $$
また，$\bigcup _ {k=m} ^{\infty} A _ k = A _ m$より，
$$ \begin{align}
  \limsup _ {n \to \infty} A _ n &= \bigcap _ {n = 1}^{\infty} \bigcup _ {k=n}^{\infty} A _ k = \bigcap _ {n=1}^{\infty} A _ n.
\end{align} $$
よって，上極限集合と下極限集合が等しくなり，
$$ \begin{align}
  \lim _ {n \to \infty} A _ k = \bigcap _ {n = 1} ^{\infty} A _ n.
\end{align} $$

