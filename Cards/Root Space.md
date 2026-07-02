---
tags:
  - Area/Math/Algebra/VectorSpace/InnerProductSpace/RootSpace
---
Let $E$ be a real [[Inner Product Space|inner product space]] with inner product $(\cdot,\cdot):E\times E\to \mathbb{R}$. A **root space** $R$ is a finite [[Subset|subset]] of $E-\{ 0 \}$ such that:
1. $R$ generates $E$, i.e. $E=\mathrm{span}_{\mathbb{R}}(R)$.
2. $\forall\alpha,\beta\in R$, the number $n(\alpha,\beta)=2(\alpha,\beta) /(\beta,\beta)$ is an integer.
3. Let $s_{\alpha}:E\to E$ as $$s_{\alpha}(x)=x-\frac{2(\alpha,x)}{(\alpha,\alpha)}\alpha.$$ Then $\forall\alpha,\beta\in R,s_{\alpha}(\beta)\in R$.

The number $r=\mathrm{dim}(E)$ is called the **rank** of $R$.

A **[[Morphism|morphism]] of root spaces** is a morphism of [[Vector Space|vector spaces]] $f:E_{1}\to E_{2}$ such that $f(R_{1})=R_{2}$ and $n_{f(\alpha)f(\beta)}=n_{\alpha\beta}$ for any $\alpha,\beta\in R_{1}$.

A root space $R$ satisfying that, if $\alpha,k\alpha$ are both roots then $k=\pm1$, is called a **reduced root space**.

For root $\alpha$, the **coroot** is $\alpha^{\vee}\in E^{*}$ defined by $\alpha^{\vee}(\lambda)=2(\alpha,\lambda) /(\alpha,\alpha)$.
## Positive roots and simple roots
Given a root space $R$, we can always choose a subset $R^{+}$ such that
1. For any $\alpha\in R$, exactly one of $\pm \alpha$ is contained in $R^{+}$.
2. For any two distinct $\alpha,\beta\in R^{+}$, if $\alpha+\beta\in R$, then $\alpha+\beta\in R^{+}$.
The elements of $R^{+}$ are called **positive roots**.

This also can be done by choosing a $p\in R$ such that $\forall\alpha\in R,(p,\alpha)\neq0$, then $R^{+}=\{ \alpha\in R:(\alpha,p)>0 \}$.

A positive root is called **simple** if it can not be written as a sum of two positive roots. The set of simple roots is denoted by $\Pi \subset R^+$. $\Pi$ forms a basis of the vector space $E$.

The set $\Pi$ of simple roots can be expressed with [[Dynkin Diagrams|Dynkin diagrams]] which are defined following:
1. For each simple root we construct a vertex.
2. For each pair of distinct simple roots $\alpha_{i},\alpha_{j}$, we connect the corresponding vertices by $n$ edges, where $n$ depends on the angle $\varphi= \arccos\frac{(\alpha_{i},\alpha_{j})}{|\alpha_{i}||\alpha_{j}|}$: 
- $\varphi=\pi /2,n=0$ (vertices are not connected).
- $\varphi=2\pi /3,n=1$.
- $\varphi=3\pi /4,n=2$.
- $\varphi=5\pi/6,n=3$.
3. For each pair of distinct simple roots $\alpha_{i},\alpha_{j}$, if $|\alpha_{i}|\neq|\alpha_{j}|$ and they are not orthogonal, we orient the edge as the longer one pointing towards the shorter one.

Irreducible reduced root spaces are fully class by simple roots and Dynkin diagrams:
1. $A_{n} (n\geq 1)$ 
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.3) {};
		\node at (0, -0.3) {};
		\node[node] (a1) at (0, 0) {};
		\node[node] (a2) at (1, 0) {};
		\draw[edge] (a1) -- (a2);
		\draw[edge] (a2) -- (1.6, 0);
		\draw[edge] (1.7,0) -- (1.8, 0);
		\draw[edge] (1.9,0) -- (2, 0);
		\draw[edge] (2.1,0) -- (2.2, 0);
		\draw[edge] (2.3,0) -- (2.4, 0);
		\draw[edge] (2.5,0) -- (2.6, 0);
		\draw[edge] (2.7,0) -- (2.8, 0);
		\node[node] (a3) at (3.5, 0) {};
		\node[node] (a4) at (4.5, 0) {};
		\draw[edge] (a3) -- (a4);
		\draw[edge] (2.9, 0) -- (a3);
	\end{tikzpicture}
