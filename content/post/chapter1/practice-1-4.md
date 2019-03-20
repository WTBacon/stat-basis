+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-4"
menu = ""
images = []
title = "The Answer of Practice 1-4"
date = "2019-03-19"
disable_profile = true
disable_widgets = true
+++

## 問
$p(A|B^c) = 1 - p(A|B)$ を満たさ無い場合を考えよ．  

## A.
$p(A|B^c) + p(A|B) = 1 $ を満たさ無い場合を考えればよい．

すなわち，$p(A|B^c) + p(A|B) \geq 1 $ または $p(A|B^c) + p(A|B) \leq 1 $ となる場合について考える．

[1] $p(A|B^c) + p(A|B) \geq 1 $ となる場合  
  $B \subset A$ のとき，この不等式を満たす．  
  
  $B \subset A$より，  
  $p(A|B) = 1$  
  $B^c \cap A \neq \phi$であるから，  
  $p(A|B^c) \geq 0$  
  よって，$B \subset A$のとき，$p(A|B^c) + p(A|B) \geq 1 $


[2] $p(A|B^c) + p(A|B) \leq 1 $ となる場合
  $A \subset B$ のとき，この不等式を満たす．  
  
  $A \subset B$より，  
  $B^c \cap A = \phi$  $\therefore p(A|B^c)=0$  
  また，$p(A) \leq p(B)$であるから，  
  $p(A|B) = \frac{p(A \cap B)}{p(B)} = \frac{p(A)}{p(B)} \leq 1$  
  よって，$A \subset B$のとき，$p(A|B^c) + p(A|B) \leq 1 $