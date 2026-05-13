---
tags:
  - Area/Math/Algebra/LieAlgebra
  - Area/Math/Algebra/LieAlgebra/RootSystem
---
Let $\mathfrak{g}$ be a finite-dimensional complex [[Simple Lie Algebra|semisimple]] [[Lie Algebra|Lie algebra]], $\mathfrak{h}$ be its [[Cartan Subalgebra|Cartan subalgebra]], and $\Delta$ be the set of [[Root Space|roots]].

A **Cartan-Weyl basis** is a basis of $\mathfrak{g}$ adapted to the [[Root Space|root space decomposition]]
$$
\mathfrak{g}=\mathfrak{h}\oplus\bigoplus_{\alpha\in\Delta}\mathfrak{g}_{\alpha}.
$$
It consists of:
1. a basis $\{H_{i}\}$ of $\mathfrak{h}$,
2. one nonzero root vector $E_{\alpha}\in\mathfrak{g}_{\alpha}$ for each root $\alpha\in\Delta$.

Thus
$$
\{H_{i}\}\cup\{E_{\alpha}:\alpha\in\Delta\}
$$
is a basis of $\mathfrak{g}$.

## Commutation relations
The Cartan-Weyl basis satisfies
$$
[H_{i},H_{j}]=0,
$$
$$
[H_{i},E_{\alpha}]=\alpha(H_{i})E_{\alpha}.
$$

For root vectors, one has
$$
[E_{\alpha},E_{-\alpha}]\in\mathfrak{h}.
$$
With a normalization of $E_{\alpha}$ and $E_{-\alpha}$, this can be written with the [[Root Space#Coroot|coroot]] $H_{\alpha}$ as
$$
[E_{\alpha},E_{-\alpha}]=H_{\alpha}.
$$

If $\alpha+\beta\in\Delta$, then
$$
[E_{\alpha},E_{\beta}]=N_{\alpha,\beta}E_{\alpha+\beta}
$$
for some structure constant $N_{\alpha,\beta}\in\mathbb{C}$. If $\alpha+\beta\notin\Delta$ and $\beta\neq-\alpha$, then
$$
[E_{\alpha},E_{\beta}]=0.
$$

## Remarks
1. The Cartan-Weyl basis is not unique, since each root vector $E_{\alpha}$ can be rescaled.
2. The relation $[E_{\alpha},E_{-\alpha}]=H_{\alpha}$ fixes only the product of the scalings of $E_{\alpha}$ and $E_{-\alpha}$.
3. In this basis, elements of $\mathfrak{h}$ are the diagonal part of the adjoint action, and root vectors are eigenvectors of all $\mathrm{ad}_{h}$, $h\in\mathfrak{h}$.
