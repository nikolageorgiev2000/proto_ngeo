---
title: "Ising Model"
---
In statistical physics, the Ising Model is classically used to model the directions of "spin" in a magnet. It is an example of a [[notes/Graphical Models|graphical model]] associated with an [[notes/Exponential Families|exponential family]]. In particular, consider the PDF
$$p_\theta(x) = \exp\left\lbrace \sum_{s\in V}\theta_sx_s + \sum_{(s,t)\in E} \theta_{st}x_sx_t - A(\theta) \right\rbrace$$
where $x\in\lbrace 0,1\rbrace^m$ represents the spin (up or down) of $m$ dipoles in an abstraction of the material. The sufficient statistics enables variation of the magnetic field strength per spin dipole, as well as pair-wise spin interactions. A generalized Ising Model allows for $k$-cliques rather than only interaction between pairs of nodes. In the extreme, where all monomials up to $k=m$ are considered, any distribution over a binary random vector can be represented.