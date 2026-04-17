---
type: card
updated: 2026-01-28
tags:
  - Area/Physics/FieldTheory/QuantumFieldTheory
---
The **Lehmann-Symanzik-Zimmermann reduction formula** shows the relation between [[S Matrix|S matrix]] and [[Correlation Function|correlation functions]].

For field satisfying following normalizations:
$$\braket{ \Omega |\phi|\Omega  }=0, \braket{ \Omega | \phi(x)|k }=\mathrm{e}^{ -\mathrm{i}k\cdot x }. $$
the LSZ reduction formula is
$$\braket{ p_{1}\cdots p_{n};\mathrm{out} |q_{1}\cdots q_{m};\mathrm{in}  }=\mathrm{i}^{n+m}\prod_{i=1}^{n}\int \mathrm{d}^{4}x_{i} \mathrm{e}^{ \mathrm{i}p_{i}\cdot x_{i} }(\partial _{i}^{2}+m^{2})\prod_{j=1}^{m}\int \mathrm{d}^{4}y_{j} \mathrm{e}^{ -\mathrm{i}q_{j}\cdot y_{j} }(\partial _{j}^{2}+m^{2}) \braket{ \Omega |\mathsf{T}[\phi(x_{1})\cdots \phi(x_{n})\phi(y_{1})\cdots \phi(y_{m})]|\Omega  }.$$

The LSZ reduction formula for fields with higher spin are mush similar, with according polarization vectors added.

## Proof
For simplicity we only prove the formula for scalars. The proofs of other fields are much similar. Let $\ket{\Omega}$ be vacuum, $\phi(x)$ be field operator satisfying normalization as
$$\braket{ \Omega |\phi|\Omega  }=0, \braket{ \Omega | \phi(x)|k }=\mathrm{e}^{ -\mathrm{i}k\cdot x }. $$
Asymptotic states and associated annihilation/creation operators are needed for building a [[Scattering Theory|scattering theory]]. Working in [[Heisenberg Picture|Heisenberg picture]], we have relations:
$$a(p,t)\ket{\Omega}=0, a(p,t)^{\dagger}\ket{\Omega}=\ket{\mathbf{p}},  a_{\mathrm{in}}(p)=\lim_{t\to-\infty}a(p,t),a_{\mathrm{out}}(p)=\lim_{t\to \infty}a(p,t)$$
and
$$a^{\dagger}_{\mathrm{in}}(p)\ket{\Omega} =\ket{p;\mathrm{in}},a^{\dagger}_{\mathrm{out}}(p)\ket{\Omega} =\ket{p;\mathrm{out}}.  $$
The S matrix element is defined as
$$\braket{ p_{1}\cdots p_{n} |\mathcal{S}|q_{1}\cdots q_{m}  } =\braket{ p_{1}\cdots p_{n};\mathrm{out} |q_{1}\cdots q_{m};\mathrm{in}  }. $$
Use the [[Scalar Field#Free field|mode expansion]] of scalar to rewrite these operators:
$$a_{\mathrm{in}}(p)=\lim_{t\to-\infty}\mathrm{i}\int \mathrm{d}^{3}x\mathrm{e}^{ \mathrm{i}p\cdot x } \overset{ \leftrightarrow  }{ \partial_{0} }\phi(x),$$
$$a_{\mathrm{out}}(p)=\lim_{t\to\infty}\mathrm{i}\int \mathrm{d}^{3}x\mathrm{e}^{ \mathrm{i}p\cdot x } \overset{ \leftrightarrow  }{ \partial_{0} }\phi(x),$$
where $f \overset{\leftrightarrow}{\partial} g=f(\partial g)-(\partial f)g$. A key formula is
$$\begin{align}
a_{\mathrm{out}}(p)-a_{\mathrm{in}}(p)&=\int_{-\infty}^{\infty}\mathrm{d}t \frac{\mathrm{d}}{\mathrm{d}t}\left( \mathrm{i}\int \mathrm{d}^{3}x \mathrm{e}^{ \mathrm{i}p\cdot x }\overset{ \leftrightarrow  }{ \partial_{0} }\phi(x)\right) \\
&=\mathrm{i}\int \mathrm{d}^{4}x\mathrm{e}^{ \mathrm{i}p\cdot x }(\partial^{2}+m^{2})\phi(x). \\
a_{\mathrm{out}}(p)^{\dagger}-a_{\mathrm{in}}(p)^{\dagger}&=-\mathrm{i}\int \mathrm{d}^{4}x\mathrm{e}^{ -\mathrm{i}p\cdot x }(\partial^{2}+m^{2})\phi(x).
\end{align}$$
Now, use this formula, we can "move" an annihilation operator from outgoing state into incoming state, or an creation operator from incoming state into outgoing state. For example:
$$\begin{align}
\braket{ \beta;\mathrm{out} |p,\alpha;\mathrm{in}  }&=\braket{ \beta;\mathrm{out} |a_{\mathrm{in}}(p)^{\dagger}|\alpha;\mathrm{in}  }=\braket{ \beta;\mathrm{out} |(a_{\mathrm{in}}(p)^{\dagger}-a_{\mathrm{out}}(p)^{\dagger}+a_{\mathrm{out}}(p)^{\dagger})|\alpha;\mathrm{in}  }   \\
&=\braket{ \beta;\mathrm{out} |a_{\mathrm{out}}(p)^{\dagger}|\alpha;\mathrm{in}  }+\mathrm{i}\int \mathrm{d}^{4}x\mathrm{e}^{ -\mathrm{i}p\cdot x }(\partial^{2}+m^{2})\braket{ \beta;\mathrm{out} |\phi(x)|\alpha;\mathrm{in}  }. 
\end{align}$$
The first term is an contact term, vanishes when no particle has momentum $p$ in $\beta$ (including other [[Quantum Number|quantum number]]), which will be omitted. When multiple "moving" is occurred, an time-ordering operator is needed. So the finally expression is
$$\begin{align}
\braket{ p_{1}\cdots p_{n};\mathrm{out} |q_{1}\cdots q_{m};\mathrm{in}  }&=\mathrm{i}^{n+m}\prod_{i=1}^{n}\int \mathrm{d}^{4}x_{i} \mathrm{e}^{ \mathrm{i}p_{i}\cdot x_{i} }(\partial _{i}^{2}+m^{2})\prod_{j=1}^{m}\int \mathrm{d}^{4}y_{j} \mathrm{e}^{ -\mathrm{i}q_{j}\cdot y_{j} }(\partial _{j}^{2}+m^{2}) \braket{ \Omega |\mathsf{T}[\phi(x_{1})\cdots \phi(x_{n})\phi(y_{1})\cdots \phi(y_{m})]|\Omega  }. 
\end{align}$$



