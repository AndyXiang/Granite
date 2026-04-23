---
tags:
  - Area/Physics/ParticlePhysics
---
Electron-proton scattering uses the [[Electron|electron]] as a clean electromagnetic probe of [[Proton|proton]] structure. In the elastic regime it measures the proton's electric and magnetic form factors; in the inelastic and deep-inelastic regimes it resolves excited states and partonic substructure through structure functions. The distinction is mainly organized by the four-momentum transfer $Q^2$ and the final-state invariant mass $W$, following the standard elastic form-factor and [[Parton Model|parton model]] frameworks.

## Elastic scattering
In elastic regime, the proton is approximated to be a point-like particle, with correction to its interaction vertex. At [[Quantum Electrodynamics|QED]] leading order, the amplitude for scattering $e^{-}(k)\mathrm{p}(p)\to e^{-}(k')\mathrm{p}(p')$ can be written as
$$A=-\frac{\mathrm{i}e^{2}}{q^{2}}\bar{u}(p')\Gamma^{\mu}(p,p')u(p) \bar{u}(k')\gamma_{\mu}u(k),$$
where $\Gamma_{\mu}(p,p')$ is the vertex for proton. The [[Vector Space|vector space]] for all $4\times4$ matrices is $16$-dimensional, with a basis of [[Gamma Matrices|gamma matrices]] as $\{ 1,\gamma^{5},\gamma^{\mu},\gamma^{\mu}\gamma^{5},\sigma^{\mu \nu} \}$. To assure the [[Z Parity|parity conservation]], the [[Lorentz Group|Lorentz-invariant]] general form of $\Gamma^{\mu}$ is
$$\Gamma^{\mu}(p,p')=K_{1}(q^{2})\gamma^{\mu}+\mathrm{i}\sigma_{\mu \nu}(p'-p)^{\nu}K_{2}(q^{2})+\mathrm{i}\sigma_{\mu \nu}(p'+p)^{\nu}K_{3}(q^{2})+(p'+p)^{\mu}K_{4}(q^{2})+(p'-p)^{\mu}K_{5}(q^{2}),$$
where $q=p'-p$. Use the [[Spinor|Gordon identity]] to simplify
$$J^{\mu}(p',p)=\bar{u}(p')\Gamma^{\mu}u(p)=\bar{u}(p')[\gamma^{\mu}F_{1}(q^{2})+\mathrm{i}F_{2}(q^{2})\sigma^{\mu \nu}q_{\nu}+q^{\mu}F_{3}(q^{2})]u(p).$$
The [[Ward Identity|Ward identity]] (standing for charge conservation) $q_{\mu}J^{\mu}=0$ further requires $F_{3}(q^{2})=0$. Thus one is left with
$$J^{\mu}(p',p)=\bar{u}(p')\Gamma^{\mu}u(p)=\bar{u}(p')[\gamma^{\mu}F_{1}(q^{2})+\mathrm{i}F_{2}(q^{2})\sigma^{\mu \nu}q_{\nu}]u(p),$$
with two **form factors** $F_{1}(q^{2}),F_{2}(q^{2})$.

Now we can compute the differential [[Cross-section|cross-section]]
$$\frac{\mathrm{d}\sigma}{\mathrm{d}\Omega}=\frac{\alpha^{2}\cos^{2} \frac{\theta}{2}}{4E^{2}\sin ^{4} \frac{\theta}{2}} \frac{1}{1+\frac{2E}{m_{\mathrm{p}}}\sin ^{2} \frac{\theta}{2}}\left[ (F_{1}^{2}+Q^{2}F_{2}^{2})+\frac{Q^{2}}{2m_{\mathrm{p}}^{2}} (F_{1}+2m_{\mathrm{p}}F_{2})^{2}\tan ^{2}\frac{\theta}{2}\right].$$
Here $Q^{2}=-q^{2}$ is called the *momentum transfer*. This is called the Rosenbluth formula.

In the limit of $q^{2}\to 0$, we expect this formula returns to the point-like situation, which leads to $F_{1}(0)=1$. Compare with the cross-section of [[Møller Scattering|Møller scattering]], one can find the correction from the [[Magnetic Momentum|magnetic momentum]] of proton is $2m_{\mathrm{p}}F_{2}$. The experiments shows that
$$F_{2}(0)=\frac{1.79}{2m_{\mathrm{p}}}.$$

## Inelastic scattering
Inelastic scattering refers to the processes with excited proton or extra particles in final states: $e^{-}\mathrm{p}\to e^{-}X$. The boundary of elastic regime and inelastic regime is roughly determined by finial state invariant mass $W^{2}=(p+q)^{2}$. In elastic regime, $W^{2}=m_{\mathrm{p}}^{2}$, while in inelastic regime $W^{2}>m_{\mathrm{p}}^{2}$. As the momentum transfer $Q^{2}$ grows bigger, the proton is excited, and one can finds a series of resonance peaks, representing other subsequent [[Hadron|hadrons]]. Typically one has $\mathrm{p}^{*}\to \pi^{0}\mathrm{p},\mathrm{p}^{*}\to \pi^{+}\mathrm{n}$. But these resonances disappear for big enough $Q^{2}$,  representing the highly energetic electron is interacting with subatomic structure of proton. This is called the *deep inelastic scattering*.

In inelastic regime, we can no longer use the expression $J^{\mu}=\bar{u}\Gamma^{\mu}u$ for proton. But at the leading order, one can still employee the current-current interaction form:
$$A=\frac{e^{2}}{q^{2}}j_{\mu}J^{\mu}$$
where $j_{\mu}=\bar{u}(k')\gamma_{\mu}u(k)$ is the electron current. The unpolarized cross section is proportional to the square of amplitude
$$\mathrm{d}\sigma \propto|A|^{2}=\frac{e^{4}}{q^{4}}L_{\mu \nu}W^{\mu \nu},$$
where
$$L_{\mu \nu}=\frac{1}{2}\sum_{r,s}j_{\mu}^{\dagger}j_{\nu}=2\left( k_{\mu}k_{\nu}'+k_{\nu}k_{\mu}'+\frac{q^{2}}{2}g_{\mu \nu} \right),$$
$$W^{\mu \nu}=\frac{1}{2}\int \mathrm{d}^{3}p'\sum_{r,s}J^{\dagger \mu}J^{\nu}\delta^{(4)}(p+q-p').$$
One can also derive the form of this tensor by Lorentz invariance and charge conservation:
$$W^{\mu \nu}(\nu,q^{2})=\left( \frac{q^{\mu}q^{\nu}}{q^{2}}-g^{\mu \nu} \right)W_{1}(\nu,q^{2})+\left( p^{\mu}-\frac{p\cdot q}{q^{2}}q^{\mu} \right)\left( p^{\nu}-\frac{p\cdot q}{q^{2}}q^{\nu} \right) \frac{W_{2}(\nu,q^{2})}{m_{\mathrm{p}}^{2}},$$
where $\nu=p\cdot q /m_{\mathrm{p}}$. $W_{1},W_{2}$ are called the *structure functions*. Now we can write the differential cross section explicitly as
$$\frac{\mathrm{d}\sigma}{\mathrm{d\Omega}\mathrm{d}E'}=\frac{\alpha^{2}}{4E^{2}\sin ^{4} \frac{\theta}{2}} E'\left[ W_{2}(\nu,q^{2})\cos ^{2} \frac{\theta}{2}+2W_{1}(\nu,q^{2}) \sin ^{2} \frac{\theta}{2} \right].$$

The experiments shows the structure functions of nucleon in deep elastic regime appears to have the *scaling phenomenon*, for which the functions $W_{1},W_{2}$ rely only on 
$$x=\frac{Q^{2}}{2m_{\mathrm{N}}\nu}.$$
This shows more information about internal structure of nucleons. The most successful model to explain this phenomenon is the [[Parton Model|parton model]]. 