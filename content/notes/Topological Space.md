---
title: "Topological Space"
---
A topological space $\mathcal{X}$, also denoted $(\mathcal{S},\mathcal{T})$, is a collection containing the empty set, $\mathcal{S}$, and an associated topology $\mathcal{T}$ - a set of neighborhoods (subsets) of $\mathcal{S}$. Formally, the elements of  $\mathcal{T}$ are *open sets*, since the open set for a point $p\in \mathcal{S}$ will contain all other points sufficiently near $p$. Note, a set is considered *closed* if its complement is open.

Given topological spaces $\mathcal{X}$ and $\mathcal{Y}$, a function $f:\mathcal{X}\rightarrow\mathcal{Y}$ is *continuous* if the inverse image $f^{-1}(V)=U$ of an open set $V$ of $\mathcal{Y}$ is an open set $U$ of $\mathcal{X}$. Note how this generalizes the notion of a continuous function from real analysis - $f:\mathbb{R}\rightarrow \mathbb{R}$ is continuous at $a$ if $f(a)=\lim_{x\rightarrow a}f(x)$. In other words, a function is continuous when points near $a$ give output near $f(a)$. [Table source](https://math.stackexchange.com/a/962688)
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
A function $g:\mathcal{X}\rightarrow\mathcal{Y}$ is a *homeomorphism* if it:
- is a bijection
- is continuous
- has a continuous inverse.
Note a homeomorphism is explicitly bicontinuous, since there exist bijective functions that are continuous in one direction but discontinuous in the other. For example, the map $\rho = \theta\mapsto e^{i\theta}:[0,2\pi)\to S^1\subset\mathbb{C}$ where $S^1$ is the unit circle on the complex plane. The inverse map $\rho^{-1}$ is not continuous, as  ([idea source](https://math.stackexchange.com/a/1855569))

If $\mathcal{X}$ is homeomorphic to a subspace in $\mathcal{Y}$, it is called *embedded*. 
