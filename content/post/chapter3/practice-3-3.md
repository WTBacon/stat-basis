+++
tags = ["chapter-3"]
categories = ["probability"]
description = "The Answer of Practice 3-3"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 3-3"
date = "2019-05-27"
disable_profile = true 
disable_widgets = false 
+++

## Q. 
超幾何分布について,$\quad \displaystyle\sum\_{x=0}^{K}P(X=x|N,M,K)=1 \quad$  を満たすことを示し, \\
また, $p=M/N$ に対して平均と分散は次のようになることを示せ. \

$$ \begin{align} 
   \displaylines{E[X]=Kp, \quad Var(X)=\frac{N-K}{N-1}Kp(1-p)} 
\end{align} $$

## A.

はじめに, $\displaystyle\sum\_{x=0}^{K}P(X=x|N,M,K)=1$ について示す.  この式は, \
$$ \begin{align} 
   \binom{N}{K} = \displaystyle\sum\_{x=0}^{K}\binom{M}{x}\binom{N-M}{K-x} \tag{1} 
\end{align} $$

と書き直すことができるため, これを示せば良い. \
そのためには, $ \ \ (a+b)^N = (a+b)^M(a+b)^{N-M}$ の両辺をそれぞれ2項展開をして, $ \ a^{K}b^{N-K}$ の項の係数を比較することで示せる. \
それぞれ二項展開すると, \

$$ \begin{align} 
  \displaystyle\sum\_{k=0}^{N}\binom{N}{k}a^{k}b^{N-k} = \displaystyle\sum\_{l=0}^{M}\binom{M}{l}a^{l}b^{M-l}\displaystyle\sum\_{m=0}^{N-M}\binom{N-M}{m}a^{m}b^{N-M-m}  \tag{2}
\end{align} $$

となり, 両辺から$a^{K}b^{N-K}$の係数を取り出して比較する.この時, $a^{K}b^{N-K} =(a^{x}b^{M-x}) \cdot (a^{K-x}b^{N-M-K+x})$ と分解できることに注意すると, \
(2)式の左側の$\ a^{x}b^{M-x}\ $の係数は$\ \binom{M}{x}\ $, 右側の$\ a^{K-x}b^{N-M-K+x}\ $の係数は$\ \binom{N-M}{K-x}\ $であり, その２つを掛けると$\ (a+b)^M(a+b)^{N-M}\ $となる.\
ただし, $\ x \ $は $\ 0 \leq x \leq K \ $ を満たす整数で $\ (K+1)\ $ 通りあるので, 

$$ \begin{align} 
  \binom{N}{K} = \displaystyle\sum\_{x=0}^{K}\binom{M}{x}\binom{N-M}{K-x} 
\end{align} $$

となり, (1)式が成り立つことが示せた.\

次に, $\ E[X]=Kp\ $ を示す.

$$ \begin{align} 
    E[X] &= \displaystyle\sum\_{x=0}^{K}x\frac{\binom{M}{x}\binom{N-M}{K-x}}{\binom{N}{K}}  \\\\\ 
    \binom{N}{K}E[X] &= \displaystyle\sum\_{x=1}^{K}x\frac{M!}{x!(M-x)!}\frac{(N-M)!}{(K-x)!(N-M-K+x)!}  \quad (\because x=0のとき0になる) \\\\\
                     &= \displaystyle\sum\_{x=1}^{K}\frac{M!}{(x-1)!(M-x)!}\frac{(N-M)!}{(K-x)!(N-M-K+x)!} \\\\\
                     &= \displaystyle\sum\_{x=1}^{K} \frac{M \cdot (M-1)!}{(x-1)!\lbrace (M-1)-(x-1)\rbrace !} \cdot \frac{\lbrace (N-1)-(M-1)\rbrace !}{\lbrace (K-1)-(x-1)\rbrace !\[\lbrace (N-1)-(M-1)\rbrace - \lbrace (K-1)-(x-1)\rbrace \]!} \\\\\
                     &= M \cdot \displaystyle\sum\_{x=1}^{K}\binom{M-1}{x-1}\cdot \binom{(N-1)-(M-1)}{(K-1)-(x-1)} \\\\\    
                     &= M \cdot \displaystyle\sum\_{y=0}^{K-1}\binom{M-1}{y}\cdot \binom{(N-1)-(M-1)}{(K-1)-y}   \quad (\because y=x-1とおくy) \\\\\
                     &= M \cdot \binom{N-1}{K-1}   \quad (\because 式(1) より) \\\\\
    E[X] &= M \cdot \frac{\binom{N-1}{K-1}}{\binom{N}{K}} \\\\\
         &=  M \cdot \frac{(N-1)!}{(K-1)!(N-K)!} \cdot \frac{K!(N-K)!}{N!} \\\\\
         &= K\frac{M}{N} = KP    \quad (\because \frac{M}{N}=P より)
