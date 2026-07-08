---
tags:
  - Area/Math/Set/Order
aliases:
  - Partial Order
  - Total Order
  - Poset
---
Let $P$ be a [[Set|set]] and $\leq$ be a [[Relation|relation]] on $P$. Then $\leq$ is a **partial order** iff satisfies
1. *reflexivity*: $\forall a\in P\implies a\leq a$.
2. *antisymmetry*: $\forall a,b\in P,a\leq b \wedge b\leq a \implies a=b.$
3. *transitivity*: $\forall a,b,c\in P,a\leq b\leq c\implies a\leq c$.
Set $P$ together with a partial order is called a **partially ordered set**, in short a **poset**. More over, a **total order** additionally needs $\forall a,b\in P\to a\leq b\vee b\leq a$.

The **strict order** $<$ refers to $a\leq b\wedge a\neq b$.

Several special elements may exist in a poset $P$:
1. greatest element $a$ s.t. $\forall x\in P,x \leq a.$
2. maximal element $b$ s.t. $\forall x\in P,x\neq b \implies b\nleq x$.
3. least element $c$ s.t. $\forall x\in P,x\geq c$.
4. minimal element $d$ s.t. $\forall x\in P, x\neq c \implies c \ngeq x$.