---
tags:
  - Area/Physics/ParticlePhysics
  - Area/Physics/FieldTheory/QuantumElectrodynamics
---
**Møller scattering** refers to the [[Electron|electron]]-electron scattering $e^{-}e^{-}\to e^{-}e^{-}$ in [[Quantum Field Theory|quantum field theory]].

## QED computation
In [[Quantum Electrodynamics|QED]], there are two tree level [[Cards/Feynman Diagram|Feynman diagrams]] contribute to the process
```tikz
\begin{document}
	\usetikzlibrary{decorations.markings, arrows.meta, decorations.pathmorphing}
	\tikzset{
		fermion/pos/.initial=0.55,
		fermion/line width/.initial=1pt,
		fermion/arrow length/.initial=2.5mm,
		fermion/arrow width/.initial=2mm,
		fermion/.style={
			draw,
		    line width=\pgfkeysvalueof{/tikz/fermion/line width},
		    postaction={decorate},
		    decoration={
			    markings,
			    mark=at position \pgfkeysvalueof{/tikz/fermion/pos} with {
				    \arrow{Stealth[
				          length=\pgfkeysvalueof{/tikz/fermion/arrow length},
				          width=\pgfkeysvalueof{/tikz/fermion/arrow width}
			        ]}
			    }
		    },
		},
		photon/line width/.initial=1pt,
		photon/amplitude/.initial=1.2mm,
		photon/segment length/.initial=3.5mm,
		photon/.style={
			decorate,
			line width=\pgfkeysvalueof{/tikz/photon/line width},
		    decoration={
			    snake,
			    amplitude=\pgfkeysvalueof{/tikz/photon/amplitude},
			    segment length=\pgfkeysvalueof{/tikz/photon/segment length},
			},
		},
		vertex/.style={
		    circle,
		    fill=black,
		    draw=black,
		    inner sep=0pt,
		    minimum size=4pt
		},
	}
	\begin{tikzpicture}
		\node at (0,1.9) {$t\mathrm{-channel}$};
		\draw[fermion] (-2,1) -- node[above] {$p_{1}$} (0,1);
		\draw[fermion] (0,1) -- node[above] {$p_{3}$} (2,1);
		\draw[fermion] (-2,-1) -- node[below] {$p_{2}$} (0,-1);
		\draw[fermion] (0,-1) -- node[below] {$p_{4}$} (2,-1);
		\draw[photon] (0,1) -- (0,-1);
		\node[vertex] at (0,1) {};
		\node[vertex] at (0,-1) {};
		\node[left] at (-2,1) {$e^{-}$};
		\node[right] at (2,1) {$e^{-}$};
		\node[left] at (-2,-1) {$e^{-}$};
		\node[right] at (2,-1) {$e^{-}$};

		\node at (8,1.9) {$u\mathrm{-channel}$};
		\draw[fermion] (6,1) -- node[above] {$p_{1}$} (8,1);
		\draw[fermion, fermion/pos=0.75] (8,1) -- node[pos=0.75, below left] {$p_{4}$} (10,-1);
		\draw[fermion] (6,-1) -- node[below] {$p_{2}$} (8,-1);
		\draw[fermion, fermion/pos=0.75] (8,-1) -- node[pos=0.75, above left] {$p_{3}$} (10,1);
		\draw[photon] (8,1) -- (8,-1);
		\node[vertex] at (8,1) {};
		\node[vertex] at (8,-1) {};
		\node[left] at (6,1) {$e^{-}$};
		\node[right] at (10,-1) {$e^{-}$};
		\node[left] at (6,-1) {$e^{-}$};
		\node[right] at (10,1) {$e^{-}$};
	\end{tikzpicture}
\end{document}
```

In the [[Center-of-Mass Frame|center-of-mass frame]], we set the momenta as
$$p_{1}=(E,0,0,p),p_{2}=(E,0,0,-p),p_{3}=(E,p \sin\theta,0,p\cos\theta),p_{4}=(E,-p \sin\theta,0,-p\cos\theta).$$
Define the Mandelstam variables
$$s=(p_{1}+p_{2})^{2},t=(p_{1}-p_{3})^{2},u=(p_{1}-p_{4})^{2},$$
with $s+t+u=4m^{2}$.

