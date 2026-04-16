---
type: card
updated: 2025-12-06
tags:
  - Area/Physics/ParticlePhysics
---
**Isospin** is a [[Quantum Number|quantum number]] of [[Hadron|hadrons]] referring to the approximated inner global symmetry of [[SU(2)|SU(2)]]. 

The motivation comes from the similar properties of proton and neutron show in masses and scattering process. This observation supports that the one can build a two-dimensional functional space out of the proton and neutron as
$$\begin{pmatrix}
p \\ n
\end{pmatrix},$$
and on which the symmetry transformations are given by $U=\exp(-\mathrm{i}\alpha^{a}\sigma^{a} /2)$ with [[Pauli Matrices|Pauli matrices]] $\sigma^{a}$. The symmetry is further generalized to all hadrons. Since each finite-dimensional representation of $\mathrm{SU}(2)$ is characterized by two number, the so-called **total isospin** $\mathrm{I}$ and **third component of isospin** $\mathrm{I}_{3}$, every hadron is assigned such quantum numbers thus respecting the symmetry. 

Some hadrons form doublets, like nucleons, while others also form triplets, as [[Z Pion|pions]], that can represent either with a three-dimensional vector or a 2x2 traceless [[Z Hermitian Matrix|Hermitian matrix]]
$$\begin{pmatrix}
\pi_{1}\\ \pi_{2} \\ \pi_{3}
\end{pmatrix}\quad\text{or}\quad\begin{pmatrix}
\pi^{+}\\ \pi^{0} \\ \pi^{-}
\end{pmatrix}\quad \text{or}\quad \Pi=\pi_{a}\sigma^{a}=\begin{pmatrix}
\pi^{0}&\sqrt{ 2 }\pi^{+}\\\sqrt{ 2 }\pi^{-}&-\pi^{0}
\end{pmatrix}.$$
Here $\pi_{a},a=1,2,3$ is canonical basis for the three-dimensional representation, and 
$$\pi_{1}=\frac{\pi^{+}+\pi^{-}}{\sqrt{ 2 }},\pi_{2}=\frac{\pi^{+}-\pi^{-}}{\mathrm{i}\sqrt{ 2 }},\pi_{3}=\pi^{0}$$
are the eigenstates of $\mathrm{I}^{3}$. Hadrons that belong to two-dimensional representation have isospin of $\frac{1}{2}$, while hadrons belong to triplet have isospin of $1$. particles with same isospin that have different value of third components have different value charges.


| Multiplet           | $I$    | Members                                        |
| ------------------- | ------ | ---------------------------------------------- |
| Nucleons $(N)$      | $1 /2$ | $p,n$                                          |
| Pions $(\pi)$       | $1$    | $\pi^{+},\pi^{0},\pi^{-}$                      |
| Kaon $(K)$          | $1 /2$ | $(K^{+},K^{0}),(\bar{K}^{0}K^{-})$             |
| Etas $(\eta,\eta')$ | $0$    | $\eta,\eta'$                                   |
| Deltas $(\Delta)$   | $3 /2$ | $\Delta^{++},\Delta^{+},\Delta^{0},\Delta^{-}$ |

## Coupling of isospin
The coupling of isospins is much like the coupling of angular momentums. Theoretically, this relates to the [[Isotypic Decomposition|direct sum decomposition]] of the direct product
$$I_{1}\otimes I_{2}\cong \bigoplus _{I=|I_{1}-I_{2}|}^{I_{1}+I_{2}}I.$$
Given product-basis states $\ket{I_{1},M_{1}}\otimes \ket{I_{2},M_{2}}$ (as charge-mass eigenstates)and coupled states $\ket{I,M}$ (eigenstates of isospin), the change of basis is encoded by  [[Clebsch-Gordan Coefficients|Clebsch-Gordan coefficients]]
$$\ket{I,M}=\sum_{M_{1}+M_{2}=M} C^{I,M}_{I_{1},M_{1};I_{2},M_{2}} \ket{I_{1},M_{1}}\otimes \ket{I_{2},M_{2}}  . $$


## Invariance and breaking of isospin
The isospin is well preserved in [[Strong Interaction|strong interaction]]. Thus the isospin invariance gives strong prediction of scattering through strong interaction from several aspects
1. different particles are connected under isospin transformation, thus the different process. Under the transformation $U=\exp(\mathrm{i}\pi\sigma^{2})$, $p\to n,\pi^{+}\to \pi^{-}$, the elastic process $p+\pi^{+}\to p+\pi^{+}$ becomes $n+\pi^{-}\to n+\pi^{-}$, that should have same [[Cross-section|cross-section]].
2. The elements of [[S Matrix|S matrix]] should only rely on values of total isospin of initial and final states. Typically,  total isospin should be conserved in possible process.

The isospin is broken by [[Z Electromagnetic Interaction|electromagnetic interaction]] and [[Weak Interaction|weak interaction]]. By the way, the strong interaction also causes small breaking effects of isospin symmetry that results in the mass deviation of particles in one multiplet. From the [[Quantum Chromodynamics|QCD]], the isospin is broken by the small deviation of up quark and down quark.

## Generalization of Isospin
Isospin symmetry shows as a global version of the $\mathrm{SU}(2)_{L}$ chiral symmetry from the [[Electroweak Unified Model|electroweak model]], that acts on doublets of left-handed fermions. The very doublet of left-handed up quark and down quark resulting in hadron isospin symmetry.