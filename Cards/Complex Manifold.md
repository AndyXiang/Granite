---
tags:
  - Area/Math/Geometry/Manifold/ComplexManifold
---
A [[Topological Space|topological space]] $M$ is called a **complex manifold** if followings hold:
1. $M$ is provided with a family of charts $\{ (U_{i},\varphi_{i}) \}$ such that $\{ U_{i} \}$ [[Covering Space|covers]] $M$, and $\varphi_{i}$ is [[Homeomorphism|homeomorphism]] that maps $U_{i}$ to a [[Topological Space|open set]] of $\mathbb{C}^{m}$.
2. Given $U_{i}$ and $U_{j}$ such that $U_{i}\cap U_{j}\neq \varnothing$, the map $\psi_{ij}=\varphi_{j}\circ\varphi_{i}^{-1}$ is [[Holomorphic Function|holomorphic]].

For complex coordinates $z^{\mu}=x^{\mu}+\mathrm{i}y^{\mu},\mu=1,2,\cdots,m$ of $\mathbb{C}^{m}$, the according coordinates for complex manifold $M$ can be 
1. ordinary coordinates $\{ (x^{\mu},y^{\mu}),\mu=1,2,\cdots,m \}$.
2. holomorphic coordinates $\{ (z^{\mu},\bar{z}^{\mu}),\mu=1,2,\cdots,m \}$.

## Tangent structures
Let $\mathfrak{F}(M)$ be the set of functions $f:M\to \mathbb{C}$ on $M$. One also defines the [[Tangent bundle|tangent bundle]] on a complex manifold. There exists a global [[Almost Complex Manifold|almost complex structure]] $J$ on $M$, expressed by
$$J=\mathrm{i}(\mathrm{d}z^{\mu}\otimes \partial _{\mu}-\mathrm{d}\bar{z}^{\mu}\otimes  \bar{\partial} _{\mu})$$
in holomorphic coordinates on some chart.

Thus is a decomposition of tangent bundles:
$$T_{\mathbb{C}}M=T_{+}M\oplus T_{-}M$$
with 
$$T_{\pm}^{(r,s)}=\left( \frac{1\mp \mathrm{i}J}{2} \right)T_{\mathbb{C}}^{(r,s)}M.$$
There is similar result for [[Tangent Bundle|cotangent bundle]] $T^{*}_{\mathbb{C}}(M)$.

### Differential forms
Due to the holomorphic decomposition, there are two parallel [[Filtration|filtration]] on the space of [[Exterior Differential Form|differential forms]]. A general differential form is written as
$$\omega=\frac{1}{r!s!} \omega_{\mu_{1}\cdots \mu_{r}\nu_{1}\cdots\nu_{s}} \mathrm{d}z^{\mu_{1}}\wedge \cdots \wedge \mathrm{d}z^{\mu_{r}} \wedge \mathrm{d}\bar{z}^{\nu_{1}}\wedge \cdots \wedge \mathrm{d}\bar{z}^{\nu_{s}}.$$
We denote the set of this differential form by $\Omega^{(r,s)}M$. The indices $(r,s)$ are called *bidegree*. We have following operations:
1. exterior product: $\wedge:\Omega^{(r,s)}M\times\Omega^{(p,q)}M\to\Omega^{(r+p,s+q)}M$.
2. exterior derivative: $\partial:\Omega^{(r,s)}M\to\Omega^{(r+1,s)}M,\bar{\partial}:\Omega^{(r,s)}M\to\Omega^{(r,s+1)}M$.
3. conjugation: $\bar{}:\Omega^{(r,s)}M\to\Omega^{(s,r)}M$.

They satisfy:
$$\overline{\eta \wedge \xi}=\bar{\eta}\wedge \xi+\eta \wedge \bar{\xi},\overline{\partial \omega}=\bar{\partial}\bar{\omega}, \partial \bar{\omega}=\overline{\bar{\partial}\omega}.$$

The space of complex differential $q$-forms admits the decomposition
$$\Omega_{\mathbb{C}}^{q}M=\bigoplus _{r+s=q} \Omega^{(r,s)}M.$$
The exterior derivative over $\Omega^{q}_{\mathbb{C}}M$ is $\mathrm{d}=\partial+\bar{\partial}$. 




One easily sees that there are two parallel [[Chain Complex & Cochain complex|cochain complexes]] for a given $q$:
```tikz
\usepackage{tikz-cd}
\begin{document}
	\begin{tikzcd}
		0 \ar[r] & \Omega^{(0,q)}M \ar[r, "\partial"] \ar[d, "\mathrm{conj}", leftrightarrow] & \Omega^{(1,q)}M \ar[d, "\mathrm{conj}", leftrightarrow]\ar[r, "\partial"] & \cdots \ar[r, "\partial"] & \Omega^{(m,q)}M\ar[d, "\mathrm{conj}", leftrightarrow]\ar[r] & 0 \\
		0 \ar[r] & \Omega^{(q,0)}M \ar[r, "\bar{\partial}"] & \Omega^{(q,1)}M \ar[r, "\bar{\partial}"] & \cdots \ar[r, "\bar{\partial}"] & \Omega^{(q,m)}M\ar[r] & 0 
	\end{tikzcd}
\end{document}
```
Thus there are two types of [[de Rham Cohomology Group|cohomology groups]] 
$$H^{(r,s)}(M)= \frac{\mathrm{ker}\left( \partial:{\Omega^{(r,s)}M\to\Omega^{(r+1,s)M}}  \right)}{\mathrm{im}\left( \partial :{\Omega^{(r-1,s)}M\to\Omega^{(r,s)}M}  \right)},\bar{H}^{(r,s)}(M)=\frac{\mathrm{ker}\left( \bar{\partial}:{\Omega^{(r,s)}M\to\Omega^{(r,s+1)M}}  \right)}{\mathrm{im}\left( \bar{\partial} :{\Omega^{(r,s-1)}M\to\Omega^{(r,s)}M}  \right)}.$$
satisfying $H^{(r,s)}(M)\cong\overline{\bar{H}^{(r,s)}(M)}$ as complex [[Vector Space|vector spaces]]. There also is a [[de Rham Cohomology Group|de Rham cohomology groups]]
$$H_{\mathrm{dR}}^{q}(M)= \frac{\mathrm{ker}(\mathrm{d}:\Omega^{q}_{\mathbb{C}}M\to\Omega^{q+1}_{\mathbb{C}}M)}{\mathrm{im}(\mathrm{d}:\Omega_{\mathbb{C}}^{q-1}M\to\Omega_{\mathbb{C}}^{q}M)}.$$


