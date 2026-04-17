---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
---
Let $M$ be a [[Differential Manifold|manifold]] and $x\in M$. A **differential form** of order $r$ or an **$r$-form** is a totally anti-symmetric [[Tangent Space#Cotangent space & tensor space|tensor]] of type $(0,r)$. The set of all $r$-forms is denoted by $\Omega^{r}_{x}(M)$ at $x\in M$. The dimension of $\Omega^{r}_{x}(M)$ is 
$$\frac{m!}{(m-r)!r!},$$
for $m$ being dimension of $M$.

## Wedge product
The $1$-forms are [[Tangent Space|cotangent vectors]] $\omega\in T^{*}_{x}M$. Higher order forms can be built from $1$-forms with **wedge product** $\wedge$ as
$$\mathrm{d}x^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{r}}\in\Omega^{r}_{x}(M).$$
For example:
$$\mathrm{d}x^{\mu}\wedge \mathrm{d}x^{\nu}=\mathrm{d}x^{\mu}\otimes \mathrm{d}x^{\nu}-\mathrm{d}x^{\nu}\otimes \mathrm{d}x^{\mu}.$$
The wedge product satisfies the following.
1. $\mathrm{d}x^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{r}}=0$ if some index $\mu$ appears at least twice.
2. $\mathrm{d}x^{\mu_{1}} \wedge \cdots \wedge \mathrm{d}x^{\mu_{r}}=\mathrm{sgn}(\sigma)\mathrm{d}x^{\mu_{\sigma(1)}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{\sigma(r)}}$ for [[Permutation|permutation]] $\sigma\in S_{r}$.
3. $\mathrm{d}x^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{r}}$ is linear in each $\mathrm{d}x^{\mu}$.

Every $r$-form can be expanded as
$$\omega=\frac{1}{r!}\omega_{\mu_{1}\cdots\mu_{r}}\mathrm{d}x^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{r}}.$$
In other words, the wedge products of $1$-forms are basis of $\Omega_{x}^{r}(M)$. 

As a generalization, the wedge product of a $q$-form and an $r$-form is a $(q+r)$-form if $q+r\leq m$ as
$$\omega \wedge \xi=\frac{1}{q!r!}\omega_{\mu_{1}\cdots\mu_{q}} \xi_{\nu_{1}\cdots \nu_{r}}\mathrm{d}x^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}x^{\mu_{q}}\wedge \mathrm{d}x^{\nu_{1}} \wedge \cdots \wedge \mathrm{d}x^{\nu_{r}}.$$
If $q+r>m$, the wedge product is zero.