\end{align} $$ \

次に, $\ Var(X)=\frac{N-K}{N-1}Kp(1-p)\ $を示す.
$$ \begin{align} 
    V[X] = E[X(X-1)] +E[X]-(E[X])^2
\end{align} $$ \
より, 
$$ \begin{align} 
    E[X(X-1)] &= \displaystyle\sum\_{x=0}^{K}x\frac{\binom{M}{x(x-1)}\binom{N-M}{K-x}}{\binom{N}{K}}  \\\\\ 
    \binom{N}{K}E[X] &= \displaystyle\sum\_{x=2}^{K}x(x-1)\frac{M!}{x!(M-x)!}\frac{(N-M)!}{(K-x)!(N-M-K+x)!}  \quad (\because x=0,x=1のとき0になる) \\\\\
                     &= \displaystyle\sum\_{x=2}^{K}\frac{M!}{(x-2)!(M-x)!}\frac{(N-M)!}{(K-x)!(N-M-K+x)!} \\\\\
                     &= \displaystyle\sum\_{x=2}^{K} \frac{M \cdot (M-1)\cdot (M-2)!}{(x-2)!\lbrace (M-2)-(x-2)\rbrace !} \cdot \frac{\lbrace (N-2)-(M-2)\rbrace !}{\lbrace (K-2)-(x-2)\rbrace !\[\lbrace (N-2)-(M-2)\rbrace - \lbrace (K-2)-(x-2)\rbrace \]!} \\\\\
                     &= M(M-1) \cdot \displaystyle\sum\_{x=2}^{K}\binom{M-2}{x-2}\cdot \binom{(N-2)-(M-2)}{(K-2)-(x-2)} \\\\\    
                     &= M(M-1) \cdot \displaystyle\sum\_{y=0}^{K-2}\binom{M-2}{y}\cdot \binom{(N-2)-(M-2)}{(K-2)-y}   \quad (\because y=x-2とおくy) \\\\\
                     &= M(M-1) \cdot \binom{N-2}{K-2}   \quad (\because 式(1) より) \\\\\
    E[X(X-1)] &= M(M-1) \cdot \frac{\binom{N-2}{K-2}}{\binom{N}{K}} \\\\\
              &= M(M-1) \cdot \frac{(N-2)!}{(K-2)!(N-K)!} \cdot \frac{K!(N-K)!}{N!} \\\\\
              &= K(K-1)\frac{M(M-1)}{N(N-1)} \\\\\
    V[X] &= K(K-1)\frac{M(M-1)}{N(N-1)} + K\frac{M}{N} - K^2\frac{M^2}{N^2} \\\\\
         &= \frac{NM(M-1)K(K-1)+MKN(N-1)-M^2K^2(N-1)}{N^2(N-1)} \\\\\ 
         &= \frac{MK(\cancel{NMK}-NM-NK+\cancel{N}+N^2\cancel{-N}\cancel{-MKN}+MK)}{N^2(N-1)} \\\\\ 
         &= \frac{MK(N-K)(N-M)}{N^2(N-1)} \\\\\ 
\end{align} $$ \

