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

## Q. 
離散一様分布の確率分布の確率母関数を求め, 平均と分散を確率母関数から求めよ.

## A.

離散一様分布の確率関数は \

$$ \begin{align} 
p(x) = P(X = x | N) = \frac{1}{N}, x = 1, 2, ... , N \
\end{align} $$ 

であるから, 確率母関数 $G_X(s)$ は \

$$ \begin{align} 
  G_X(s) = \displaystyle\sum\_{k=1}^{N} s^k f(x) & = \frac{1}{N}\displaystyle\sum\_{k=1}^{N} s^k \\\\\
    & = \frac{S^{N+1} - S}{S-1} \\\\\
    & = \underline{\frac{S(S^N-1)}{N(S-1)}}
\end{align} $$

一般に, $ \begin{align} G_{X}^{(k)}(1) = E[X(X-1)\ldots(X-k+1)] \end{align} $ より, 平均 $E[X]$ は, \

$$ \begin{align}
    E[X] = \left.\frac{d{G_X}(s)}{dt}\right|\_{s=1} &= \displaystyle\left.\frac{s(1-s^N)}{N(1-s)}\right|\_{s=1} \\\\\
        &= \left.\frac{1-s^N(1+N)+Ns^{N+1}}{N(1-s)^2}\right|\_{s=1} \\\\\
\end{align}$$

  ここで, ロピタルの定理より, それぞれ2階微分して, 

$$\ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \ \begin{align}
        &=  \displaystyle\lim_{s \to 1}\frac{N(1-N)(1+N)s^{N-2}+N^2(N+1)}{2N} \\\\\
        &=  \frac{N(1-N)(1+N)+N^2(N+1)}{2N} \\\\\
        &=  \underline{\frac{N+1}{2}}
\end{align}$$

また, $E[X(X-1)]$ は, \

$$ \begin{align}
    E[X(X-1)] = \left.\frac{d^2{G_X}(s)}{dt^2}\right|\_{s=1} = \frac{N^2-1}{3} \\\\\
\end{align}$$

であるから, 分散 $Var(X)$ は, 

$$ \begin{align}
    Var(X) = E[X(X-1)] + E[X] - (E[X])^2 &= \frac{N^2-1}{3} + \frac{N+1}{2} + (\frac{N+1}{2})^2\\\\\
                                         &= \underline{\frac{(N-1)(N+1)}{12}}
\end{align}$$



