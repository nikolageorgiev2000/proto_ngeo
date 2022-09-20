---
title: "Gaussian Mixture Model"
---
Consider a  multinomial random variable $X$ with values in $\lbrace 0,1,\dots,r-1\rbrace$ that specifies the choice of distribution from a collection of $r$ Gaussians parametrized by $\lbrace\mu_j,\sigma^2_j\rbrace$ for $X=j$. The distribution of $X$ is an [[notes/Exponential Families|exponential family]] with sufficient statistics $\lbrace\mathbb{I}_j[x]\rbrace$ and canonical parameters $\alpha$. Each Gaussian $Y$ conditioned on $X$ is also an exponential family with sufficient statistics $\lbrace y,y^2\rbrace$ and canonical parameters $(\gamma_j,\gamma'_j) := (\frac{\mu_j}{\sigma^2_j},-\frac{1}{2\sigma^2_j})$. The resulting PDF is of the form

$$p_\theta = p_\alpha(x)p_\gamma(y|x) \propto \exp\left\lbrace\sum_j\alpha_j\mathbb{I}_j[x] + \sum_j (\gamma_jy+\gamma'_jy^2)\mathbb{I}_j[x]\right\rbrace$$
The pair of random variables $(X,Y)$ can be used to create more complex [[notes/Graphical Models]] to describe multivariate distributions of the form $((X_1,Y_1),\dots,(X_m,Y_m))$.
