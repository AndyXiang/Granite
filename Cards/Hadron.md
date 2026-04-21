---
tags:
  - Area/Physics/ParticlePhysics/Hadron
  - Area/Physics/FieldTheory/QuantumChromodynamics
---
In particle physics, hadron is 

## $\mathrm{SU}(3)$ Quark Model
In 1964, Gell-Mann and Zweig proposed the $\mathrm{SU}(3)$ [[Quark Model|Quark Model]], with there more elementary components for hadrons, as *quarks*. Quarks have three [[Flavor Symmetry|flavors]], denoted by $u,d,s$. They form the [[Fundamental Representation|fundamental representation]] $3$ of $\mathrm{SU}(3)$ [[Flavor Symmetry|flavor symmetry]], and their anti-particles form the [[Complex Conjugate Representation|complex conjugate representation]] $3^{*}$. The quantum numbers of quarks are list below:

| Quark | $I$           | $I_{3}$        | $B$           | $S$  | $Y$            | $Q$            |
| ----- | ------------- | -------------- | ------------- | ---- | -------------- | -------------- |
| $u$   | $\frac{1}{2}$ | $\frac{1}{2}$  | $\frac{1}{3}$ | $0$  | $\frac{1}{3}$  | $\frac{2}{3}$  |
| $d$   | $\frac{1}{2}$ | $-\frac{1}{2}$ | $\frac{1}{3}$ | $0$  | $\frac{1}{3}$  | $-\frac{1}{3}$ |
| $s$   | $0$           | $0$            | $\frac{1}{3}$ | $-1$ | $-\frac{2}{3}$ | $-\frac{1}{3}$ |

In this model, mesons are a pair of quark and anti-quark $q\bar{q}$, while baryons are composed of three quarks $qqq$. From the representation theory, one has
$$3\otimes 3^{*}\cong 8\oplus 1,3\otimes 3\otimes 3\cong 10\oplus 8\oplus 8\oplus 1.$$
Then one can recover the octet in mesons and baryons, and decuplet in baryons (there are subrepresentations in $qqq$ that are no corresponding particles).

The weight diagram for pseudoscalar meson octet:
```tikz
\begin{document}
	\begin{tikzpicture}[
		dot/.style={circle, fill=black, inner sep=2pt}
	]
		\draw[->, line width=1pt] (-3, 0) -- (3, 0) node[right] {$I_3$};
		\draw[->, line width=1pt] (0, -3) -- (0, 3) node[right] {$Y$};
		
		\draw[line width=0.8pt] (2, 0) -- (1, 2);
		\draw[line width=0.8pt] (-1, 2) -- (1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (2, 0);
		\draw[dashed, line width=0.8pt] (1, 2) -- (1, 0);
		
		\node[dot] at (2, 0) {};
		\node at (2.3, 0.3) {$\pi^+$};
		\node[dot] at (0, 0) {};
		\node at (0.3, 0.3) {$\pi^0$};
		\node at (-0.3, 0.3) {$\eta$};
		\node[dot] at (-2, 0) {};
		\node at (-2.3, 0.3) {$\pi^-$};
		\node[dot] at (1, 2) {};
		\node at (1.3, 2.3) {$K^+$};
		\node[dot] at (-1, 2) {};
		\node at (-1.3, 2.3) {$K^0$};
		\node[dot] at (-1, -2) {};
		\node at (-1.3, -2.3) {$K^-$};
		\node[dot] at (1, -2) {};
		\node at (1.3, -2.3) {$\bar{K}^0$};
		
		\node at (2.3, -0.3) {$1$};
		\node at (-2.3, -0.3) {$-1$};
		\node at (0.3, 2.3) {$1$};
		\node at (0.3, -2.3) {$-1$};
		\node at (1, -0.3) {$1/2$};
		
	\end{tikzpicture}
\end{document}
```

The weight diagram for vector meson octet:
```tikz
\begin{document}
	\begin{tikzpicture}[
		dot/.style={circle, fill=black, inner sep=2pt}
	]
		\draw[->, line width=1pt] (-3, 0) -- (3, 0) node[right] {$I_3$};
		\draw[->, line width=1pt] (0, -3) -- (0, 3) node[right] {$Y$};
		
		\draw[line width=0.8pt] (2, 0) -- (1, 2);
		\draw[line width=0.8pt] (-1, 2) -- (1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (2, 0);
		\draw[dashed, line width=0.8pt] (1, 2) -- (1, 0);
		
		\node[dot] at (2, 0) {};
		\node at (2.3, 0.3) {$\rho^+$};
		\node[dot] at (0, 0) {};
		\node at (0.3, 0.3) {$\rho^0$};
		\node[dot] at (-2, 0) {};
		\node at (-2.3, 0.3) {$\rho^-$};
		\node[dot] at (1, 2) {};
		\node at (1.3, 2.3) {$K^{*+}$};
		\node[dot] at (-1, 2) {};
		\node at (-1.3, 2.3) {$K^{*0}$};
		\node[dot] at (-1, -2) {};
		\node at (-1.3, -2.3) {$K^{*0}$};
		\node[dot] at (1, -2) {};
		\node at (1.3, -2.3) {$\bar{K}^{*0}$};
		
		\node at (2.3, -0.3) {$1$};
		\node at (-2.3, -0.3) {$-1$};
		\node at (0.3, 2.3) {$1$};
		\node at (0.3, -2.3) {$-1$};
		\node at (1, -0.3) {$1/2$};
		
	\end{tikzpicture}
\end{document}
```

