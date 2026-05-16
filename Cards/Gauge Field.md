---
tags:
  - Area/Physics/FieldTheory
  - Area/Physics/GaugeTheory
  - Area/Math/Topology/FiberBundle
---
Consider a [[Lie Group|Lie group]] $G$ as the [[Gauge Theory|gauge group]]. Let $\mathfrak{g}$ be its [[Lie Algebra|Lie algebra]]. Given a [[Principal Bundle|principal bundle]] $P(M,G)$, and its [[Principal Bundle#Connections on principal bundle#Algebraic definition|connection]] $\omega\in \mathfrak{g}\otimes \Omega(P)$ and a [[Fiber Bundle#Section|local section]] $\sigma:M\to P$ defined on the [[Neighborhood|neighborhood]] $U$, the **gauge field** is
$$\mathcal{A}=\sigma ^{*}\omega\in \mathfrak{g}\otimes \Omega(U).$$
In coordinate basis $\mathcal{A}=A_{\mu}\mathrm{d}x^{\mu}$.

## Field strength and curvature
Define the **field strength** by the [[Curvature (Principal Bundle)|curvature]] $\Omega\in \mathfrak{g}\otimes\Omega^{2}(P)$ as
$$\mathcal{F}=\sigma ^{*}\Omega\in \mathfrak{g}\otimes \Omega^{2}(U).$$
It satisfies
1. $\mathcal{F}=\mathrm{d}\mathcal{A}+\mathcal{A}\wedge \mathcal{A}$. In coordinate basis, $\mathcal{F}=F_{\mu \nu}\mathrm{d}x^{\mu}\wedge \mathrm{d}x^{\nu}$, then $F_{\mu \nu}=\partial_{\mu}A_{\nu}-\partial_{\nu}A_{\mu}+[A_{\mu},A_{\nu}]$.
2. [[Bianchi Identity|Bianchi identity]]: $\mathrm{d}\mathcal{F}+[\mathcal{A},\mathcal{F}]=0$.
