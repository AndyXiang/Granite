---
tags:
  - Area/Physics/QuantumTheory/PathIntegral
  - Area/Physics/FieldTheory/QuantumFieldTheory
---
As an addition to [[Faddeev-Popov Method|Faddeev-Popov method]], the non-abelian [[Gauge Field|gauge field]] [[Gauge Theory|theory]] still has a symmetry after one fixed the gauge. The symmetry is denoted by **Becchi-Rouet-Stora-Tyutin (BRST) symmetry**.

## BRST transformations
Start with Faddeev-Popov modified action
$$S=S_{\mathrm{YM}}+S_{\mathrm{gh}}+S_{\mathrm{FP}}=\int \mathrm{d}^{d}x \left( -\frac{1}{4}F_{a,\mu \nu}F^{a,\mu \nu} -\bar{c}_{a}\Delta^{ab}c_{b}+\frac{1}{2\xi} f_{a}f^{a} \right)$$
where $f[A]$ is the gauge-fixing condition and $\Delta^{ab}[A]=(\delta f^{a}[A^{\Gamma}] /\delta \Gamma_{b})_{\Gamma=0}$. For our purpose, the gauge-fixing term can be expressed with an auxiliary field $B_{a}(x)$:
$$S=\int \mathrm{d}^{d}x\left( -\frac{1}{4}F_{a,\mu \nu}F^{a,\mu \nu}- \bar{c}_{a}\Delta^{ab}c_{b}+\frac{1}{2}\xi B_{a}B^{a}-B_{a}f^{a} \right).$$

This action is not gauge-invariant (since we have gauge-fixed it), but still invariant under BRST transformations as:
$$\delta_{\theta} A_{\mu}^{a}=\theta D_{\mu}c^{a},\delta_{\theta}\bar{c}_{a}=-\theta B_{a}, \delta_{\theta} c_{a}=-\frac{1}{2}\theta C_{ab}^{~~~~c}c^{b}c_{c},\delta_{\theta} B_{a}=0$$
where $C$ is the [[Lie Algebra|structure constant]] and $\theta$ is an infinitesimal [[Grassmann Calculus|Grassmann number]]. For gauge field, it's a gauge transformation: $A_{\mu}^{a}\to A_{\mu}^{a}+D_{\mu}(\theta c^{a})$.

The first important fact here is that this transformation is nilpotent. Define an operator on the field space as $\theta s\phi=\delta_{\theta} \phi$ for $\phi=A,c, \bar{c},B$ and any functional of these fields. Direct computation shows that $s^{2}=0$. By this, we can reformulate the Lagrangian:
$$\mathcal{L}=\mathcal{L}_{\mathrm{YM}}+s\Psi$$
where $\Psi=\bar{c}_{a}f^{a}+\frac{1}{2}\xi  \bar{c}_{a}B^{a}$ and $s(\mathcal{L}_{\mathrm{YM}})=0$. This formula provides us an insight: the physical content is something in the kernel of $s$ modulo the image of $s$. Mathematically speaking, this is the [[de Rham Cohomology Group|cohomology]].