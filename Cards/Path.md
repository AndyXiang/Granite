---
tags:
  - Area/Math/Topology
---
Let $X$ be a [[Topological Space|topological space]] and $I=[0,1]$ be an interval. A [[Continuous Map (Topology)|continuous map]] $\alpha:I\to X$ is called a **path**. The two points $x_{0}=\alpha(0)$ and $x_{1}=\alpha(1)$ are called initial point and end point. If the two points coincide, then the path is called a **loop**. The **constant path** at point $x$ is the path as $\alpha(s)=x,s\in I$.

## Operations
Let $\alpha,\beta:I\to X$ be two paths s.t. $\alpha(1)=\beta(0)$. The **product** of $\alpha$ and $\beta$, denoted by $\alpha*\beta$ is a path in $X$ defined by
$$(\alpha*\beta)(s)=\left\{  \begin{align}
&\alpha(2s),~\qquad\quad0\leq s\leq \frac{1}{2} \\
&\beta(2s-1), ~\quad\frac{1}{2}\leq s\leq1
\end{align}\right.$$

For path $\alpha:I\to X$, the **inverse path** $\alpha ^{-1}$ is defined by
$$\alpha ^{-1}(s)=\alpha(1-s),s\in I.$$
