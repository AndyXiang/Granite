---
tags:
  - Area/Math/Topology/Homotopy
  - Area/Math/Algebra/Group
aliases:
  - Fundamental Group
---
Let $\alpha:I\to X$ be a [[Path|loop]] at point $x_{0}$ on the [[Topological Space|topological space]] $X$ and $[\alpha]$ be its.

The set of homotopy classes of loops at $x\in X$ is denoted by $\pi_{1}(X,x)$, which is called the **fundamental [[Group|group]]** (or **first homotopy group**) at $x$, with group properties as followed:
1. $[\alpha]*[\beta]=[\alpha*\beta]$.
2. $[\alpha]*[c_{x}]=[\alpha]$.
3. $[\alpha]*[\alpha ^{-1}]=[c_{x}]\implies[\alpha]^{-1}=[\alpha ^{-1}]$.
Here $c_{x}$ represents the constant loop at $x$.

Let $I^{n}=\{ (s_{1},\cdots,s_{n}):0\leq s_{i}\leq 1 \}$. The continuous map $\alpha:I^{n}\to X$ which maps the boundary $\partial I^{n}$ to a point $x$ of $X$ is called a **n-loop** at $x$. The set of homotopy classes of n-loops at $x\in X$ is denoted by $\pi_{n}(X,x)$, called the **$n$th homotopy group**.

Typically one can define the zeroth homotopy group $\pi_{0}(X)$, which is actually not a group, but the number of the [[Connected Space|connected components]]. 

## Properties
1. If $X$ is [[Connected Space|arcwise connected]], then the homotopy groups at every point are [[Homomorphism (Group)|isomorphic]].  
2. If $X,Y$ are both arcwise connected, then $\pi_{1}(X\times Y)\cong \pi_{1}(X)\oplus \pi_{1}(Y)$.
3. If $X,Y$ are [[Homotopy Equivalence|homotopy equivalent]], and $f:X\to Y$ is a homotopy equivalence, then $\pi_{1}(X,x)$ is isomorphic to $\pi_{1}(Y,f(x))$.
4. Let $(\tilde{X},p)$ be the [[Covering Space|universal covering space]] of $X$, and $p(\tilde{x}_{0})=x_{0}$, then the induced [[Homomorphism (Group)|homomorphism]] $$p_{*}: \pi_{n}(\tilde{X},\tilde{x})\to \pi_{n}(X,x)$$is an isomorphism for $n\geq2$.


## Examples
1. $\pi_{1}(\mathbb{S}^{1})\cong \mathbb{Z}$.
2. $\pi_{1}(\mathbb{T}^{2})\cong \mathbb{Z}\oplus \mathbb{Z}$.
3. $\pi_{1}(\mathrm{\mathrm{SO}}(n))=\mathbb{Z}_{2}$.

Here is a table of some useful homotopy groups:

| Group                  |        $\pi_1$ |      $\pi_2$ |                 $\pi_3$ |                     $\pi_4$ |                     $\pi_5$ |                           $\pi_6$ |
| ---------------------- | -------------: | -----------: | ----------------------: | --------------------------: | --------------------------: | --------------------------------: |
| $\mathrm{SO}(3)$       | $\mathbb{Z}_2$ |          $0$ |            $\mathbb{Z}$ |              $\mathbb{Z}_2$ |              $\mathbb{Z}_2$ |                 $\mathbb{Z}_{12}$ |
| $\mathrm{SO}(4)$       | $\mathbb{Z}_2$ |          $0$ | $\mathbb{Z}+\mathbb{Z}$ | $\mathbb{Z}_2+\mathbb{Z}_2$ | $\mathbb{Z}_2+\mathbb{Z}_2$ | $\mathbb{Z}_{12}+\mathbb{Z}_{12}$ |
| $\mathrm{SO}(5)$       | $\mathbb{Z}_2$ |          $0$ |            $\mathbb{Z}$ |              $\mathbb{Z}_2$ |              $\mathbb{Z}_2$ |                               $0$ |
| $\mathrm{SO}(6)$       | $\mathbb{Z}_2$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                $\mathbb{Z}$ |                               $0$ |
| $\mathrm{SO}(n),\ n>6$ | $\mathbb{Z}_2$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                               $0$ |
| $\mathrm{U}(1)$        |   $\mathbb{Z}$ |          $0$ |                     $0$ |                         $0$ |                         $0$ |                               $0$ |
| $\mathrm{SU}(2)$       |            $0$ |          $0$ |            $\mathbb{Z}$ |              $\mathbb{Z}_2$ |              $\mathbb{Z}_2$ |                 $\mathbb{Z}_{12}$ |
| $\mathrm{SU}(3)$       |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                $\mathbb{Z}$ |                    $\mathbb{Z}_6$ |
| $\mathrm{SU}(n),\ n>3$ |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                $\mathbb{Z}$ |                               $0$ |
| $\mathbb{S}^2$         |            $0$ | $\mathbb{Z}$ |            $\mathbb{Z}$ |              $\mathbb{Z}_2$ |              $\mathbb{Z}_2$ |                 $\mathbb{Z}_{12}$ |
| $\mathbb{S}^3$         |            $0$ |          $0$ |            $\mathbb{Z}$ |              $\mathbb{Z}_2$ |              $\mathbb{Z}_2$ |                 $\mathbb{Z}_{12}$ |
| $\mathbb{S}^4$         |            $0$ |          $0$ |                     $0$ |                $\mathbb{Z}$ |              $\mathbb{Z}_2$ |                    $\mathbb{Z}_2$ |
| $G_2$                  |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                    $\mathbb{Z}_3$ |
| $F_4$                  |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                               $0$ |
| $E_6$                  |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                               $0$ |
| $E_7$                  |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                               $0$ |
| $E_8$                  |            $0$ |          $0$ |            $\mathbb{Z}$ |                         $0$ |                         $0$ |                               $0$ |

Here $G_{2},F_{4},E_{6},E_{7},E_{8}$ are [[Exceptional Lie Groups|exceptional Lie groups]].