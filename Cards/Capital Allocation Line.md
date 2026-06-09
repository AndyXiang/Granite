---
tags:
  - Area/Finance/Portfolio
---
**Capital allocation line (CAL)** is a graph created by investors to measure the the trade-off of risk and return for a [[Portfolio|portfolio]] composed of a risky and a risk-free asset. The formula is
$$E(r_{C})=r_{F}+\sigma_{C} \frac{E(r_{P})-r_{F}}{\sigma_{P}},$$
where $C$ is the combination of a risky asset $P$ and a risk-free asset $F$. The slope is known as [[Sharpe Ratio|Sharpe ration]].

With borrowing at higher rates as $r_{B}>r_{F}$, the according line is **kinked CAL**:
$$E(r_{C})=\left\{ \begin{align}
&r_{F}+\sigma_{C} \frac{E(r_{P})-r_{F}}{\sigma_{P}} &\sigma_{C}\geq\sigma_{P}  \\
&r_{B}+\sigma_{C} \frac{E(r_{P})-r_{B}}{\sigma_{P}} &\sigma_{C}<\sigma_{P}
\end{align} \right. $$
