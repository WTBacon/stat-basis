+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-1"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-1"
date = "2019-03-19"
disable_profile = true
disable_widgets = true
+++

## 問2 
事象$A$と$B$の対称差$A \Delta B$は，$A \Delta B = A^c \Delta B^c = (A \cup B) \setminus (A \cap B)$と表されることを示して次を示せ．

$$ \begin{align}
  P(A \Delta B) = P(A \cup B) - P(A \cap B) = P(A) + P(B) - 2 P(A \cap B)
\end{align} $$

## A.

$A \Delta B = (A \cap B^c) \cup (B \cap A^c)$かつ，これらはdisjointより，
$$ \begin{align}
  P(A \Delta B) &= P(A \cap B^c) + P(B \cap A^c) \\\\\
    & = P(A \setminus (A \cap B)) + P(B \setminus (A \cap B)) \\\\\
    & = P(A) - P(A \cap B) + P(B) - P(A \cap B) \\\\\
    & = P(A \cup B) - P(A \cap B) = P(A) + P(B) - 2 P(A \cap B)
\end{align} $$

