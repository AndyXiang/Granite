---
tags:
  - Area/Math/Topology
---
**Paracompact**, as a relaxation the requirement of [[Compact Space|compactness]], has the main requirement that any [[Topological Space|open cover]] can be *locally* refined.

## Definition
Let $(X,\tau)$ be a [[Topological Space|topological space]]. An open cover $\{ U_{i}\in \tau: i\in I \}$ of $X$ is **locally finite**, iff for each point $x\in X$, there exists a [[Topological Space#Related concepts|neighborhoods]] $U_{x}\supset \{ x \}$, such that $U_{x}\cap U_{i}$ for only a finite number of $i\in I$.

A **refinement** of an open cover $\{ U_{i} \}_{I}$ is another open cover $\{ V_{j} \}_{J}$ such that for each $j\in J$, there exists $i\in I$ with $V_{j}\subset U_{i}$.

A **paracompact topological space** is a topological space that every its open cover has refinement by a locally finite open cover.

## Examples
1. Every [[Compact Space|compact space]] is paracompact.
