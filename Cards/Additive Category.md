---
tags:
  - Area/Math/Category/AdditiveCategory
---
A [[Category|category]] $\mathbf{A}$ is called a **pre-additive category** if $\forall x,y\in \mathrm{ob}(\mathbf{A})$, the set of [[Morphism|morphisms]] $\mathrm{mor}_{\mathbf{A}}(x,y)$ is endowed with the structure of [[Abelian Group|abelian group]] (whose operation is called addition and denoted by $+$), that is compatible with composition.

A [[Functor|functor]] $\mathbf{f}:\mathbf{A}\to \mathbf{A}'$ of pre-additive categories is called **additive functor** iff the [[Map|map]] $\mathbf{f}:\mathrm{mor}_{\mathbf{A}}(x,y)\to \mathrm{mor}_{\mathbf{A}'}(\mathbf{f}(x),\mathbf{f}(y))$ is a [[Group#Basic concepts|morphism]] of abelian groups for all $x,y\in \mathrm{ob}(\mathbf{A})$.

A pre-additive category $\mathbf{A}$ is called an **additive category** iff it has [[Zero Object|zero object]] and [[Direct Sum|direct sum]].