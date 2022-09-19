---
title: "Gaussian Mixture Model"
---
Consider a  multinomial random variable $X$ with values in $\{0,1,\dots,r-1\}$ that specifies the choice of distribution from a collection of $r$ Gaussians parametrized by $\{\mu_j,\sigma^2_j\}$ for $X=j$. The distribution of $X$ is an [[notes/Exponential Families|exponential family]] with sufficient statistics $\{\mathbb{I}_j[x]\}$ and canonical parameters $\alpha$. Each Gaussian $Y$ conditioned on $X$ is also an exponential family with sufficient statistics $\{y,y^2\}$ and canonical parameters $(\gamma_j,\gamma'_j) := (\frac{\mu_j}{\sigma^2_j},-\frac{1}{2\sigma^2_j})$. The resulting PDF is of the form
$$p_{\theta} = p_\alpha(x)p_\gamma(y|x) \propto \exp\left\{\sum_j\alpha_j\mathbb{I}_j[x]\right\} + \sum_j (\gamma_jy+\gamma'_jy^2)\mathbb{I}_j[x]$$
The pair of random variables $(X,Y)$ can be used to create more complex [[notes/Graphical Models]] to describe multivariate distributions of the form $((X_1,Y_1),\dots,(X_m,Y_m))$.