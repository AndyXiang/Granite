---
tags:
  - Area/Finance/Portfolio
---
**Markowitz [[Portfolio|portfolio]] selection model** is a method to choose the best portfolio based on expected rates of return and variances.

Given $n$ risky assets, with a [[Vector Space|vector]] $\mu\in \mathbb{R}^{n}$ for expected rates of return, a [[Matrix|matrix]] $\Sigma\in \mathbb{R}^{n\times n}$ for [[Variance|variances]] and [[Covariance|covariances]].  We want to solve a weight vector $w\in \mathbb{R}^{n}$ for the portfolio. The Markowitz selection model describes the problem as minimizing the variance for a given expected rate of return $\mu_{P}$:
$$\min_{w} w^{\mathsf{T}}\Sigma w$$
subject to $w^\mathsf{T}w=1,w^{\mathsf{T}}\mu=\mu_{P}$.

For every expected rate of return $\mu_{P}$, a best portfolio can be found. Draw these portfolios on the plane $\sigma-\mu_{P}$ that connect a curve. The left-right part of the curve is called the **effective frontier**. It represents the highest return at the specific risk.