+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-11"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-11"
date = "2019-03-19"
disable_profile = true 
disable_widgets = false 
+++

## 問11
ボレル・カンテリの補題を証明する

## A
(1) 
単調減少列 $B_n = \bigcup^{\infty}\_{k=n}A_k$ として、確率の連続性に着目して、

\begin{align}
P(\limsup\_{n \to \infty} A_n) &= P(\bigcap^{\infty}\_{n=1}\bigcup^{\infty}\
_{k=n}A_k) \\\\ 
&= P(\bigcap^{\infty}\_{n=1}B_n) \\\\ 
&= \lim\_{n \to \infty} P(B_n)
\end{align}

$\sum^{\infty}\_{n=1}P(A_n) \lt \infty$ の前提条件より級数が収束しているので
、$\lim\_{n \to \infty} P(A_n) = 0$ が成立する。よって、$ P(\limsup\_{n \to \infty} A_n) = 0$ が成立。

(2) 
単調増大列 $B_n = \bigcap^{\infty}\_{k=n}A_k$ として、

\begin{align}
P(\limsup\_{n \to \infty}A_n) &= P(\bigcap^{\infty}\_{n=1}\bigcup^{\infty}\_{k=n}A_k) \\\\ 
&= 1 - P(\bigcup^{\infty}\_{n=1}\bigcap^{\infty}\_{k=n}A^{c}\_k) \\\\ 
&= 1 - P(\bigcup^{\infty}\_{n=1}B_n) \\\\ 
&= 1 - \lim\_{n \to \infty} P(B_n) \\\\ 
&= 1 - \lim\_{n \to \infty} P(\bigcap^{\infty}\_{k=n}A^{c}\_k)
\end{align}

ここで、$(A_n)^{\infty}\_{n=1}$ の独立性より、

\begin{align}
P(\bigcap^{\infty}\_{k=n} A^{c}\_k) = \prod^{\infty}\_{k=n} P(A^{c}\_k) = \prod^{\infty}\_{k=n} (1-P(A_k))
\end{align}

ここで、前提条件 $\sum^{\infty}\_{n=1}P(A_n) = \infty$ と $0 \leq P(A_k) \leq 1 \Rightarrow 0 \leq 1 - P(A_k) \leq e^{- P(A_k)}$ であることを用
いて、

\begin{align}
\prod^{\infty}\_{k=n} (1-P(A_k))  \leq \prod^{\infty}\_{k=n} \exp(-P(A_k)) = \exp(- \sum^{\infty}\_{k=n} P(A_k)) = 0
\end{align}

よって、$P(\bigcap^{\infty}\_{k=n}A^{c}\_k) = 0$ となり、 $P(\limsup\_{n \to \infty}A_n)=1$