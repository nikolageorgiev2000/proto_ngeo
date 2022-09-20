---
title: "Graphical Models"
---
There are a variety of graphical models, which explicitly represent the structure of a joint PDF.  Three popular variants are described below. The more general framework of describing interaction between nodes - think particles - using graphs is extremely versatile.

## Bayesian Networks
A Bayesian network $\mathcal{B}=(V,E)$ is a directed acyclic graph (DAG). Its nodes $V = \lbrace X_1\dots X_n\lbrace$ represent random variables and the edges $E \subset V\times V$ show conditional dependencies. It encodes a probability distribution where factors are either a prior of a variable, or a posterior conditioned on its parents. If we denote the parent nodes of $X_i$ as $\pi_i$, the joint PDF over $n$ variables is defined as
$$p_{X_1\dots X_n}(x_1\dots x_n) = \prod_i p(x_i|\pi_i)p(x_i)$$

## Markov Random Fields
A Markov random field (MRF) is an undirected graph $\mathcal{M}=(V,E)$, which encodes conditional independence between variables in a joint PDF. For example, in a three node graph $X-Z-Y$, the joint probability is $p_{XYZ}(x,y,z) = p_{X|Z}(x;z)p_{Y|Z}(y;z)p_Z(z)$. In particular, since all paths between nodes $X$ and $Y$ on the graph pass through node $Z$, we deduce that $X$ and Y are independent conditioned on $Z$. This is similar to the Markov property and motivates a factorization over cliques $\lbrace (X,Z),(Y,Z)\lbrace$. A clique is a complete induced subgraph and is maximal when it is not contained within a larger clique. If nodes in $V$ are grouped into a set of maximal cliques $C$, the joint probability represented by the undirected graph can be written as a product of potential functions with inputs in $C$ and normalizing partition function $Z$.
$$p_{X_1\dots X_n}(x_1\dots x_n) =\frac{1}{Z}\prod_{c\,\in C} \psi_{c}(x_{c}) $$
A DAG can be converted to an undirected graph through moralization -- fully connecting each node's parents. This can result in loss of some conditional independencies though.

## Factor Graphs
Factor graph $\mathcal{F}=(V,E,F)$ is an undirected bipartite graph with edges $E\subseteq V\times F$ between nodes $V$ representing random variables and nodes $F$ for factors, making the factorization explicit. A variable connected to a factor means it is given as input to the factor function. Hence, the joint PDF with normalizing partition function $Z$ can be expressed as:
$$p_{X_1\dots X_n}(x_1\dots x_n) =\frac{1}{Z}\prod_{\phi\,\in F} \phi(x_{\phi})$$