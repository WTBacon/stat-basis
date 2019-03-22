+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-7"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-7"
date = "2019-03-19"
disable_profile = true
disable_widgets = true
+++

## 問7
書籍参照

## A
(1) 変数間に因果関係がないとき、独立であるとする。変数間が独立のときは以下が成立する。

$$\begin{eqnarray}
P(A_1 \cap B_1) &= P(A_1)P(B_1) \\\\ 
P(A_1 \cap B_2) &= P(A_1)P(B_2) \\\\ 
P(A_2 \cap B_1) &= P(A_2)P(B_1) \\\\ 
P(A_2 \cap B_2) &= P(A_2)P(B_2) 
\end{eqnarray} $$

これを用いて、 

$$
a = \frac{2}{9}, b = \frac{2}{3}, c = \frac{1}{3}, d = \frac{2}{9} 
$$

と解ける。

(2) 独立性が仮定できないとき、変数間には以下が成立する。

$$\begin{eqnarray}
P(A_1 \cap B_1) &= P(A_1 \mid B_1)P(B_1) \\\\ 
P(A_1 \cap B_2) &= P(A_1 \mid B_2)P(B_2) \\\\ 
P(A_2 \cap B_1) &= P(A_2 \mid B_1)P(B_1) \\\\ 
P(A_2 \cap B_2) &= P(A_2 \mid B_2)P(B_2) 
\end{eqnarray} $$

これを用いて、

$$
a = \frac{4}{9} - d, b = \frac{8}{9} - d, c = \frac{8}{9} - d 
$$

と解ける。
