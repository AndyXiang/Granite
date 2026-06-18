---
tags:
  - Area/Math/Geometry/Manifold/ComplexManifold
---
Let $M$ be a [[Differential Manifold|differential manifold]]. It's called an **almost complex manifold** iff there exists a [[Tangent Bundle|tensor field]] $J:TM\to TM$ such that
$$J^{2}=-\mathrm{id}.$$
$J$ is called a **almost complex structure**.

## Properties
1. $J$ only exists for even dimension.
2. Define the **Nijenhuis tensor** $N:\mathfrak{X}(M)\times \mathfrak{X}(M)\to \mathfrak{X}(M)$ by $$N(X,Y)=[X,Y]+J([J(X),Y])+J([X,J(Y)])-[J(X),J(Y)].$$ $J$ is **integrable** iff $N$ vanishes. 

>[!note] Theorem
>The manifold $M$ with almost complex structure $J$ is a [[Complex Manifold|complex manifold]] iff $J$ is integrable.

3. The complexified [[Tangent Bundle|tangent bundle]] $T_{\mathbb{C}}M=TM\otimes_{\mathbb{R}}\mathbb{C}$ admits the decomposition $$T_{\mathbb{C}}M=T_{+}M\oplus T_{-}M$$ where $T_{\pm}M=(1\pm\mathrm{i}J)(T_{\mathbb{C}}M)$.