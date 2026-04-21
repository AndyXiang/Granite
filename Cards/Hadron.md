---
tags:
  - Area/Physics/ParticlePhysics
  - Area/Physics/FieldTheory/QuantumChromodynamics
---
In particle physics, hadron is 

pseudoscalar meson octet:
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

vector meson octet:
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

Hadron octet:
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

Hadron decuplet:
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