The amplitudes are
$$\begin{align}
\mathrm{i}\mathcal{M}_{t}&=(-\mathrm{i}e)^{2}\bar{u}(p_{3})\gamma^{\mu}u(p_{1})\frac{-\mathrm{i}}{t}\bar{u}(p_{4})\gamma_{\mu}u(p_{2}), \\
\mathrm{i}\mathcal{M}_{u}&=(-\mathrm{i}e)^{2}\bar{u}(p_{3})\gamma^{\mu}u(p_{2})\frac{-\mathrm{i}}{u}\bar{u}(p_{4})\gamma_{\mu}u(p_{1}), \\
\mathrm{i}\mathcal{M}&=\mathrm{i}(\mathcal{M}_{t}-\mathcal{M}_{u}).
\end{align}$$
The relative minus sign between two diagrams comes from exchanging the two electrons in the final state.

To compute unpolarized [[Cross section|cross section]], we average over initial spins and sum over final spins:
$$\begin{align}
\overline{|\mathcal{M}|^{2}}&=\frac{1}{4}\sum_{\mathrm{spins}}|\mathcal{M}|^{2} \\
&=2e^{4}\left\{  \frac{s^{2}+u^{2}-8m^{2}(s+u)+24m^{4}}{t^{2}}+\frac{s^{2}+t^{2}-8m^{2}(s+t)+24m^{4}}{u^{2}}+\frac{2(s^{2}-8m^{2}s+12m^{4})}{tu}  \right\}.
\end{align}$$

Using $E_{\mathrm{CM}}^{2}=s=4E^{2}$, $t=-2p^{2}(1-\cos\theta)$, $u=-2p^{2}(1+\cos\theta)$, the tree-level differential cross section is
$$\begin{align}
\frac{\mathrm{d}\sigma}{\mathrm{d}\Omega}&=\frac{1}{64\pi^{2}E_{\mathrm{CM}}^{2}}\overline{|\mathcal{M}|^{2}} \\
&=\frac{\alpha^{2}}{2E_{\mathrm{CM}}^{2}}\left\{  \frac{s^{2}+u^{2}-8m^{2}(s+u)+24m^{4}}{t^{2}}+\frac{s^{2}+t^{2}-8m^{2}(s+t)+24m^{4}}{u^{2}}+\frac{2(s^{2}-8m^{2}s+12m^{4})}{tu}  \right\} \\
&=\frac{\alpha^{2}}{E_{\mathrm{CM}}^{2}p^{4}\sin ^{4}\theta}\Big\{ 4(m^{2}+2p^{2})^{2}+\big[4p^{4}-3(m^{2}+2p^{2})^{2}\big]\sin ^{2}\theta+p^{4}\sin ^{4}\theta\Big\}.
\end{align}$$

In the relativistic limit $m\ll p$,
$$
\frac{\mathrm{d}\sigma}{\mathrm{d}\Omega}=\frac{\alpha^{2}}{E_{\mathrm{CM}}^{2}}\frac{(3+\cos ^{2}\theta)^{2}}{\sin ^{4}\theta}.
$$
When the two final electrons are counted as identical particles over the full angular range, one should either divide the total phase-space integral by $2$ or restrict the angular domain.

### Electroweak corrections
In [[Electroweak Unified Model|electroweak model]], there are extra tree level diagrams where electrons exchange a [[Z Boson|Z boson]] instead of a photon. Other diagrams exchanging [[Higgs Boson|Higgs boson]] and [[Goldstone Theorem|Goldstone boson]] when the model is not in [[Unitary Gauge|unitary gauge]] are possible, but rather smaller comparing to the four diagrams of photon and $Z$ boson.

$Z$ boson prefers left-handed electrons to right-handed, thus there are asymmetry in Møller scattering that reveals the [[Parity Violation|parity violation]].
