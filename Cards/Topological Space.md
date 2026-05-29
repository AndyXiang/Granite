---
tags:
  - Area/Math/Topology
---
A **topological space** is a [[Set|set]] $X$ equipped with a set $\tau$ of [[Subset|subsets]] $U \subset X$, which are closed under
1. finite intersection,
2. arbitrary unions,
and contains $\varnothing$ and $X$. These subsets are called **open sets**.

For any set $X$, two general topologies can be defined:
1. *trivial topology*: $\tau=\{ \varnothing,X \}$.
2. *discrete topology*: $\tau=\mathcal{P}(X)$ is the [[Power Set|power set]].

## Related concepts
Let $(X,\tau)$ be a topological space. 
1. A subset $N\subset X$ is the **neighborhood** of $x\in X$ iff $\exists U\in \tau$ s.t. $x\in U\subset N$. If a neighborhood is an open set itself, then we call it an open neighborhood. 
2. A subset $A \subset X$ is **closed** if its complement is open: $X-A\in \tau$. $\varnothing$ and $X$ are both closed and open.
3. The **closure** of $A\subset X$ is the smallest closed set that contains $A$, and is denoted by $\bar{A}$.
4. The **interior** of $A\subset X$ is the largest open set that is contained by $A$, and is denoted by $A^{\circ}$.
5. The **boundary** of $A\subset X$ is the complement of $A^{\circ}$ in $A$: $\partial A=A-A^{\circ}$.