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

With these preparation, we can state the Levi theorem in the very first of this note.

## Cartan subalgebra and root decomposition
Our final goal is to illustrate the equivalence of the [[Category|category]] of semisimple Lie algebra and the category of [[Root Space|reduced root space]]. By this, we fully classified the complex semisimple Lie algebras by classification of root spaces. See [[Root Space and Simple Roots]] for detail on classification of root spaces. The first tool we need is the [[Killing Form|Killing form]] 
$$K:\begin{matrix}
\mathfrak{g}\times \mathfrak{g} & \to & \mathbb{C} \\
(x,y)& \mapsto & \mathrm{tr}(\mathfrak{ad}(x)\mathfrak{ad}(y))
\end{matrix}$$
For a semisimple Lie algebra $\mathfrak{g}$, the Killing form is non-degenerate, thus one can lift it to a [[Metric Space|metric]] on $\mathfrak{g}$. Then $\mathfrak{g}$ is a metric space as well as a [[Inner Product Space|inner product space]].

The [[Adjoint Action|adjoint action]] $\mathfrak{ad}:\mathfrak{g}\to \mathrm{aut}(\mathfrak{g})$ transforms the Lie algebra into a set of [[Linear Transformation|linear transformations]] on $\mathfrak{g}$. To investigate the Lie algebra, we can also investigate this linear transformations.

We call an element $x\in \mathfrak{g}$ **semisimple** if $\mathfrak{ad}(x)$ is diagonalizable. A [[Lie Subalgebra|subalgebra]] $\mathfrak{h}$ is called **toral** if it's commutative and consists of semisimple elements. Then the operators in toral algebra can be simultaneously diagonalized. This leads to a decomposition of $\mathfrak{g}$ as $\mathfrak{g}=\bigoplus_{\alpha\in \mathfrak{h}^{*}}\mathfrak{g}_{\alpha}$, where $\mathfrak{g}_{\alpha}$ is the common eigenspace for all operators $\mathfrak{ad}(h),h\in \mathfrak{h}$ with eigenvalue $\alpha$:
$$\mathfrak{ad}(h)(x)=\alpha(h)x.$$
In particular, $\mathfrak{h}\subset \mathfrak{g}_{0}$. These eigenspaces are graded: $[\mathfrak{g}_{\alpha},\mathfrak{g}_{\beta}]\subset \mathfrak{g}_{\alpha+\beta}$. Finally, using the Killing form, one finds:
1. If $\alpha+\beta\neq 0$, then $K(\mathfrak{g}_{\alpha},\mathfrak{g}_{\beta})=0$.
2. If $\alpha+\beta =0$, then $K$ gives a non-degenerate pairing $\mathfrak{g}_{\alpha}\otimes \mathfrak{g}_{-\alpha}\to \mathbb{C}$. Particularly, $K$ restricted to $\mathfrak{h}$ is non-degenerate.

Now we sees the toral algebra gives a clear decomposition of the semisimple Lie algebra. Based on that, we now give the [[Cartan Subalgebra|Cartan subalgebra]] as the largest toral subalgebra. Formally, the Cartan subalgebra is the toral subalgebra $\mathfrak{h}\subset \mathfrak{g}$ which coincides with its [[Center|centralizer]]:
$$\mathfrak{h}=C(\mathfrak{h})=\{ x:[x,\mathfrak{h}]=0 \}.$$
This definition is only suitable for semisimple Lie algebra over [[Algebraically Closed Field|algebraically closed field]]. 

Since the restriction of Killing form to $\mathfrak{h}$ is non-degenerate, it defines an isomorphism $h \cong h^{*}$, and a map $K:\mathfrak{h}^{*}\times \mathfrak{h}^{*}\to \mathbb{C}$. Let's denote for $\alpha\in \mathfrak{h}^{*}$ by $H_{\alpha}$ as
$$K(H_{\alpha},h)=\alpha(h).$$
Define $h_{\alpha}=2H_{\alpha} /K(\alpha,\alpha).$

The main theorem for the structure of semisimple Lie algebra is 
>[!tip] Theorem 1
>1. $R$ spans $\mathfrak{h}^{*}$ as a [[Vector Space|vector space]], and $\{ h_{\alpha},\alpha\in R \}$ spans $\mathfrak{h}$ as a vector space.
>2. The *root subspace* $\mathfrak{g}_{\alpha}=\{ x:[h,x]=\alpha(h)x,\forall h\in \mathfrak{h} \}$ is one-dimensional.
>3. For any two roots $\alpha,\beta\in R$, the number $$2K(\alpha,\beta) /K(\alpha,\alpha)$$ is integer.
>4. For any root $\alpha\in R$, define the reflection operator $s_{\alpha}:\mathfrak{h}^{*}\to \mathfrak{h}^{*}$ by $$s_{\alpha}(\lambda)=\lambda-\lambda(h_{\alpha}) \alpha.$$ Then $s_{\alpha}(\beta)$ is also a root.
>5. For any root $\alpha$, the only multiples of $\alpha$ which are also roots are $\pm \alpha$.
>6. If $\alpha,\beta$ are roots such that $\alpha+\beta$ is also a root, then $[\mathfrak{g}_{\alpha},\mathfrak{g}_{\beta}]=\mathfrak{g}_{\alpha +\beta}$.

This shows that $R$ is a [[Root Space|root space]] of $\mathfrak{h}^{*}$. By this, every complex semisimple Lie algebra uniquely defines a reducible root space, and simple Lie algebra defines a irreducible root space. The next question is that, whether can we recover the Lie algebra from a root space. The answer is by the following theorem:
>[!tip] Theorem 2
>Let $R$ be a root space with simple roots $\Pi=\{ \alpha_{1},\cdots,\alpha_{r} \}$. Let $$a_{ij}=2K(\alpha_{i},\alpha_{j}) /K(\alpha_{i},\alpha_{i}).$$ Then $R$ gives a Lie algebra $\mathfrak{g}(R)$ with generators $e_{i},f_{i},h_{i},i=1,\cdots, r$ and 
> $$[h_{i},h_{j}]=0,[h_{i},e_{j}]=a_{ij}e_{j},[h_{i},f_{j}]=-a_{ij}f_{j},[e_{i},f_{j}]=\delta_{ij}h_{i},$$
> $$(\mathfrak{ad}(e_{i}))^{1-a_{ij}}e_{j}=0,(\mathfrak{ad}(f_{i}))^{1-a_{ij}}f_{j}=0.$$ 
> This Lie algebra has root space $R$.


So by the above two theorems, there is equivalence between the [[Category|category]] of complex semisimple Lie algebras and the category of reduced root space. The classification of irreducible root spaces is equivalent to the classification of simple Lie algebras.