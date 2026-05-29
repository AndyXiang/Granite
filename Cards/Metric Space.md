---
tags:
  - Area/Math/Topology
---
A **metric** is the [[Map|map]] $d:X\times X\to \mathbb{R}$ that satisfies following conditions:
1. *symmetric*: $d(x,y)=d(y,x)$;
2. *non-negative*: $d(x,y)\geq0$ where the equality holds iff $x=y$;
3. *triangule inequality*: $d(x,y)+d(y,z)\geq d(x,z)$,
for any $x,y,z\in X$. The set equipped with a metric is called a **metric space**.

If $X$ is endowed with a metric $d$, $X$ is made in to a [[Topological Space|topological space]] whose open sets are given by *open ball*
$$B(x,\epsilon)=\{ y\in X|d(x,y)<\epsilon \},$$
and all their possible unions. This topology thus defined is called the **metric topology** determined by $d$.