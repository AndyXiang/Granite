---
tags:
  - Area/Math/Set
aliases:
  - Equivalence Class
---
Consider a [[Set|set]] $X$, a **equivalence relation** $\sim$ is a [[Relation|relation]] satisfying
1. reflexivity: $\forall x\in X,x\sim x$.
2. symmetric: $\forall x,y\in X,x\sim y \implies y\sim x$.
3. transitivity: $\forall x,y,z\in X,x\sim y,y\sim z\implies x\sim z$.

Any equivalent relation on set $X$ gives a [[Partition|partition]] of $X$
$$X /\simeq \{ [x]:x\in X \}$$
where $[x]=\{ x'\in X:x' \sim x \}$ is called the **equivalence class** of $x$.


>[!theorem] Equivalence relations and partitions
>Let $S$ be a nonempty set and $\sim$ be an equivalence relation on $S$. Then $\sim$ yields a [[Partition|partition]] of $S$, where each cell
> $$\bar{a}=\{ x\in S:x\sim a \}.$$
> Also each partition of $S$ yields an equivalence relation $\sim$ such that $\forall a,b\in S, a\sim b$ iff $a,b$ are in the same cell.

