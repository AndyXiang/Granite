---
tags:
  - Area/Math/Topology/FiberBundle
  - Area/Math/Algebra/Group
---
Let $G$ be a [[Topological Group|topological group]]. The [[G-Bundle|G-bundle]] $(P,B,G,\pi,G,\mu)$ is called a (right) **principal bundle** as:
1. The total space $P$ has a fiberwise [[Group Action#Basic concepts|free right action]] $\mu:P\times G\to P$ as the diagram commutes
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		P\times G \ar[r, "\mu"] \ar[d, "\pi\times 1"'] & P \ar[d, "\pi"] \\
		B\times \{1\} \ar[r, "\mathrm{proj}"] & B
	\end{tikzcd}
\end{document}
```
2. The induced action on fibers $$\mu: \pi ^{-1}(x)\times G\to \pi ^{-1}(x)$$ is free and [[Group Action#Basic concepts|transitive]].
3. The local trivializations $\phi: \pi ^{-1}(U)\to U\times G$ are [[Group Action#Basic concepts|equivariant]], that is, the diagram commutes
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		\pi^{-1}(U)\times G \ar[r, "\phi\times \mathrm{id}", leftrightarrow] \ar[d, "\mu"] & U\times G\times G \ar[d, "\mathrm{id}\times \mathrm{mul}"] \\
		\pi^{-1}(U) \ar[r, "\phi", leftrightarrow] & U\times G
	\end{tikzcd}
\end{document}
```

 
A principal bundle is trivial iff it admits a [[Fiber Bundle#Section|global section]].

Given a local section $s$ over $U\subset B$, we define a preferred local trivialization $\phi:U\times G\to \pi ^{-1}(U)$ as follow. For $p\in \pi ^{-1}(x),x\in U$, there is a *unique* element $g_{p}\in G$ such that $p=\mu(s(x),g_{p})$. We define $\phi$ by $\phi ^{-1}(p)=(x,g_{p})$, and the section can be expressed as $s(x)=\phi(x,1)$ with identity $1$ of $G$. This is called the **canonical local trivialization** of the principal bundle.

## Connections on principal bundle
Let $G$ be a [[Lie Group|Lie group]] and $\mathfrak{g}$ be its [[Lie Algebra|Lie algebra]]. Let $M$ be a [[Differential Manifold|manifold]]. Consider the principal bundle $(P,M,G,\pi,\mu)$. For $p\in P$ and $m=\pi(p)\in M$, the projection $\pi$ induces a linear map between [[Tangent Space|tangent spaces]] $T_{p}P$ and $T_{m}M$, that is the push-forward $\pi_{*}:T_{p}P\to T_{m}M$. The **vertical subspace** $V_{p}P\subset T_{p}P$ is defined as the kernel $\mathrm{ker} (\pi_{*})$. This means the vectors in $V_{p}P$ have no components in $T_{m}M$, i.e. $\pi_{*}(v)=0$. One can generalize it to a [[Tangent Bundle|vector bundle]] $VP$.

### Geometric definition
A **connection** on principal bundle $(P,M,G,\pi)$ is a unique separation on every point $p$ of $T_{p}P$ into one vertical subspace $V_{p}P$ and its complement $H_{p}P$, called the **horizontal subspace** such that
$$H_{\mu(p,g)}P=\mu_{*}(H_{g})$$
for the right action $\mu:M\times G\to G$.

### Algebraic definition
For any vector $X\in \mathfrak{g}$, its gives a curve lying in fiber $G_{m}\cong G$ on $m$ as $\mu(p, \mathrm{e}^{ tX }):\mathbb{R}\to P$. Such curve has tangent vector belong to $V_{p}P$, we denote it as $\bar{X}$. We now define the **Ehresmann connection** as the $\mathfrak{g}$-value [[Exterior Differential Form|1-form]] $\omega\in \mathfrak{g}\otimes T^{*}P$ satisfying
1. $\omega(\bar{X})=X$.
2. $\mu_{g}^{*}(\omega)=\mathrm{ad}_{g^{-1}}(\omega)$.
Now the horizontal subspace can be defined as the kernel of connection 1-form $H_{p}P=\mathrm{ker}(\omega)$.

The equivalence of these two definition is shown by following proposition

>[!note] Proposition
>The horizontal subspace defined from connection 1-form satisfy $$\mu_{g*}(H_{p}P)=H_{\mu(p,g)}P.$$

*Proof*: For $X\in H_{p}P$, $\mu_{g*}(X)\in T_{\mu(p,g)}P$, and $\omega(\mu_{g*}(X))=\mu_{g}^{*}(\omega)(X)=\mathrm{ad}_{g^{-1}}(\omega(X))=0$, then $\mu_{g*}(X)\in H_{\mu(p,g)}P$. Since $\mu_{g*}$ is invertible, this proves the proposition.