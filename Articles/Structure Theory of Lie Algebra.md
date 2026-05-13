---
tags:
  - Area/Math/Algebra/LieAlgebra
---
Let $\mathfrak{g}$ be a finite-dimensional [[Lie Algebra|Lie algebra]] over a [[Field (Math)|field]] $\mathbb{K}$, what we take to be either $\mathbb{R}$ or $\mathbb{C}$ through the note otherwise specifically noted. The main question is to decompose $\mathfrak{g}$ into smaller and simpler parts, and how to categorize them.

The answer to the above question, and the main goal we want to state here, is the following theorem:
>[!tip] Levi Theorem
>Every complex Lie algebra can be written as
> $$\mathfrak{g}=\mathrm{rad}(\mathfrak{g}) \oplus \mathfrak{g}_{ss},$$
> where $\mathrm{rad}(\mathfrak{g})$ is the **radical**, and $\mathfrak{g}_{ss}$ is a **[[Simple Lie Algebra|semisimple]] [[Lie Subalgebra|subalgebra]]**. 

The first part of this note is to prove this theorem, which enables us to investigate only the semisimple Lie algebras. 

## Solvable and nilpotent Lie algebras
Like what we do in [[Associative Algebra|associative algebras]], we start with the [[Lie Ideal|ideals]] of Lie algebra.
>[!note] Definition 1 (Lie ideal)
>A **Lie ideal** in Lie algebra $\mathfrak{g}$ is a subalgebra $\mathfrak{h}$ such that $[\mathfrak{g},\mathfrak{h}]\subset \mathfrak{h}$.

With an ideal, we can take the [[Quotient Algebra|quotient]] which has the canonical structure of Lie algebra. In additional we have the following lemma

>[!tip] Lemma 1
>Let $f:\mathfrak{g}_{1}\to \mathfrak{g}_{2}$ be a morphism of Lie algebras. Then $\mathrm{ker}(f)$ is an ideal in $\mathfrak{g}_{1}$, $\mathrm{img}(f)$ is a subalgebra in $\mathfrak{g}_{2}$, and $f$ gives rise to an isomorphism of Lie algebras: $\mathfrak{g} / \mathrm{ker}(f)\cong \mathrm{img}(f)$.
>

Start by the ideals, we now study Lie algebras by analyzing how close the Lie algebra is to a commutative one. That leads to two ways to make it precise. First is the **derived algebra**.

>[!note] Definition 2 (derived algebra)
>The **derived algebra** of $\mathfrak{g}$ is $\mathrm{der}(\mathfrak{g})=[\mathfrak{g},\mathfrak{g}]$.

Clearly it's an ideal. Moreover, the quotient $\mathfrak{g} /\mathrm{der}(\mathfrak{g})$ is abelian, and the derived algebra is the *smallest* ideal with this property. Generalize the idea, we introduce the **derived series** $\mathfrak{g}^{(k)},k\in \mathbb{N}$ defined by
$$\mathfrak{g}^{(0)}=\mathfrak{g},\mathfrak{g}^{(k+1)}=[\mathfrak{g}^{(k)},\mathfrak{g}^{(k)}].$$
Each $\mathfrak{g}^{(k)}$ is an ideal, and $\mathfrak{g}^{(k+1)} /\mathfrak{g}^{(k)}$ is abelian.

>[!note] Definition 3 (solvable Lie algebra)
>A Lie algebra $\mathfrak{g}$ is **solvable** iff $\mathfrak{g}^{(n)}=0$ for some $n\in \mathbb{N}$.

Informally, solvable Lie algebra is an "almost commutative algebra": it is an algebra that can be obtained by successive extensions of commutative algebras. Another way is to introduce the **lower central series** $\mathfrak{g}_{(k)},k\in \mathbb{N}$ as
$$\mathfrak{g}_{(0)}=\mathfrak{g},\mathfrak{g}_{(k+1)}=[\mathfrak{g},\mathfrak{g}_{(k)}].$$

>[!note] Definition 4 (nilpotent Lie algebra)
>A Lie algebra $\mathfrak{g}$ is **nilpotent** iff $\mathfrak{g}_{(n)}=0$ for some $n\in \mathbb{N}$.

Let's summarize some properties of solvable and nilpotent algebras:

>[!tip] Theorem 2
>1. A real Lie algebra $\mathfrak{g}$ is solvable (nilpotent) if its complexification $\mathfrak{g}_{\mathbb{C}}=\mathfrak{g}\otimes \mathbb{C}$ is solvable (nilpotent).
>2. If $\mathfrak{g}$ is solvable (nilpotent), then any subalgebra and quotient of $\mathfrak{g}$ is solvable (nilpotent).
>3. If $\mathfrak{g}$ is nilpotent, then $\mathfrak{g}$ is solvable.
>4. If $\mathfrak{i}\subset \mathfrak{g}$ is an ideal such that $\mathfrak{i},\mathfrak{g} /\mathfrak{i}$ is solvable, then $\mathfrak{g}$ is solvable.

## Semisimple Lie algebras and radical
Above we have analyzed Lie algebra by how close it is to a commutative algebra. Now we will describe the opposite case, Lie algebras that are as far as possible from being abelian.

>[!note] Definition 5 (semisimple Lie algebra)
>A Lie algebra is semisimple if it contains no nonzero solvable ideals.

>[!note] Definition 6 (simple Lie algebra)
>A Lie algebra is simple if it's not abelian and contains no ideals other than $0$ and itself.

>[!tip] Lemma 2
>Any simple Lie algebra is semisimple.

These two definitions are according to the idea of "as far as possible from abelian". Based on semisimple and solvable Lie algebra, we can try to decompose general Lie algebra that is neither solvable nor semisimple. Let's introduce the radical:

>[!note] Definition 7 (radical)
>The radical $\mathrm{rad}(\mathfrak{g})$ of a Lie algebra $\mathfrak{g}$ is the solvable ideal which contains any other solvable ideal.

The radical is obviously unique. One can take the finite sum over all solvable ideals to extract the radical, thus there always exists a radical.

With these preparation, we can state the Levi theorem.  