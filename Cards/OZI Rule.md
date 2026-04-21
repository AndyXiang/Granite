---
tags:
  - Area/Physics/ParticlePhysics
  - Area/Physics/FieldTheory/QuantumFieldTheory
---
The *Okubo-Zweig-Iizuka rule*, or **OZI rule**, is a heuristic rule that, if the [[Cards/Feynman Diagram|Feynman diagram]] of a decay process is disconnected between initial and final states when all internal [[Z Gluon|gluon]] lines are removed, such process is heavily suppression.

Theoretically, this is the consequence of [[Quantum Chromodynamics|QCD]] that the coupling constant decreases as the energy increasing. 

For example, the process of $\phi\to \pi^{+}\pi^{-}\pi^{0}$ has the Feynman diagram as following
```tikz
\begin{document}
	\usetikzlibrary{decorations.markings, decorations.pathmorphing}
	\tikzset{
		fermion/.style={
			postaction={decorate},
		    decoration={markings, mark=at position #1 with {\arrow{stealth}}},
		},
		fermion/.default=0.5,
		photon/.style={
			decorate,
		    decoration={snake, amplitude=1.2mm, segment length=3.5mm},
		},
		gluon/.style={
			decorate,
		    decoration={coil, amplitude=0.6mm, segment length=1.2mm},
		},
		vertex/.style={
		    circle,
		    fill=black,
		    draw=black,
		    inner sep=0pt,
		    minimum size=2.2pt
		},
	}
	\begin{tikzpicture}
		\draw[fermion] (-2,0.2) -> (-1,0.6);
		\draw[fermion] (-1,0.6) -> (-0.8,0);
		\draw[fermion] (-0.8,0) -> (-1,-0.6);
		\draw[fermion] (-1,-0.6) -> (-2,-0.2);
		  
		\node[vertex] at (-1,0.6) {};
		\node[vertex] at (-0.8,0) {};
		\node[vertex] at (-1,-0.6) {};
		  
		\draw[gluon] (-1,0.6) -> (0.7,0.6);
		\draw[gluon] (-0.8,0) -> (-0.2,0);
		\draw[gluon] (-1,-0.6) -> (0.7,-0.6);
		  
		\node[vertex] at (0.7,0.6) {};
		\node[vertex] at (-0.2,0) {};
		\node[vertex] at (0.7,-0.6) {};
		
		\draw[fermion=0.25] (1,1.2) -> (-0.2,0);
		\draw[fermion=0.8] (-0.2,0) -> (1,-1.2);
		\draw[fermion] (0.7,0.6) -> (1,0.9);
		\draw[fermion] (1,0.15) -> (0.7,0.6);
		\draw[fermion] (1,-0.9) -> (0.7,-0.6);
		\draw[fermion] (0.7,-0.6) -> (1,-0.15);
		
		\node at (-2.3,0) {$\phi$};
		\node at (1.3,1.1) {$\pi^-$};
		\node at (1.3,0.05) {$\pi^0$};
		\node at (1.3,-1) {$\pi^+$};
	\end{tikzpicture}
\end{document}
```
The left part is disconnected to the right part if all gluon lines are removed.

