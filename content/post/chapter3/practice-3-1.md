+++
tags = ["chapter-3"]
categories = ["probability"]
description = "The Answer of Practice 3-1"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 3-1"
date = "2019-05-23"
disable_profile = true 
disable_widgets = false 
+++

## 問1 
離散一様分布の確率分布の確率母関数を求め, 平均と分散を確率母関数から求めよ.

## A.

$A \Delta B = (A \cap B^c) \cup (B \cap A^c)$かつ，これらはdisjointより，
$$ \begin{align}
  P(A \Delta B) &= P(A \cap B^c) + P(B \cap A^c) \\\\\
    & = P(A \setminus (A \cap B)) + P(B \setminus (A \cap B)) \\\\\
    & = P(A) - P(A \cap B) + P(B) - P(A \cap B) \\\\\
    & = P(A \cup B) - P(A \cap B) = P(A) + P(B) - 2 P(A \cap B)
\end{align} $$

