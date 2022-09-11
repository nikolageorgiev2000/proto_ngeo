---
title: "Continuous Function"
---
Given [[notes/Topological Space|topological spaces]] $\mathcal{X}$ and $\mathcal{Y}$, a function $f:\mathcal{X}\rightarrow\mathcal{Y}$ is *continuous* if the inverse image $f^{-1}(V)=U$ of an open set $V$ of $\mathcal{Y}$ is an open set $U$ of $\mathcal{X}$. Note how this generalizes the notion of a continuous function from real analysis - $f:\mathbb{R}\rightarrow \mathbb{R}$ is continuous at $a$ if $f(a)=\lim_{x\rightarrow a}f(x)$. In other words, a function is continuous when points near $a$ give output near $f(a)$. [Table source](https://math.stackexchange.com/a/962688)
$$\begin{array}{|c|c|}
\hline
\text{Continuity on } \Bbb R & \text{Topological space} \\ \hline
\text{Fix } \varepsilon  & \text{Fix a neighborhood }  V \text{of } f(x_0) \\
\hline
\text{exists } \delta   & \text{exists a neighborhood  }  U \text{of } x_0\\
\hline 
|x-x_0|\le \delta \Rightarrow |f(x)-f(x_0)|\le \varepsilon    & f(U)\subseteq V \\
\hline
 \end{array}$$
