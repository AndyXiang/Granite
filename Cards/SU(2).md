---
tags:
  - Area/Math/Algebra/Group/LieGroup
---
The [[Unitary Group|special unitary group]] of degree $2$.

## Parameterizations
1. Exponential map: choose a basis for its [[Lie Algebra|Lie algebra]], usually one use [[Pauli Matrices|Pauli matrices]] $\sigma_{i}$, then $u=\exp(-\mathrm{i}\omega_{i}\sigma_{i}),\omega_{i}\in$.
2. axis-angle: pick an unit axis $\hat{n}\in \mathrm{S}^{2}$ and an angle $\omega\in[0,2\pi]$, then 
$$u=\exp\left( -\frac{\mathrm{i}\omega}{2}\hat{n}\cdot\sigma\right)=\cos \frac{\omega}{2}1_{2\times2}-\mathrm{i}\sin\frac{\omega}{2}(\hat{n}\cdot\sigma),$$
where
$$\hat{n}=(\sin\theta \cos \phi,\sin\theta \sin \phi,\cos\theta),\theta\in[0,\pi],\phi\in[0,2\pi].$$
At the 
3. Euler-angle: similar to [[SO(3)|SO(3)]]:
$$u(\alpha,\beta,\gamma)=u(\mathbf{e}_{3},\alpha)u(\mathbf{e}_{2},\beta)u(\mathbf{e}_{3},\gamma),a\in[-\pi,\pi],\beta\in[0,\pi],\gamma\in[-2\pi,2\pi].$$

## Lie algebra
The [[Lie Algebra|Lie algebra]] of $\mathrm{SU}(2)$ is $\mathfrak{su}(2)$. Usually we use [[Pauli Matrices|Pauli matrices]] for its generators:
$$[t_{i},t_{j}]=\mathrm{i}\epsilon_{ijk}t_{k},t_{i}= \frac{\sigma_{i}}{2}.$$
The [[Killing Form|Killing form]] is
$$K=-2\begin{pmatrix}
1 & 0 & 0 \\ 0 & 1 & 0 \\0 & 0 & 1
\end{pmatrix}.$$

## Haar measure
Since the unitary groups are [[Compact Space|compact]], their [[Haar Measure|Haar measure]] is unimodular. Use the axis-angle parameterization:
$$u=\cos \frac{\omega}{2}1_{2\times2}-\mathrm{i}\sin \frac{\omega}{2}(\mathbf{n}\cdot\sigma),$$
where $|\mathbf{n}|^{2}=1$. This is a [[Submanifold|embedding]] $\mathrm{SU}(2)\cong \mathbb{S}^{3}\hookrightarrow \mathbb{R}^{4}$ as
$$(\omega,\mathbf{n})\mapsto(a_{0},\mathbf{a})=\left( \cos \frac{\omega}{2},-\sin \frac{\omega}{2}\mathbf{n} \right).$$
The induced [[Riemannian Metric|metric]] of $\mathbb{S}^{3}$ is
$$\begin{align}
\mathrm{d}s^{2}&=\mathrm{d}a_{0}^{2}+||\mathrm{d}\mathbf{a}||^{2} \\
&=\frac{1}{4}\sin ^{2} \frac{\omega}{2}\mathrm{d\omega^{2}}+\left\lVert-\frac{1}{2}\cos \frac{\omega}{2}\mathbf{n}\mathrm{d\omega} -\sin \frac{\omega}{2}\mathrm{d}\mathbf{n}\right\rVert ^{2}\\
&=\frac{1}{4}\mathrm{d}\omega^{2}+\sin ^{2} \frac{\omega}{2}||\mathrm{d}\mathbf{n}||^{2} \\
&=\frac{1}{4}\mathrm{d}\omega^{2}+\sin ^{2} \frac{\omega}{2}(\mathrm{d\theta^{2}}+\sin ^{2}\theta\mathrm{d}\phi^{2}). 
\end{align}$$
Thus the [[Volume Form|volume]] is
$$\mathrm{d}\mu=\sqrt{ \det(g) }\mathrm{d}\omega \wedge \mathrm{d}\theta \wedge \mathrm{d}\phi=\frac{1}{2}\sin ^{2} \frac{\omega}{2}\sin\theta\mathrm{d}\omega \wedge \mathrm{d}\theta \wedge \mathrm{d}\phi.$$
Now normalize it to obtain the Haar measure
$$\begin{align}
\int \mathrm{d}\mu&=\frac{1}{2}\int_{0}^{2\pi}\sin ^{2} \frac{\omega}{2}\mathrm{d}\omega \int_{0}^{\pi}\sin\theta \mathrm{d\theta}\int_{0}^{2\pi}\mathrm{d}\phi=2\pi^{2} \\
\implies \mathrm{d}\mu_{\mathrm{H}}&=\frac{1}{4\pi^{2}}\sin ^{2} \frac{\omega}{2}\sin\theta\mathrm{d}\omega \wedge \mathrm{d}\theta \wedge \mathrm{d}\phi
\end{align}$$

