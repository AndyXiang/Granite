---
tags:
  - Area/Math/Algebra/VectorSpace/InnerProductSpace/RootSpace
---
Let $E$ be a [[Inner Product Space|inner product space]] over [[Field (Math)|field]] $\mathbb{K}$ with inner product $(\cdot,\cdot):E\times E\to \mathbb{K}$. A **root space** $R$ is a finite [[Subset|subset]] of $E-\{ 0 \}$ such that:
1. $R$ generates $E$, i.e. $E=\mathrm{span}_{\mathbb{K}}(R)$.
2. $\forall\alpha,\beta\in R$, the number $n(\alpha,\beta)=2(\alpha,\beta) /(\beta,\beta)$ is an integer.
3. Let $s_{\alpha}:E\to E$ as $$s_{\alpha}(x)=x-\frac{2(\alpha,x)}{(\alpha,\alpha)}\alpha.$$ Then $\forall\alpha,\beta\in R,s_{\alpha}(\beta)\in R$.

The number $r=\mathrm{dim}(E)$ is called the **rank** of $R$.

A **[[Morphism|morphism]] of root spaces** is a morphism of [[Vector Space|vector spaces]] $f:E_{1}\to E_{2}$ such that $f(R_{1})=R_{2}$ and $n_{f(\alpha)f(\beta)}=n_{\alpha\beta}$ for any $\alpha,\beta\in R_{1}$.

A root space $R$ satisfying that, if $\alpha,k\alpha$ are both roots then $k=\pm1$, is called a **reduced root space**.

## Positive roots and simple roots
Given a root space $R$, we can always choose a subset $R^{+}$ such that
1. For any $\alpha\in R$, exactly one of $\pm \alpha$ is contained in $R^{+}$.
2. For any two distinct $\alpha,\beta\in R^{+}$, if $\alpha+\beta\in R$, then $\alpha+\beta\in R^{+}$.
The elements of $R^{+}$ are called **positive roots**.

This also can be done by choosing a $p\in R$ such that $\forall\alpha\in R,(p,\alpha)\neq0$, then $R^{+}=\{ \alpha\in R:(\alpha,p)>0 \}$.

A positive root is called **simple** if it can not be written as a sum of two positive roots. The set of simple roots is denoted by $\Pi \subset R^+$. $\Pi$ forms a basis of the vector space $E$.

The set $\Pi$ of simple roots can be expressed with [[Dynkin Diagrams|Dynkin diagrams]] which are defined following:
1. For each simple root we construct a vertex.
2. For each pair of distinct simple roots $\alpha_{i},\alpha_{j}$, we connect the corresponding vertices by $n$ edges, where $n$ depends on the angle $\varphi= \arccos\frac{(\alpha_{i},\alpha_{j})}{|\alpha_{i}||\alpha_{j}|}$: 
- $\varphi=\pi /2,n=0$ (vertices are not connected).
- $\varphi=2\pi /3,n=1$.
- $\varphi=3\pi /4,n=2$.
- $\varphi=5\pi/6,n=3$.
3. For each pair of distinct simple roots $\alpha_{i},\alpha_{j}$, if $|\alpha_{i}|\neq|\alpha_{j}|$ and they are not orthogonal, we orient the edge as the longer one pointing towards the shorter one.

Irreducible reduced root spaces are fully class by simple roots and Dynkin diagrams:
![[dynkin_diagrams.png]]