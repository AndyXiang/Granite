---
type: card
updated: 2025-11-11
tags:
  - Area/Math/Algebra/Group
---
Let $G$ be a [[Group|group]] $G$ and $\cong$ be a [[Congruence Relation|congruence relation]] over it. The set of congruence classes $G/\cong$ actually admits a well-defined group structure:
1. Closure: $\forall g_{1},g_{2}\in G,[g_{1}]*[g_{2}]=[g_{1}g_{2}]$.
2.  Identity: $[1]$.
3. Inverse: $\forall g\in G,[g]^{-1}=[g^{-1}]$.
We call $G /\cong$ the **factor group**.

There are several way to obtain a congruence relation from $G$.
1. Let $\phi:G\to G'$ be a [[Homomorphism|homomorphism]], then it induces a congruence relation as a corollary of the first [[The Isomorphism Theorems|isomorphism theorem]].
2. Let $H$ be a [[Normal Subgroup|normal subgroup]] of $G$, the [[Equivalence Relation|equivalence relation]] it gives is left to a congruence relation since it is normal. In this case, one usually use the terminology *quotient group*.
3. For every $g\in G$, define the [[Conjugacy Class|conjugation]] of $x\in G$ as $i_{g}(x)=gxg^{-1}$. This is a congruence relation, since $i_{g}(xy)=gxyg^{-1}=(gxg^{-1})(gyg^{-1})=i_{g}(x)i_{g}(y)$.
