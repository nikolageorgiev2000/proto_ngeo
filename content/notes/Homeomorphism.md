---
title: "Homeomorphism"
---
Given [[notes/Topological Space|topological spaces]] $\mathcal{X}$ and $\mathcal{Y}$, a function $g:\mathcal{X}\rightarrow\mathcal{Y}$ is a *homeomorphism* if it:
- is a bijection
- is [[notes/Continuous Function|continuous]]
- has a continuous inverse.
A homeomorphism is explicitly bicontinuous, since there exist bijective functions that are continuous in one direction but discontinuous in the other. For example, the map $\rho = \theta\mapsto e^{i\theta}:[0,2\pi)\to S^1\subset\mathbb{C}$ where $S^1$ is the unit circle on the complex plane. The inverse map $\rho^{-1}$ is not continuous, since $[0,r)$ is an open set of $[0,2\pi)$ for any $r\in(0,2\pi)$, but $\rho([0,r))$ is not an open set of $S^1$ due to the interval being closed on one side.  ([idea source](https://math.stackexchange.com/a/1855569))

If $\mathcal{X}$ is homeomorphic to a subspace in $\mathcal{Y}$, it is called *embedded*.