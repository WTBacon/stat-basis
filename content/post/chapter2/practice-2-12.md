+++
tags = ["chapter-2"]
categories = ["probability"]
description = "The Answer of Practice 2-12"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 2-12"
date = "2019-03-22"
disable_profile = true 
disable_widgets = false 
+++

## 問12 

## A

(1) 
$$
\begin{align}
M\_X(t) &= E[e^{tX}] \\\\ 
&= \int\_{0}^{1} f(x) e^{tx} dx \\\\ 
&= \left[ \frac{1}{t} e^{tx} \right]^{1}\_{0} \\\\ 
&= \frac{e^t - 1}{t}
\end{align}
$$

このとき、平均 $E[X]$, 分散 $V[X]$ について、
$$
\begin{align} 
E[X] &= \int\_{0}^{1} x dx = \frac{1}{2} \\\\ 
E[X^2] &= \int\_{0}^{1} x^2 dx = \frac{1}{3} \\\\ 
V[X] &= E[X^2] - (E[X])^2 = \frac{1}{12}
\end{align}
$$

(2)
$$
\begin{align}
F_Y(Y) &= P(Y \leq y) \\\\
&= P(- \sqrt{y} \leq X \leq \sqrt{y}) \\\\ 
&= P(X \leq \sqrt{y}) \\\\ 
&= \int\_{0}^{\sqrt{y}} f(x) dx \\\\ 
&= \sqrt{y} 
\end{align}
$$

より、 $f_Y(y) = \frac{d}{dy} F_Y(y) = \frac{1}{2} y^{-\frac{1}{2}}$。このとき、平均 $E[Y]$, 分散 $V[Y]$ について、
$$
\begin{align}
E[Y] &= \int\_{0}^{1} y f_Y(y) dy = \frac{1}{3} \\\\ 
E[Y^2] &= \int\_{0}^{1} y^2 f_Y(y) dy = \frac{1}{5} \\\\ 
V[Y] &= E[Y^2] - (E[Y])^2 = \frac{4}{45}
\end{align}
$$

(3) 
$Y = - \ln{X}$ の変換には逆関数が存在して、$X = e^{-Y}, (0 \leq Y)$ である。このとき、
$$
f_Y(y) = f(e^{-y}) \mid \frac{d}{dy} e^{-y} \mid = e^{-y}
$$

このとき、平均 $E[Y]$, 分散 $V[Y]$ について、

$$
\begin{align}
E[Y] &= \int\_{0}^{\infty} y e^{-y} dy \\\\ 
&=  \left[ - y e^{-y} \right]\_{0}^{\infty} + \int\_{0}^{\infty} e^{-y} dy \\\\ 
&= \left[ - e^{-y} \right]\_{0}^{\infty} = 1 \\\\ 
E[Y^2] &= \int\_{0}^{\infty} y^2 e^{-y} dy \\\\ 
&= \left[ - y^2 e^{-y} \right]\_{0}^{\infty} + 2 \int\_{0}^{\infty} y e^{-y} dy  = 2\\\\ 
V[Y] &= E[Y^2] - (E[Y])^2 = 1
\end{align}
$$

(4)
$Y = \sigma X + \mu$ の変換には逆関数があり、 $X=\frac{Y - \mu}{\sigma}, (\mu \leq Y \leq \sigma + \mu)$ である。このとき、
$$
f_Y(y) = f_X(\frac{Y - \mu}{\sigma}) \mid \frac{d}{dy} \frac{Y - \mu}{\sigma} \mid = \frac{1}{\sigma}
$$

よって、 $Y$ の従う分布は定義域 $\mu \leq Y \leq \sigma + \mu$ の一様分布である。このとき、
$$
\begin{align}
M_Y(t) &= \int\_{\mu}^{\sigma + \mu}f_Y(y) e^{ty} dy \\\\ 
&= \frac{1}{\sigma} \int\_{\mu}^{\sigma + \mu} e^{ty} dy \\\\ 
&= \frac{1}{t \sigma} (e^{t(\sigma + \mu)} - e^{t \mu}) \\\\ 
E[Y] &= \int\_{\mu}^{\sigma + \mu} \frac{1}{\sigma} y dy = \frac{1}{2}(\sigma + 2 \mu) \\\\ 
E[Y^2] &= \int\_{\mu}^{\sigma + \mu} \frac{1}{\sigma} y^2 dy = \frac{1}{3}(\sigma^2 + 3\mu \sigma + 3 \mu^2) \\\\ 
V[Y] &= E[Y^2] - (E[Y])^2 = \frac{1}{12}\sigma^2
\end{align}
$$