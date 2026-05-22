---
tags:
  - Area/Math/Algebra/LieAlgebra/SemisimpleLieAlgebra
  - Area/Math/Representation
---
In this note, we discuss the classification and representation of complex [[Simple Lie Algebra|semisimple Lie algebras]].

## Cartan subalgebra and root decomposition
The first tool we need is the [[Killing Form|Killing form]] 
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

## Representation