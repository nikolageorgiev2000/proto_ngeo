---
title: "Gaussian Belief Propagation (GBP)"
---
With an understanding of Gaussian algebra, [[notes/Graphical Models|PGMs]], tree decomposition, and variable elimination, it becomes apparent that GBP is nothing more than a clever application of the distributive law. Certain SLAM algorithms can be represented by a factor graph and with a smart choice of elimination ordering, [[notes/Exact Inference]] can be performed using GBP.

![[visuals/factor_graph_slam.png]]