\end{document}
```
2. $B_{n}(n\geq 2)$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.3) {};
		\node at (0, -0.3) {};
		\node[node] (a1) at (0, 0) {};
		\node[node] (a2) at (1, 0) {};
		\draw[edge] (a1) -- (a2);
		\draw[edge] (a2) -- (1.6, 0);
		\draw[edge] (1.7,0) -- (1.8, 0);
		\draw[edge] (1.9,0) -- (2, 0);
		\draw[edge] (2.1,0) -- (2.2, 0);
		\draw[edge] (2.3,0) -- (2.4, 0);
		\draw[edge] (2.5,0) -- (2.6, 0);
		\draw[edge] (2.7,0) -- (2.8, 0);
		\draw[edge] (2.9, 0) -- (3.5, 0);
		\draw[edge] (4.5, 0.05) -- (5.5, 0.05);
		\draw[edge] (4.5, -0.05) -- (5.5, -0.05);
		\draw[edge] (3.5, 0) -- (4.5, 0); 
		\node[node] (a3) at (3.5, 0) {};
		\node[node] (a4) at (4.5, 0) {};
		\node[node] (a5) at (5.5, 0) {};
		\draw[edge] (4.9, 0.15) -- (5.1, -0.01);
		\draw[edge] (4.9, -0.15) -- (5.1, 0.01);
	\end{tikzpicture}
\end{document}
```
3. $C_{n}(n\geq 2)$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.3) {};
		\node at (0, -0.3) {};
		\node[node] (a1) at (0, 0) {};
		\node[node] (a2) at (1, 0) {};
		\draw[edge] (a1) -- (a2);
		\draw[edge] (a2) -- (1.6, 0);
		\draw[edge] (1.7,0) -- (1.8, 0);
		\draw[edge] (1.9,0) -- (2, 0);
		\draw[edge] (2.1,0) -- (2.2, 0);
		\draw[edge] (2.3,0) -- (2.4, 0);
		\draw[edge] (2.5,0) -- (2.6, 0);
		\draw[edge] (2.7,0) -- (2.8, 0);
		\draw[edge] (2.9, 0) -- (3.5, 0);
		\draw[edge] (4.5, 0.05) -- (5.5, 0.05);
		\draw[edge] (4.5, -0.05) -- (5.5, -0.05);
		\draw[edge] (3.5, 0) -- (4.5, 0); 
		\node[node] (a3) at (3.5, 0) {};
		\node[node] (a4) at (4.5, 0) {};
		\node[node] (a5) at (5.5, 0) {};
		\draw[edge] (5.1, 0.15) -- (4.9, -0.01);
		\draw[edge] (5.1, -0.15) -- (4.9, 0.01);
	\end{tikzpicture}
\end{document}
```
4. $D_{n}(n\geq 4)$:
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.8) {};
		\node at (0, -0.3) {};
		\node[node] (a1) at (0, 0) {};
		\node[node] (a2) at (1, 0) {};
		\draw[edge] (a1) -- (a2);
		\draw[edge] (a2) -- (1.6, 0);
		\draw[edge] (1.7,0) -- (1.8, 0);
		\draw[edge] (1.9,0) -- (2, 0);
		\draw[edge] (2.1,0) -- (2.2, 0);
		\draw[edge] (2.3,0) -- (2.4, 0);
		\draw[edge] (2.5,0) -- (2.6, 0);
		\draw[edge] (2.7,0) -- (2.8, 0);
		\draw[edge] (2.9, 0) -- (3.5, 0);
		\draw[edge] (4.5, 0) -- (5.2, 0.7);
		\draw[edge] (4.5, 0) -- (5.2, -0.7);
		\draw[edge] (3.5, 0) -- (4.5, 0); 
		\node[node] (a3) at (3.5, 0) {};
		\node[node] (a4) at (4.5, 0) {};
		\node[node] (a5) at (5.2, 0.7) {};
		\node[node]  at (5.2, -0.7) {};
	\end{tikzpicture}
\end{document}
```
5. $E_{6}$ 
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (2, 1.1) {};
		\draw[edge] (0, 0) -- (1, 0);
		\draw[edge] (1, 0) -- (2, 0);
		\draw[edge] (2, 0) -- (3, 0);
		\draw[edge] (3, 0) -- (4, 0);
		\draw[edge] (2, 0) -- (2, 1);
		\node[node] at (0, 0) {};
		\node[node] at (1, 0) {};
		\node[node] at (2, 0) {};
		\node[node] at (3, 0) {};
		\node[node] at (4, 0) {};
		\node[node] at (2, 1) {};
	\end{tikzpicture}
