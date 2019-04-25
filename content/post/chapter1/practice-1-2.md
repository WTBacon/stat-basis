+++
tags = ["chapter-1"]
categories = ["probability"]
description = "The Answer of Practice 1-2"
menu = ""
banner = "banners/modern-mathematical-statistics.jpg"
images = []
title = "The Answer of Practice 1-2"
date = "2019-03-19"
disable_profile = true 
disable_widgets = false 
+++

## 問2 
$$
事象 A_1, A_2, A_3 に対して次の等式を示せ.\\\\\\
P(A \cup B) = P(A) +  P(B) - P(A \cap B) \quad より \\\\\\
\begin{align}
P(A_1 \cup (A_2 \cup A_3)) &=  P(A_1) + P(A_2 \cup A_3) - P(A_1 \cap (A_2 \cup A_3)) \\\\\\
&= P(A_1) + P(A_2) + P(A_3) - P(A_2 \cap A_3) -  P(A_1 \cap (A_2 \cup A_3)) \\\\\\
&= P(A_1) + P(A_2) + P(A_3) - P(A_2 \cap A_3) - (P(A_1 \cap A_3) + P(A_1 \cap A_2) - P(A_1 \cap A_2 \cap A_3)) \\\\\\
&= P(A_1) + P(A_2) + P(A_3) - P(A_1 \cap A_2) - P(A_2 \cap A_3) - P(A_3 \cap A_1) + P(A_1 \cap A_2 \cap A_3) \Box
\end{align}
$$


