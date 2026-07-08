---
tags:
  - Area/Math/Category/AdditiveCategory/AbelianCategory
aliases:
  - Exact Series
---
Let $\mathbf{A}$ be an [[Abelian Category|abelian category]]. The sequence of [[Morphism|morphisms]]
$$\dots\to x\to y\to z\to \dots$$
or
$$0\to x_{1}\to x_{2}\to x_{3}\to\dots\to x_{n}\to0$$
are **complexes** iff the composition of any two consecutive arrows in the sequence is [[Zero Morphism|zero]].

A complex is **exact** if for any part $x\to y\to z$ satisfies $\mathrm{im}(x\to y)=\mathrm{ker}(y\to z)$. Such exact complex is also called a **exact series**.

A **short exact series** is as $0\to a\to b\to c\to0$.


>[!tip] Theorem
>Consider a complex $0\to a\to b \to c\to0$ in abelian category $\mathbf{A}$. Then
> 1. $x\to y \to z \to0$ is exact iff $0\to \mathrm{hom}_{\mathbf{A}}(c,x)\to \mathrm{hom}_{\mathbf{A}}(b,x)\to \mathrm{hom}_{\mathbf{A}}(a,x)$ is an exact sequence of [[Abelian Group|abelian groups]] for all $x\in \mathrm{ob}(\mathbf{A})$.
>2. $0\to x\to y \to z$ is exact iff $0\to\mathrm{hom}_{\mathbf{A}}(x,a)\to \mathrm{hom}_{\mathbf{A}}(x,b)\to \mathrm{hom}_{\mathbf{A}}(x,c)$ is an exact sequence of abelian groups for all $x\in \mathrm{ob}(\mathbf{A})$.

