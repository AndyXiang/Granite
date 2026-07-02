---
tags:
  - Area/Math/Geometry/Manifold/DifferentialManifold
  - Area/Math/Topology/Cohomology
---
Let $M$ be a [[Differential Manifold|manifold]], and consider the [[Exterior Differential Form|differential forms]] $\omega\in\Omega^{r}(M)$ on it. The [[Set|set]] of [[Exterior Differential Form#Related|closed r-forms]] is called the $r$th **cocycle [[Group|group]]** $Z^{r}(M)=\mathrm{ker}(\mathrm{d}|_{\Omega^{r}(M)})$. The set of [[Exterior Differential Form#Related|exact r-forms]] is called the $r$th **coboundary group** $B^{r}(M)=\mathrm{im}(\mathrm{d}|_{\Omega^{r-1}(M)})$. It follows from $\mathrm{d}^{2}=0$ that $Z^{r}(M) \supset B^{r}(M)$. There is a [[Chain Complex & Cochain complex|cochain complex]]
$$0\to \Omega^{0}(M)\xrightarrow{~d~} \Omega^{1}(M)\xrightarrow{~d~} \cdots \xrightarrow{~d~} \Omega^{n}(M)\to0$$

The $r$th **de Rham cohomology group** is defined by
$$H^{r}(M)=Z^{r}(M) /B^{r}(M).$$

## de Rham Theorem
As the name suggests, the cohomology group $H^{r}(M)$ is the [[Dual Space|dual space]] of the [[Simplicial Homology|homology group]] $H_{r}(M)$. First one has a bilinear [[Map|map]]
$$(,): \begin{matrix}
C_{r}(M)\times\Omega^{r}(M) &\to & \mathbb{R} \\
(c,\omega)&\mapsto&\int_{c}\omega
\end{matrix}$$
This induces a dual
$$\Lambda:\begin{matrix}
H_{r}(M)\times H^{r}(M) &\to &\mathbb{R} \\
([c],[\omega]) & \mapsto & (c,\omega)=\int_{c}\omega.
\end{matrix}$$

>[!tip] de Rham's theorem
>If $M$ is a [[Compact Space|compact]] manifold, $H_{r}(M)$ and $H^{r}(M)$ are finite-dimensional, and $\Lambda:H_{r}(M)\times H^{r}(M)\to \mathbb{R}$ is bilinear and non-degenerate.