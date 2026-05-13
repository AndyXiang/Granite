---
tags:
  - Area/Math/Algebra/LieAlgebra/SemisimpleLieAlgebra
---
Let $\mathfrak{g}$ be a [[Lie Algebra|Lie algebra]] and $\mathfrak{h}$ be its [[Cartan Subalgebra|Cartan subalgebra]]. For a linear functional $\alpha\in \mathfrak{h}^{*}$, the **root space** of $\alpha$ is the [[Vector Subspace|vector subspace]]
$$
\mathfrak{g}_{\alpha}=\{x\in\mathfrak{g}:\forall h\in\mathfrak{h},[h,x]=\alpha(h)x\}.
$$

Equivalently, $\mathfrak{g}_{\alpha}$ is the simultaneous eigenspace of the commuting operators $\mathrm{ad}_{h}:\mathfrak{g}\to\mathfrak{g}$, $h\in\mathfrak{h}$.

A nonzero $\alpha\in\mathfrak{h}^{*}$ is called a **root** if $\mathfrak{g}_{\alpha}\neq0$. The set of all roots is denoted by
$$
\Delta=\{\alpha\in\mathfrak{h}^{*}-\{0\}:\mathfrak{g}_{\alpha}\neq0\}.
$$

If $\mathfrak{g}$ is a finite-dimensional complex semisimple Lie algebra, then
$$
\mathfrak{g}=\mathfrak{h}\oplus \bigoplus_{\alpha\in\Delta}\mathfrak{g}_{\alpha}.
$$
This is called the **root space decomposition** of $\mathfrak{g}$.

## Coroot
When $\mathfrak{g}$ is finite-dimensional complex semisimple, for each root $\alpha\in\Delta$, the restriction of the [[Killing Form|Killing form]] $B$ to $\mathfrak{h}$ identifies $\alpha$ with a unique element $h_{\alpha}\in\mathfrak{h}$:
$$
\alpha(h)=B(h_{\alpha},h),\forall h\in\mathfrak{h}.
$$
The **coroot** of $\alpha$ is
$$
H_{\alpha}=\frac{2h_{\alpha}}{B(h_{\alpha},h_{\alpha})}.
$$
It is normalized by
$$
\alpha(H_{\alpha})=2.
$$

## Properties
1. $[\mathfrak{g}_{\alpha},\mathfrak{g}_{\beta}]\subset \mathfrak{g}_{\alpha+\beta}$.
2. $\mathfrak{g}_{0}=\mathfrak{h}$ for finite-dimensional complex semisimple $\mathfrak{g}$.
3. $\dim \mathfrak{g}_{\alpha}=1$ for every $\alpha\in\Delta$ when $\mathfrak{g}$ is finite-dimensional complex semisimple.
4. The [[Killing Form|Killing form]] gives a non-degenerate pairing $\mathfrak{g}_{\alpha}\otimes\mathfrak{g}_{-\alpha}\to\mathbb{C}$.

