+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-3"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-3"
date = "2019-03-19"
disable_profile = true
disable_widgets = true
+++

## 問3
(1.2) を示せ

## A
帰納的に示す。

- $n=2$ のとき

$P(A_1) \gt 0$ のとき、 $P(A_1 \cap A_2) = P(A_2 \mid A_1)P(A_1)$ は条件付き確率の定義より成立。

- $n=k$ のとき

$$P(A_1 \cap ... \cap A_k) = P(A_k \mid A_1 \cap ... \cap A\_{k-1}) \times ... \times P(A_2 \mid A_1) \times P(A_1)$$ 

を仮定する。$B = A_1 \cap ... \cap A_k$ とおいて、 $P(B) \gt 0$ のとき、条件付き確率の定義より、

$$
\begin{align}
P(B \cap A_\{k+1})&=P(A\_{k+1} \mid B)P(B) \\\\ 
&=P(A\_{k+1} \mid A_1 \cap ... \cap A_k) \times P(A_k \mid A_1 \cap ... \cap A\_{k - 1}) \times ... \times P(A_2 \mid A_1) \times P(A_1)
\end{align}
$$ 

よって、すべての $n$ で (1.2) が成立する。