The weight diagram for hadron octet:
```tikz
\begin{document}
	\begin{tikzpicture}[
		dot/.style={circle, fill=black, inner sep=2pt}
	]
		\draw[->, line width=1pt] (-3, 0) -- (3, 0) node[right] {$I_3$};
		\draw[->, line width=1pt] (0, -3) -- (0, 3) node[right] {$Y$};
		
		\draw[line width=0.8pt] (2, 0) -- (1, 2);
		\draw[line width=0.8pt] (-1, 2) -- (1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, 2);
		\draw[line width=0.8pt] (-2, 0) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (-1, -2);
		\draw[line width=0.8pt] (1, -2) -- (2, 0);
		\draw[dashed, line width=0.8pt] (1, 2) -- (1, 0);
		
		\node[dot] at (2, 0) {};
		\node at (2.3, 0.3) {$\Sigma^+$};
		\node[dot] at (0, 0) {};
		\node at (0.3, 0.3) {$\Sigma^0$};
		\node at (-0.3, 0.3) {$\Lambda$};
		\node[dot] at (-2, 0) {};
		\node at (-2.3, 0.3) {$\Sigma^-$};
		\node[dot] at (1, 2) {};
		\node at (1.3, 2.3) {$p$};
		\node[dot] at (-1, 2) {};
		\node at (-1.3, 2.3) {$n$};
		\node[dot] at (-1, -2) {};
		\node at (-1.3, -2.3) {$\Xi^-$};
		\node[dot] at (1, -2) {};
		\node at (1.3, -2.3) {$\Xi^0$};
		
		\node at (2.3, -0.3) {$1$};
		\node at (-2.3, -0.3) {$-1$};
		\node at (0.3, 2.3) {$1$};
		\node at (0.3, -2.3) {$-1$};
		\node at (1, -0.3) {$1/2$};
		
	\end{tikzpicture}
\end{document}
```

The weight diagram for hadron decuplet:
```tikz
\begin{document}
	\begin{tikzpicture}[
		dot/.style={circle, fill=black, inner sep=2pt}
	]
		\draw[->, line width=1pt] (-4, 0) -- (4, 0) node[right] {$I_3$};
		\draw[->, line width=1pt] (0, -5) -- (0, 3) node[right] {$Y$};
		
		\draw[line width=0.8pt] (0, -4) -- (3, 2);
		\draw[line width=0.8pt] (3, 2) -- (-3, 2);
		\draw[line width=0.8pt] (-3, 2) -- (0, -4);
		\draw[dashed, line width=0.8pt] (3, 2) -- (3, 0);
		\draw[dashed, line width=0.8pt] (1, 2) -- (1, 0);
		\draw[dashed, line width=0.8pt] (1, -2) -- (-1, -2);
		
		% Delta row
		\node[dot] at (3, 2) {};
		\node at (3.45, 2.2) {$\Delta^{++}$};
		\node[dot] at (1, 2) {};
		\node at (1.35, 2.2) {$\Delta^{+}$};
		\node[dot] at (-1, 2) {};
		\node at (-1.45, 2.2) {$\Delta^{0}$};
		\node[dot] at (-3, 2) {};
		\node at (-3.45, 2.2) {$\Delta^{-}$};
		
		% Sigma* row
		\node[dot] at (2, 0) {};
		\node at (2.3, -0.3) {$\Sigma^{*+}$};
		\node[dot] at (0, 0) {};
		\node at (0.3, -0.3) {$\Sigma^{*0}$};
		\node[dot] at (-2, 0) {};
		\node at (-2.3, -0.3) {$\Sigma^{*-}$};

		% Xi* row
		\node[dot] at (1, -2) {};
		\node at (1.35, -2.3) {$\Xi^{*0}$};
		\node[dot] at (-1, -2) {};
		\node at (-1.45, -2.3) {$\Xi^{*-}$};

		% Omega row
		\node[dot] at (0, -4) {};
		\node at (0.35, -4.3) {$\Omega^{-}$};

		% I3 labels
		\node at (3, -0.35) {$\frac{3}{2}$};
		\node at (1, -0.35) {$\frac{1}{2}$};
		\node at (1.7, 0.3) {$1$};
		\node at (-1.7, 0.3) {$-1$};
		\node at (0.3, 2.3) {$1$};
		\node at (-0.3, -2.3) {$-1$};
		\node at (-0.3, -4.3) {$-2$};
		
	\end{tikzpicture}
\end{document}
```
