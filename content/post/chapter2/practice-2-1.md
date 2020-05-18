+++
tags = ["chapter-2"]
categories = ["probability"]
description = "The Answer of Practice 2-1"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 2-1"
date = "2020-05-16"
disable_profile = true 
disable_widgets = false 
+++

## Q. 
次の関数が確率密度関数になるように正規化定数 $C$ を与えよ．また分布関数を求めよ．

## A.
(1) $ \quad f(x)=Cx^{3}, \quad 0<x<2 $ \

正規化定数は，
$$ \begin{equation}
\int\_{-\infty}^{\infty} f_X(x) dx = \int\_{0}^{2} Cx^{3} dx = C \left \[ \frac{1}{4} x^{4} \right \]^{2}\_{0} = 4C = 1 \\\\\
\therefore C = \frac{1}{4}
\end{equation} $$

分布関数は，$0<x<2$ のとき，
$$ \begin{equation}
F_X(x) = \int\_{0}^{x} \frac{1}{4} x^{3} dx = \frac{1}{4} \left \[ \frac{1}{4} x^{4} \right \]^{x}\_{0} =  \frac{1}{16} x^{4} \\\\\
\end{equation} $$

$$ \begin{equation}
\therefore F_X(x) = 
\begin{cases}
\frac{1}{16} x^{4} & (0<x<2) \\\\\[2ex]
0 & (x \leqq 0, 2 \leqq x)
\end{cases}
\end{equation} $$

(2) $ \quad f(x) = Ce^{-|x|}, \quad -\infty<x<\infty $

正規化定数は，
$$ \begin{align}
\int\_{-\infty}^{\infty} f_X(x) dx = \int\_{-\infty}^{\infty} Ce^{-|x|} dx &= \int\_{-\infty}^{0} Ce^{x} dx +  \int\_{0}^{\infty} Ce^{-x} dx \\\\\[2ex]
&= C \left \[ e^{x} \right \]^{0}\_{-\infty} + C \left \[ -e^{-x} \right \]^{\infty}\_{0} \\\\\[2ex]
& = 2C = 1 \\\\\
\end{align} $$

$$ \begin{equation}
\therefore C = \frac{1}{2}
\end{equation} $$

分布関数は，$x<0$ のとき
$$ \begin{equation}
F_X(x) = \int\_{-\infty}^{x} \frac{1}{2} e^{t} dt = \frac{1}{2} e^{x}
\end{equation} $$

$x \geqq 0$ のとき
$$ \begin{equation}
F_X(x) = \int\_{0}^{x} \frac{1}{2} e^{-t} dt = \frac{1}{2} (1-e^{-x})
\end{equation} $$

(3) $ \quad f(x) = Ce^{-2x}, \quad x > 0 $

正規化定数は，
$$ \begin{equation}
\int\_{-\infty}^{\infty} f_X(x) dx = \int\_{0}^{\infty} Ce^{-2x} dx = C \left \[ - \frac{1}{2} e^{-2x} \right \]^{\infty}\_{0} = C \frac{1}{2} = 1 \\\\\[1em]
\therefore C = 2
\end{equation} $$

分布関数は，
$$ \begin{equation}
F_X(x) = \int\_{0}^{x} 2 e^{-2t} dt = \left \[ - e^{-2t} \right \]^{x}\_{0} = -e^{-2x} + 1
\end{equation} $$

(4) $ \quad f(x) = Ce^{-x}e^{-e^{-x}}, \quad x > 0 $

正規化定数は，
$$ \begin{equation}
\int\_{-\infty}^{\infty} f_X(x) dx = \int\_{0}^{\infty} Ce^{-x}e^{-e^{-x}} dx \\\\\
\end{equation} $$

$e^{-x}=t$ とおくと，

$$ \begin{align}
\frac{d}{dx}e^{-x} &= \frac{d}{dx}t \\\\\[1em]
e^{-x}dx &= -dt \quad (0<t<1) \\\\\
\end{align} $$

であるから，

$$ \begin{equation}
\int\_{0}^{\infty} Ce^{-x}e^{-e^{-x}} dx = \int\_{0}^{1} Ce^{-t} (-1)dt = C \left \[ e^{-t} \right \]^{1}\_{0} = C(e^{-1} - 1) = 1 \\\\\
\therefore C = \frac{1}{e^{-1} - 1}
\end{equation} $$

分布関数は，
$$ \begin{equation}
F_X(x) = \int\_{0}^{x} \frac{1}{e^{-1} - 1}e^{-t}e^{-e^{-t}} dt 
\end{equation} $$

$e^{-t}=y$ とおくと，

$$ \begin{align}
\frac{d}{dt}e^{-t} &= \frac{d}{dt}y \\\\\[1em]
e^{-t}dt &= -dy \quad (0<t<1) \\\\\
\end{align} $$

また $ 0<t<x $ より，$ 1<y<e^{-x} $ だから，

$$ \begin{align}
F_X(x) = \int\_{1}^{e^{-x}} \frac{1}{e^{-1} - 1}e^{-y} (-1)dy &= \frac{1}{e^{-1}-1}(-1) \left \[ -e^{-y} \right \]^{e^{-x}}\_{1} \\\\\ 
&= \frac{1}{e^{-1}-1}(-1)(-e^{-e^{-x}} + e^{-1}) \\\\\
&=  \frac{1}{e^{-1}-1}(e^{-e^{-x}}-e^{-1})
\end{align} $$


