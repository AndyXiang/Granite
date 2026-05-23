---
tags:
  - Area/Physics/FieldTheory/QuantumFieldTheory
  - Area/Physics/QuantumTheory/PathIntegral
---
Consider the [[Dyson-Schwinger Equation|Dyson-Schwinger equation]] for [[Z Internal Symmetry|internal symmetry]], as $F_{i}[\phi]=\mathrm{i}\theta^{a}T^{a}_{ij}\phi_{j}$, where $T^{a}$ is the generator for internal symmetry, and $\theta^{a}$ may or may not depends on spacetime. The [[Generating Functional|generating functional]] for it is
$$\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[\phi,J] }\left\{  \int \mathrm{d}^{d}x \left[ T^{a}_{ii} +\left( \frac{\delta S}{\delta \phi_{i}}+J_{i} \right)T^{a}_{ij}\phi_{j}\right] \theta^{a}  \right\}=0.$$
By applying functional derivative w.r.t. external source $J(x)$, one gets a series of identities that the [[Correlation Function|correlation functions]] satisfy for the symmetry to be held. They are called **Ward-Takahashi identities**.

## Ward Identity
Suppose the functional measure is invariant under the symmetry transformation, i.e. $\delta F /\delta \phi=0$, and when the variation of the [[Action (Physics)|action]] is a conserved current, the corresponding identities are called **Ward identities**, whose generating functional is
$$\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[\phi,J] }\left\{  \int \mathrm{d}^{d}x  \left( \partial _{\mu}j^{a,\mu}+J_{i}T^{a}_{ij}\phi_{j} \right) \theta^{a}  \right\}=0.$$


## Examples
### $\mathrm{U}(1)$
Consider the global [[Unitary Group|U(1)]] symmetry for complex [[Scalar Field|scalar field]], in which $F[\phi]=\mathrm{i}\theta \phi,F[\phi ^{\dagger}]=-\mathrm{i}\theta \phi ^{\dagger}$. The measure is invariant, and the generating functional is
$$\int \mathcal{D}\phi \mathrm{e}^{ \mathrm{i}S[\phi,J,J^{\dagger}] }\left[ \int \mathrm{d}^{d}x( J^{\dagger}\phi-J\phi ^{\dagger}) \right]=0.$$
The first two correlation functions are
$$\left\langle \phi \right\rangle=\left\langle \phi ^{\dagger} \right\rangle =0,\left\langle \phi ^{\dagger}(x_{1})\phi ^{\dagger}(x_{2}) \right\rangle=\left\langle \phi(x_{1})\phi(x_{2}) \right\rangle=0,\left\langle \phi ^{\dagger}(x_{1})\phi(x_{2}) \right\rangle=\left\langle \phi(x_{2})\phi ^{\dagger}(x_{1}) \right\rangle.      $$

### [[Quantum Electrodynamics|QED]]
Consider the $\mathrm{U}(1)$ gauge symmetry in spinor QED, in which $j^{\mu}=e\bar{\psi}\gamma^{\mu}\psi$, the generating functional is
$$\int \mathcal{D}\bar{\psi}\mathcal{D}\psi \mathrm{e}^{ \mathrm{i}S[\bar{\psi},\psi,\bar{\eta},\eta] }\left\{  \int \mathrm{d}^{d}x[\partial _{\mu}(\bar{\psi}\gamma^{\mu}\psi)+e\bar{\eta}\psi-e\bar{\psi}\eta] \theta(x)\right\}=0.$$
For this to be held on every point of spacetime, one has
$$\int \mathcal{D}\bar{\psi}\mathcal{D}\psi \mathrm{e}^{ \mathrm{i}S[\bar{\psi},\psi,\bar{\eta},\eta] }\left[\partial _{\mu}(\bar{\psi}\gamma^{\mu}\psi)+e\bar{\eta}\psi-e\bar{\psi}\eta \right]=0.$$
The second order correlation function it gives is
$$\partial _{\mu}\left\langle j^{\mu}(x)\psi (x_{1})\bar{\psi}(x_{2}) \right\rangle=-e \delta ^{(4)}(x-x_{1})\left\langle \psi(x_{1})\bar{\psi}(x_{2}) \right\rangle+e\delta^{(4)}(x-x_{2})\left\langle \psi (x_{1})\bar{\psi}(x_{2}) \right\rangle.  $$