\end{document}
```
6. $E_{7}$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (2, 1.1) {};
		\draw[edge] (0, 0) -- (1, 0);
		\draw[edge] (1, 0) -- (2, 0);
		\draw[edge] (2, 0) -- (3, 0);
		\draw[edge] (3, 0) -- (4, 0);
		\draw[edge] (4, 0) -- (5, 0);
		\draw[edge] (2, 0) -- (2, 1);
		\node[node] at (0, 0) {};
		\node[node] at (1, 0) {};
		\node[node] at (2, 0) {};
		\node[node] at (3, 0) {};
		\node[node] at (4, 0) {};
		\node[node] at (2, 1) {};
		\node[node] at (5, 0) {};
	\end{tikzpicture}
\end{document}
```
7. $E_{8}$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (2, 1.1) {};
		\draw[edge] (0, 0) -- (1, 0);
		\draw[edge] (1, 0) -- (2, 0);
		\draw[edge] (2, 0) -- (3, 0);
		\draw[edge] (3, 0) -- (4, 0);
		\draw[edge] (4, 0) -- (5, 0);
		\draw[edge] (5, 0) -- (6, 0);
		\draw[edge] (2, 0) -- (2, 1);
		\node[node] at (0, 0) {};
		\node[node] at (1, 0) {};
		\node[node] at (2, 0) {};
		\node[node] at (3, 0) {};
		\node[node] at (4, 0) {};
		\node[node] at (2, 1) {};
		\node[node] at (5, 0) {};
		\node[node] at (6, 0) {};
	\end{tikzpicture}
\end{document}
```
8. $F_{4}$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.3) {};
		\node at (0, -0.3) {};
		\draw[edge] (0, 0) -- (1, 0);
		\draw[edge] (1, 0.05) -- (2, 0.05);
		\draw[edge] (1, -0.05) -- (2, -0.05);
		\draw[edge] (2, 0) -- (3, 0);
		\draw[edge] (1.4, 0.15) -- (1.6, -0.01);
		\draw[edge] (1.4, -0.15) -- (1.6, 0.01);
		\node[node] at (0, 0) {};
		\node[node] at (1, 0) {};
		\node[node] at (2, 0) {};
		\node[node] at (3, 0) {};
	\end{tikzpicture}
\end{document}
```
9. $G_{2}$
```tikz
\begin{document}
	\usetikzlibrary{arrows.meta,calc}  
	\tikzset{  
		node/.style={  
			circle,  
			draw,  
			fill=white,  
			inner sep=0pt,  
			minimum size=8pt,
			line width=1pt
		},  
		edge/.style={  
			line width=1.2pt  
		},  
		arrow/.style={  
			-{Latex[length=2mm,width=1.6mm]},  
			line width=0.6pt  
		}  
	}
	\begin{tikzpicture}
		\node at (0, 0.3) {};
		\node at (0, -0.3) {};
		\draw[edge] (1, 0.075) -- (2, 0.075);
		\draw[edge] (1, 0) -- (2, 0);
		\draw[edge] (1, -0.075) -- (2, -0.075);
		\draw[edge] (1.4, 0.15) -- (1.6, -0.01);
		\draw[edge] (1.4, -0.15) -- (1.6, 0.01);
		\node[node] at (1, 0) {};
		\node[node] at (2, 0) {};
	\end{tikzpicture}
\end{document}
```

