---
tags:
  - Area/Physics/QuantumTheory/PathIntegral
  - Area/Physics/FieldTheory/QuantumFieldTheory
---
In [[Path Integral Quantization|path integral formalism]] of [[Quantum Field Theory|QFT]], the question arises that how to describe the [[Symmetry|symmetry]] on quantum aspect. Consider the [[Generating Functional|generating functional]] under the infinitesimal transformation $\phi\to \phi'=\phi+\epsilon F[\phi,x]$ where $f$ is a [[Functional|functional]] of the field $\phi$:
$$\begin{align}
Z'[J]&=\int \mathcal{D}\phi'\exp\left[  \mathrm{i}S'[\phi]+\mathrm{i}\int \mathrm{d}^{d}xJ(x)\phi'(x) \right] \\
&=\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[\phi,J] }\left\{  1+\epsilon\left[ \int \mathrm{d}^{d}x \left( \frac{\delta F[\phi,x]}{\delta \phi(x)} +\mathrm{i}\left( \frac{\delta S}{\delta \phi}+J \right)F\right) \right]  +\mathcal{O}(\epsilon^{2})\right\}.
\end{align}$$
In this formalism, the requirement for this symmetry to hold on quantum aspect is the invariant of generating functional. This results in the **Dyson-Schwinger equation**:
$$\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[J,\phi] }\left\{  \int \mathrm{d}^{d}x \left[ \frac{\delta F}{\delta \phi} +\mathrm{i}\left( \frac{\delta S}{\delta \phi}+J \right)F\right]   \right\}=0.$$

Explicitly, consider the shift of field $F=\delta \phi$, which gives
$$\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[\phi,J] }\int \mathrm{d}^{d}x\left( \frac{\delta S}{\delta \phi}+J \right)\delta \phi(x)=0.$$
