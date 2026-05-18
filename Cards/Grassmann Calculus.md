---
tags:
  - Area/Math/Algebra/AssociativeAlgebra/ExteriorAlgebra
  - Area/Math/Calculus
---
Let $V$ be a [[Vector Space|vector space]] over [[Field (Math)|field]] $\mathbb{K}$, and $\bigwedge V$ be the [[Exterior Algebra|exterior algebra]]. Here covers the differentiation and integral of functions of Grassmann numbers. For simplicity, take $\mathbb{K}=\mathbb{C}$.

For functions as $f:\bigwedge V\to \bigwedge V$, it's defined by [[Taylor Expansion|Taylor expansion]]
$$f(\theta)=\sum_{k=0}^{\infty}f_{k} \theta^{k},$$
where $\theta^{0}=1\in \mathbb{C}$ and $f_{k}\in \mathbb{C}$. Since Grassmann numbers are anti-commuting, so $\theta^{2}=0$. This implies
$$f(\theta)=a+b\theta,a,b\in \mathbb{C}.$$
For multi-variable functions, one has
$$f(\theta_{1},\theta_{2},\cdots,\theta_{r})=a+\sum_{k=1}^{r} \sum_{i_{1},i_{2},\cdots,i_{k}=1}^{r} \frac{1}{k!} f_{i_{1}\cdots i_{k}}\theta_{i_{1}}\theta_{i_{2}} \cdots \theta_{i_{k}},$$
as $f_{i_{1}\cdots i_{k}}$ is fully anti-symmetric.

## Derivatives
Since Grassmann numbers are anti-commuting, so are their derivatives. A **left Grassmann derivative** is
$$\frac{\partial }{\partial \theta_{i}}\theta_{j}=\delta_{ij}$$
and anti-commutes with other variables and derivatives. It's nilpotent
$$\left( \frac{\partial }{\partial \theta_{i}} \right)^{2}f(\theta)=0.$$
The **right derivatives** are defined similarly, but it acts on the functions from the right.

## Integral
The integral for single-variable Grassmann function is the linear functional
$$\int \mathrm{d}\theta[af(\theta)+bg(\theta)]=a\int \mathrm{d}\theta f(\theta)+b\int \mathrm{d}\theta g(\theta),a,b\in \mathbb{C},$$
where
$$\int \mathrm{d}\theta~1=0,\int \mathrm{d}\theta\theta=1.$$

Generalized to multi-variable cases, one has
$$\int \mathrm{d}\theta f(\theta)=\int \mathrm{d}\theta_{r}\mathrm{d\theta}_{r-1}\cdots \mathrm{d}\theta_{1}\left( a+\sum_{k=1}^{r} \sum_{i_{1},i_{2},\cdots,i_{k}=1}^{r} \frac{1}{k!} f_{i_{1}\cdots i_{k}}\theta_{i_{1}}\theta_{i_{2}} \cdots \theta_{i_{k}}  \right)=f_{12\cdots r}.$$

### Change of variables
$\theta_{i}=A_{ij}\eta_{j}$ then
$$\mathrm{d}\theta=(\det A)^{-1}\mathrm{d}\eta.$$

### Path integral
$$\int \prod_{i}\mathcal{D}\bar{\psi}_{i} \mathcal{D}\psi_{i} \exp(-\bar{\psi}_{i}A_{ij}\psi_{j})=\det A.$$