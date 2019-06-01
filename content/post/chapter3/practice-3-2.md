+++
tags = ["chapter-3"]
categories = ["probability"]
description = "The Answer of Practice 3-2"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 3-2"
date = "2019-05-27"
disable_profile = true 
disable_widgets = false 
+++

## Q. 
2項係数について (3.4) で与えられた関係式が成り立つことを示せ. また数学的帰納法を用いて2項定理を証明せよ.

## A.
・
$ \begin{align} 
  \displaystyle\sum\_{k=0}^{n} \binom{n}{k} = 2^n 
\end{align} $
について \

二項定理より, $a=1$, $b=1$ のとき, \

$ \begin{align} 
  \underline{\displaystyle\sum\_{k=0}^{n} \binom{n}{k} = 2^n} \\\\\
\end{align} $

が成り立つ.\
\ 

・
$ \begin{align} 
    \binom{n}{k} = \binom{n}{n-k}
\end{align} $
について \

$ \begin{align} 
    \binom{n}{n-k} = \frac{n!}{(n-k)!(n-(n-k))!} &= \frac{n!}{(n-k)!k!} \\\\\
                                                 &= \underline{\binom{n}{k}} 
\end{align} $ \

・
$ \begin{align} 
    \binom{n+1}{k} = \binom{n}{k-1} + \binom{n}{k}
\end{align} $
について \

$ \begin{align} 
    \binom{n}{k-1} + \binom{n}{k} &= \frac{n!}{(k-1)!(n-k+1)!} + \frac{n!}{k!(n-k)!} \\\\\
                                  &= \frac{k \cdot n!}{k(k-1)!(n-k+1)!} + \frac{n! \cdot (n-k+1)}{k!(n-k+1)(n-k)!} \\\\\
                                  &= \frac{(n+1) \cdot n!}{k!(n-k+1)!} \\\\\
                                  &= \frac{(n+1)!}{k!(n-k+1)!} \\\\\
                                  &= \underline{\binom{n+1}{k}} \\\\\
\end{align} $ \


・二項定理の証明について \

$n=1$ のとき \

$ \begin{align} 
  (a+b) = \displaystyle\sum\_{k=0}^{1} \binom{1}{k}a^{k}b^{1-k} = \binom{1}{0}a^{0}b^{1} + \binom{1}{1}a^{1}b^{0} = a + b \\\\\
\end{align} $

$n=m-1$ のとき, \

$ \begin{align} 
  (a+b)^{m-1} = \displaystyle\sum\_{k=0}^{m-1} \binom{m-1}{k}a^{k}b^{m-1-k} \\\\\
\end{align} $ \

が成り立つと仮定して, $n=m$ が成り立つことを示す.\
両辺に $(a+b)$ をかけると, \

$ \begin{align} 
  (a+b)^{m} &= (a+b)\left( \displaystyle\sum\_{k=0}^{m-1} \binom{m-1}{k}a^{k}b^{m-1-k} \right) \\\\\
            &= a \displaystyle\sum\_{k=0}^{m-1} \binom{m-1}{k}a^{k}b^{m-1-k}  + b \displaystyle\sum\_{k=0}^{m-1} \binom{m-1}{k}a^{k}b^{m-1-k} \\\\\
            &= a \left( \displaystyle\sum\_{k=0}^{m-2} \binom{m-1}{k}a^{k}b^{m-1-k} + \binom{m-1}{m-1}a^{m-1}b^{0}  \right) + b \left( \displaystyle\sum\_{k=1}^{m-1} \binom{m-1}{k}a^{k}b^{m-1-k} + \binom{m-1}{0}a^{0}b^{m-1}  \right) \\\\\
            &= a^m + \displaystyle\sum\_{k=0}^{m-2} \binom{m-1}{k}a^{k+1}b^{m-1-k} + b^m + \displaystyle\sum\_{k=1}^{m-1} \binom{m-1}{k}a^{k}b^{m-k}  \\\\\
            &= a^m + \displaystyle\sum\_{k=1}^{m-1} \binom{m-1}{k-1}a^{k}b^{m-k} + b^m + \displaystyle\sum\_{k=1}^{m-1} \binom{m-1}{k}a^{k}b^{m-k}  \\\\\
            &= a^m + b^m + \displaystyle\sum\_{k=1}^{m-1} \left( \binom{m-1}{k-1} + \binom{m-1}{k}\right) a^{k}b^{m-k} \\\\\
            &= a^m + b^m + \displaystyle\sum\_{k=1}^{m-1}\binom{m}{k}a^{k}b^{m-k} \\\\\
            &= \displaystyle\sum\_{k=0}^{m}\binom{m}{k}a^{k}b^{m-k} \\\\\
\end{align} $ \

となり, n=m のとき成り立つことを示せたので, 二項定理は成り立つ.




