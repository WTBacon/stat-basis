+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-5"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-5"
date = "2019-03-19"
disable_profile = true
disable_widgets = true
+++

## 問2 
情報を$0$と$1$に符号化して送る際に，受信者は1割の確率で間違って受信してしまう場合を想定してみる．
送信者は，$0$を$1 / 3$の確率，$1$を$2 / 3$の確率で送信していることがわかっている．

1. $0$を受信する確率を求めよ．
2. $0$を受信したとするとき，それが間違って受信した確率を求めよ．$1$を受信したときには，間違って受信する確率はどうなるか．


### A.
Aを送信の事象，Bを受信の事象とすると，

* $P(A = 0) = 1 / 3$
* $P(A = 1) = 2 / 3$
* $P(B = 0 \mid A = 1) = P(B = 1 \mid A = 0) = 1 / 10$

1.

$$ \begin{align}
  P(B = 0) &= P(B = 0 \mid A = 0) \\\\\
  &= P(B = 0 \mid A = 1) P(A = 1) \\\\\
  &= 9 / 10 \cdot 1 / 3 + 1 / 10 \cdot 2 / 3 \\\\\
  &= 11 / 30.
\end{align} $$

2.

$$ \begin{align}
  P(A = 1) &= P(B = 0 \mid A = 0) \\\\\
  &= \frac{P(B = 0 \mid A = 1) P(A = 1)}{P(B = 0)} \\\\\
  &= \frac{1 / 10 \cdot 2 / 3}{11 / 30} \\\\\
  &= 2 / 11.
\end{align} $$

ここで，$P (B = 1)$は以下で計算できる．

$$ \begin{align}
  P(B = 1) &= P(B = 1 \mid A = 0)P(A = 0) + P(B = 1 \mid A = 1) P(A = 1) \\\\\
  &= 1 / 10 \cdot 1 / 3 + 9 / 10 \cdot 2 / 3 \\\\\
  &= 19 / 30.
\end{align} $$

よって，
$$ \begin{align}
  P(A = 0 \mid B = 1) &= \frac{P(B = 1 \mid A = 0)P(A = 0)}{P(B = 1)} \\\\\
  &= \frac{1 / 10 \cdot 1 / 3}{19 / 30} \\\\\
  &= 1 / 19.
\end{align} $$




