---
tags:
  - Area/Physics/FieldTheory/QuantumFieldTheory
  - Area/Physics/QuantumTheory/PathIntegral
---
The **generating functional** is a [[Functional|functional]] of external source $J(x)$, and is defined as
$$Z[J]=\int \mathcal{D}\phi \exp\left[ \mathrm{i}\int \mathrm{d}^{4}x(\mathcal{L}+J(x)\phi(x)) \right].$$
This is the generating functional for [[Correlation Function|correlation function]] 
$$\braket{ \Omega | \mathrm{T}[\phi (x_{1})\cdots\phi(x_{n})]|\Omega }=\frac{1}{Z[0]} \left[ \prod_{i=1}^{n} \frac{1}{\mathrm{i}}\frac{\delta}{\delta J(x_{i})}Z[J] \right]_{J=0} .$$


## Generating functional of free field
For most cases, the generating functionals of free fields can be computed directly by Gaussian integral:
$$Z[J]=\int \mathcal{D}\phi \exp\left[ \mathrm{i}\left( \frac{1}{2}\int \mathrm{d}^{d}x\mathrm{d}^{d}y~\phi(x)\Delta(x,y) \phi(y)+\int \mathrm{d}^{d}xJ(x)\phi(x) \right) \right]=Z[0] \exp\left[-\frac{1}{2}\int \mathrm{d}^{d}x \mathrm{d}^{d}y J(x)D(x,y)J(y)\right]$$where $D$ is inverse of $\Delta$ that is defined by
$$\int \mathrm{d}^{d}z\Delta(x,z)D(z,y)=\mathrm{i}\delta^{(d)}(x-y).$$

### Scalar field
Consider the generating functional of free [[Scalar Field|scalar field]]:
$$Z[J]=\int \mathcal{D}\phi \exp\left\{ \mathrm{i}\int \mathrm{d}^{d}x\left[ -\frac{1}{2}\phi( \partial^{2}+m^{2})\phi+J\phi \right] \right\}.$$
Now $\Delta(x,y)=-(\partial^{2}+m^{2})\delta^{(d)}(x-y)$. The inverse is
$$D_{F}(x-y)=\int \frac{\mathrm{d}^{d}p}{(2\pi)^{d}} \frac{\mathrm{i}\mathrm{e}^{ -\mathrm{i}p\cdot (x-y) }}{p^{2}-m^{2}+\mathrm{i}\epsilon}$$
where $\epsilon\to 0$ is added to make the integral converge. One has
$$Z[J]=Z[0]\exp\left[ -\frac{1}{2}\int \mathrm{d}^{d}x \mathrm{d}^{d}y J(x)D(x,y)J(y)  \right]$$

For complex field, the generating functional is 
$$Z[J,J^{\dagger}]=\int \mathcal{D}\phi \mathcal{D}\phi ^{\dagger} \exp\left\{ \mathrm{i}\int \mathrm{d}^{d}x\Big[\phi ^{\dagger}(\partial^{2}+m^{2}+\mathrm{i}\epsilon)\phi+J^{\dagger}\phi+J\phi ^{\dagger}\Big] \right\}.$$
Similarly one can derive the Gaussian form
$$Z[J,J^{\dagger}]=Z[0] \exp\left[ -\int \mathrm{d}^{d}x\mathrm{d}^{d}y J^{\dagger}(x) D_{F}(x-y)J(y) \right].$$

### Spinor field
Spinor field is expressed with [[Grassmann Calculus|Grassmann number]] in path integral formalism. The generating functional is
$$Z[\bar{\eta},\eta]=\int \mathcal{D}\bar{\psi}\mathcal{D}\psi \exp \left\{  \mathrm{i}\int \mathrm{d}^{4}x \Big[\bar{\psi}(\mathrm{i}\partial \!\!\!/-m+\mathrm{i}\epsilon)\psi+\bar{\psi}\eta+\bar{\eta}\psi\Big]  \right\}$$
with Grassmannian sources $\bar{\eta},\eta$. By making use of the [[Grassmann Calculus#Path integral|Grassmann Gaussian integral]] , the generating functional is cast into the form
$$Z[\bar{\eta},\eta]=Z[0]\exp\left[ -\int \mathrm{d^{d}}x\mathrm{d}^{d}y \bar{\eta}(x)S(x-y)\eta(y) \right]$$
with the Feynman propagator for spinor field
$$S(x-y)=\int \frac{\mathrm{d}^{d}k}{(2\pi)^{d}} \frac{\mathrm{i}(k\!\!\!/+m)}{k^{2}-m^{2}+\mathrm{i}\epsilon}\mathrm{e}^{ -\mathrm{i}k\cdot (x-y) }.$$

### Gauge field
Now consider a [[Construct field theory with gauge symmetry|gauge field theory]] with
$$Z[J]=\int \mathcal{D}A \exp\left\{ \mathrm{i}\int \mathrm{d}^{d}x\left[ -\frac{1}{2}\mathrm{tr}(F_{\mu \nu}F^{\mu \nu})+J_{\mu}^{a}A_{a}^{\mu} \right] \right\}.$$
There comes the problem of **gauge-fixing**. The integral tends to explodes because we include many unphysical field configuration in the measure $\mathcal{D}A$, that should be excluded by choosing a gauge. For details, see [[Faddeev-Popov Method]].

