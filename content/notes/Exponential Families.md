---
title: "Exponential Families"
---
An exponential family of probability distributions is associated with a set of functions $\phi=\lbrace \phi_\alpha:\mathcal{X}^m\rightarrow\mathbb{R}|\alpha\in\mathcal{I}\rbrace $ called the sufficient statistics, for index set $\mathcal{I}$. The canonical parameters $\theta=\lbrace \theta_\alpha\in\mathbb{R}|\alpha\in\mathcal{I}\rbrace $ are used to specify the particular distribution within the familty, with probability density
$$p_\theta(x) = \exp\lbrace \theta\cdot\phi(x) - A(\theta)\rbrace $$
where the quantity $A(\theta)$ is the log partition function - provides normalization. Some examples of [[notes/Graphical Models]] can easily be shown to represent exponential families, such as the [[notes/Ising Model]], [[notes/Gaussian MRF]] or [[notes/Gaussian Mixture Model]].