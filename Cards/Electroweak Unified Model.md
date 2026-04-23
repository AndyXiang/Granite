---
tags:
  - Area/Physics/ParticlePhysics
  - Area/Physics/FieldTheory/QuantumFieldTheory
---
The theory of **electroweak unified model** (EUM) is a **[[Gauge Field|gauge field theory]] with maximally breaking of [[Chiral Symmetry|chiral symmetry]]**. The gauge symmetry [[Group|group]] is $\mathrm{SU}(2)\times \mathrm{U}(1)$, and the maximally breaking of chiral symmetry refers to that the gauge field couples with left-handed fermions only.


## Gauge fields and Higgs field
Under the electroweak gauge field, we denote the representation a matter field lives in by a pair of integer $(j,Y)$, standing for the $(2j+1)$-dimensional [[Irreducible Representation|irreducible representation]] of $\mathrm{SU}(2)$, and the charge w.r.t. $\mathrm{U}(1)$. The [[Higgs Field|Higgs field]] is a complex [[Scalar Field|scalar field]] $\varphi$ in the $\left( \frac{1}{2},-\frac{1}{2} \right)$ representation. Thus the covariant derivative of it is:
$$\begin{align}
D_{\mu}\varphi&=\partial _{\mu}\varphi-\mathrm{i}\left( g_{2}A^{a}_{\mu}\frac{\sigma^{a}}{2}- \frac{1}{2}g_{1}B_{\mu} \right)\varphi.
\end{align}$$
Here $A_{\mu}^{a},B_{\mu}$ are gauge fields, $\sigma^{a},a=1,2,3$ are [[Pauli Matrices|Pauli matrices]].

We know that the [[Boson|gauge bosons]] in EUM, the [[W Boson|W bosons]] and [[Z Boson|Z boson]], are massive. Theoretically, this is accomplished by [[Spontaneous Symmetry Breaking|spontaneous breaking]] of the gauge symmetry. Suppose the scalar field has a potential
$$V(\varphi)=\frac{1}{4}\lambda\left( \varphi ^{\dagger}\varphi-\frac{1}{2}v^{2} \right)^{2},$$
which gives the scalar field a nonzero vacuum expectation value (VEV) $\braket{ \Omega | \varphi(x)|\Omega }=(v /\sqrt{ 2 },0)^{\mathsf{T}}$. We now choose a perturbation vacuum as
$$\varphi(x)=\frac{1}{\sqrt{ 2 }}\begin{pmatrix}
v+H(x) \\\rho(x)
\end{pmatrix}.$$
Then in this vacuum, a mass term for gauge fields are introduced from the covariant derivative term as
$$\begin{align}
\mathcal{L}_{\pu{ mass of gauge }}=-\frac{v^{2}}{8}\begin{pmatrix}
1&0
\end{pmatrix}\begin{pmatrix}
g_{2}A^{3}_{\mu}-g_{1}B_{\mu}&g_{2}(A^{1}_{\mu}-\mathrm{i}A^{2}_{\mu})\\g_{2}(A^{1}_{\mu}+\mathrm{i}A^{2}_{\mu}) & -g_{2}A^{3}_{\mu}-g_{1}B_{\mu}
\end{pmatrix}^{2}\begin{pmatrix}
1\\0
\end{pmatrix} .
\end{align}$$
The term contains the mixing of gauge fields as the interaction eigenstates. Now let's diagonalize the matrix. First one defines the [[Weak Mixing Angle|weak mixing angle]] as
$$\theta_{W}=\arctan\left( \frac{g_{1}}{g_{2}} \right),$$
and the mass eigenstates as
$$\begin{align}
W^{\pm}_{\mu}&=\frac{1}{\sqrt{ 2 }}(A^{1}_{\mu}\mp \mathrm{i}A^{2}_{\mu}), \\
Z_{\mu}&=\cos\theta_{W}A_{\mu}^{3}-\sin\theta_{W}B_{\mu}, \\
A_{\mu}&=\sin\theta_{W}A_{\mu}^{3}+\cos\theta_{W}B_{\mu}.
\end{align}$$
Now the mass term becomes
$$\begin{align}
\mathcal{L}_{\pu{ mass of gauge }}&=-\frac{1}{8}g_{2}^{2}v^{2}\begin{pmatrix}
1&0
\end{pmatrix}\begin{pmatrix}
\frac{1}{\cos\theta_{W}}Z_{\mu}&\sqrt{ 2 }W_{\mu}^{+}\\\sqrt{ 2 }W^{-}_{\mu}&-\frac{1}{\sin\theta_{W}}A_{\mu}
\end{pmatrix}^{2}\begin{pmatrix}
1\\0
\end{pmatrix} \\
&=-\left( \frac{g_{2}v}{2} \right)^{2}W^{+\mu}W^{-}_{\mu}-\frac{1}{2}\left( \frac{g_{2}v}{2\cos\theta_{W}} \right)^{2}Z^{\mu}Z_{\mu}.
\end{align}$$
Here the two gauge field $W_{\mu}^{\pm}, Z_{\mu}$ obtains the masses as
$$M_{W}=\frac{g_{2}v}{2},M_{Z}=\frac{g_{2}v}{2\cos\theta_{W}}.$$
The massless gauge field $A_{\mu}$ (distinguish from $A^{a}_{\mu}$) is identified as the [[Z Electromagnetic Interaction|electromagnetism]] field, or the corresponding [[Photon|photon]] field. The measurements on the masses give
$$\cos\theta_{W}\approx 0.881.$$
For simplicity, let's work in [[Unitary Gauge|unitary gauge]], where we set $\rho(x)=0$. The potential now reads
$$V(H)=\frac{1}{4}\lambda v^{2}H^{2}+\frac{1}{4}\lambda vH^{3}+\frac{1}{16}\lambda H^4.$$
The kinetic term for gauge fields give 
$$\begin{align}
\mathcal{L}&=-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}-\frac{1}{4}Z_{\mu \nu}Z^{\mu \nu}-D^{\dagger \mu}W^{-\nu}D_{\mu}W^{+ }_{\nu}+D^{\dagger \mu}W^{-\nu}D_{\nu}W^{+ }_{\mu} \\
&\qquad+\mathrm{i}e(F^{\mu \nu}+\cot\theta_{W}Z^{\mu \nu})W^{+}_{\mu}W^{-}_{\nu}-\frac{e^{2}}{2\sin ^{2}\theta_{W}}(W^{+\mu}W^{-}_{\mu}W^{+\nu}W^{-}_{\nu}-W^{+\mu}W^{+}_{\mu}W^{-\nu}W^{-}_{\nu}).
\end{align}$$
The several new objects are defined by
$$\begin{align}
&F_{\mu \nu}=\partial _{\mu}A_{\nu}-\partial _{\nu}A_{\mu},Z_{\mu \nu}=\partial _{\mu}Z_{\nu}-\partial _{\nu}Z_{\mu}, \\
&D^{\mu}W^{+\nu}=\partial _{\mu}W^{+\nu}-\mathrm{i}e(A_{\mu}+\cot\theta_{W}Z_{\mu}), \\
&D^{\mu}W^{-\nu}=\partial _{\mu}W^{+\nu}-\mathrm{i}e(-A_{\mu}+\cot\theta_{W}Z_{\mu}), \\
&e=g_{2}\sin\theta_{W}.
\end{align}$$

The full Lagrangian for electroweak and Higgs sector is
$$\begin{align}
\mathcal{L}&=-\frac{1}{4}F_{\mu \nu}F^{\mu \nu}-\frac{1}{4}Z_{\mu \nu}Z^{\mu \nu}-D^{\dagger \mu}W^{-\nu}D_{\mu}W^{+ }_{\nu}+D^{\dagger \mu}W^{-\nu}D_{\nu}W^{+ }_{\mu} \\
&\qquad+\mathrm{i}e(F^{\mu \nu}+\cot\theta_{W}Z^{\mu \nu})W^{+}_{\mu}W^{-}_{\nu} \\
&\qquad-\frac{e^{2}}{2\sin ^{2}\theta_{W}}(W^{+\mu}W^{-}_{\mu}W^{+\nu}W^{-}_{\nu}-W^{+\mu}W^{+}_{\mu}W^{-\nu}W^{-}_{\nu}) \\
&\qquad-\left( M_{W}^{2}W^{+\mu}W^{-}_{\mu}+\frac{1}{2}M_{Z}^{2}Z^{\mu}Z_{\mu} \right)(1+v^{-1}H)^{2} \\
&\qquad-\frac{1}{2}\partial ^{\mu}H\partial _{\mu}H-\frac{1}{4}\lambda v^{2}H^{2}-\frac{1}{4}\lambda vH^{3}-\frac{1}{16}\lambda H^4
\end{align}$$

## Lepton Sector
In order to construct a chiral theory that is consistent with experimental observation, the left-handed and right-handed leptons are described separately by Weyl spinors. Here we introduce two Weyl fields $l_{L}$ and $e_{R}$ in the representation $\left( \frac{1}{2},-\frac{1}{2} \right)$ and $(0,-1)$ of $\mathrm{SU(2)\times U(1)}$, such that
$$\begin{align}
&D_{\mu}l_{L}=\partial _{\mu}l_{L}-\frac{\mathrm{i}}{2}(g_{2}A_{\mu}^{a}\sigma^{a}-g_{1}B_{\mu})l_{L} \\
&D_{\mu}e_{R}=\partial _{\mu}e_{R}-\mathrm{i}g_{1}B_{\mu}e_{R}.
\end{align}$$
The kinetic term for Weyl fields are
$$\mathcal{L}_{\mathrm{kin}}=\mathrm{i}l^{\dagger}\bar{\sigma}^{\mu}D_{\mu}l+\mathrm{i}e_{R}^{\dagger}\bar{\sigma}^{\mu}D_{\mu}e_{R}.$$
Leptons are all color singlets, thus no [[Strong Interaction|strong interaction]] here.

There is no naive mass term $m(l^{\dagger}_{L}e_{R}+e_{R}^{\dagger}l_{L})$ for leptons, since this is not a gauge group singlet
$$\left( \frac{1}{2}, \frac{1}{2} \right)\otimes (0,-1)\cong\left( \frac{1}{2},-\frac{1}{2} \right).$$
However, a Yukawa coupling associated with Higgs field can give the leptons' mass after spontaneous symmetry breaking. From the aspect of [[Representation (Lie Group)|representation of Lie groups]], a term like $\varphi l_{L}e_{R}^{\dagger}$ is in the representation
$$\left( \frac{1}{2},-\frac{1}{2} \right)\otimes \left( \frac{1}{2},-\frac{1}{2} \right)\otimes (0,1)=(1,0)\otimes (3,0),$$
so by choosing a projector, one can get a representation $(1,0)$. After all, the allowed Yukawa term is
$$\mathcal{L}_{\pu{ Yukawa}}=-\frac{1}{\sqrt{ 2 }}y_{e}e_{R}^{\dagger}\varepsilon^{ij}\varphi_{i}l_{j}+\mathrm{h.c.}$$
After symmetry breaking, the VEV results in the mass term
$$\mathcal{L}_{\pu{ Yukawa}}=-\frac{1}{2}y_{e}(v+H)e_{R}^{\dagger}e_{L}+\mathrm{h.c.}$$
where we have written 
$$l=\begin{pmatrix}
\nu_{L}\\e_{L}
\end{pmatrix},$$
so the $\nu_{L}$ corresponding to [[Neutrino|neutrinos]] has zero mass.

For gauge fields in mass eigenstates, one has
$$\begin{align}
&g_{2}A^{1}_{\mu}T^{1}+g_{2}A^{2}_{\mu}T^{2}=\frac{g_{2}}{\sqrt{ 2 }}\begin{pmatrix}
0&W^{+}_{\mu}\\W^{-}_{\mu}&0
\end{pmatrix}, \\
&g_{2}A^{3}_{\mu}T^{3}+g_{1}B_{\mu}Y=e(T^{3}+Y)A_{\mu}+e(\cot\theta_{W}T^{3}-\tan\theta_{W}Y)Z_{\mu}.
\end{align}$$
With the representation, we have
$$\begin{align}
&T^{3}\nu_{L}=\frac{1}{2}\nu_{L},T^{3}e_{L}=-\frac{1}{2}e_{L},T^{3}e_{R}=0, \\
&Y\nu_{L}=-\frac{1}{2}\nu_{L},Ye_{L}=-\frac{1}{2}e_{L},Ye_{R}=-e_{R}.
\end{align}$$
One can define $Q=T^{3}+Y$ as the generator of electric charge, since
$$Q\nu_{L}=0,Qe_{L}=-e_{L},Qe_{R}=-e_{R}.$$
With $Q$, the gauge field part is written as
$$eQA_{\mu}+\frac{e}{\sin\theta_{W}\cos\theta_{W}}(T^{3}-\sin ^{2}\theta_{W}Q)Z_{\mu}.$$
Now couplings of gauge bosons and leptons are
$$\frac{g_{2}}{\sqrt{ 2 }}(W_{\mu}^{+}J^{+\mu}+W_{\mu}^{-}J^{-\mu})-eA_{\mu}J^{\mu}_{\mathrm{EM}}+eZ_{\mu}J^{\mu}_{Z},$$
where the currents are defined by
$$\begin{align}
&J^{+\mu}=\nu ^{\dagger}_{L}\bar{\sigma}^{\mu}e_{L},J^{-\mu}=e^{\dagger}_{L}\bar{\sigma}^{\mu}\nu_{L},J_{\pu{ EM}}^{\mu}=e^{\dagger}_{L}\bar{\sigma}^{\mu}e_{L}+e^{\dagger}_{R}\bar{\sigma}^{\mu}e_{R}, \\
&J^{\mu}_{Z}=\frac{2}{\sin 2\theta_{W}}\left[ \left( \sin ^{2}\theta_{W}-\frac{1}{2} \right)e^{\dagger}_{L}\bar{\sigma}^{\mu}e_{L}+\frac{1}{2}\nu_{L}^{\dagger}\bar{\sigma}^{\mu}\nu_{L}+\sin ^{2}\theta_{W}e^{\dagger}_{R}\bar{\sigma}^{\mu}e_{R} \right].
\end{align}$$

### Generations of Lepton
Now let's introduce the extra generations of leptons, and denote the generation indices with uppercase letters $I,J,\cdots$. The Yukawa coupling is now
$$\mathcal{L}_{\mathrm{Yukawa}}=-\frac{1}{2}(v+H)Y_{e,IJ}\tilde{e}_{R,I}^{\dagger}\tilde{e}_{L,J}+\mathrm{h.c .}$$
The currents are now
$$\begin{align}
&J^{+\mu}=\tilde{\nu} ^{\dagger}_{L,I}\bar{\sigma}^{\mu}\tilde{e}_{L,I},J^{-\mu}=\tilde{e}^{\dagger}_{L,I}\bar{\sigma}^{\mu}\tilde{\nu}_{L,I},J_{\pu{ EM}}^{\mu}=\tilde{e}^{\dagger}_{L,I}\bar{\sigma}^{\mu}\tilde{e}_{L,I}+\tilde{e}^{\dagger}_{R,I}\bar{\sigma}^{\mu}\tilde{e}_{R,I}, \\
&J^{\mu}_{Z}=-\cot 2 \theta_{W}\tilde{e}^{\dagger}_{L,I}\bar{\sigma}^{\mu}\tilde{e}_{L,I}-\csc 2\theta_{W}\tilde{\nu}_{L,I}^{\dagger}\bar{\sigma}^{\mu}\tilde{\nu}_{L,I}+\tan\theta_{W}\tilde{e}^{\dagger}_{R,I}\bar{\sigma}^{\mu}\tilde{e}_{R,I}.
\end{align}$$
First let us diagonalize the mass matrices $Y_{e,IJ}$, as 
$$Y_{e}=E_{R}^{\dagger}\mathrm{diag}(m_{e},m_{\mu},m_{\tau})E_{L},$$
then the mass eigenstates are
$$e_{L}=E_{L}\tilde{e}_{L},e_{R}=E_{R}\tilde{e}_{R}.$$
The currents are also diagonalized since the neutrinos can rotate as above, which is not the case in quark sector.

## Quark Sector
Similar to leptons, only left-handed quarks take part in the weak interaction, thus the analysis only differs from the representation that quarks live in. Left-handed quarks represents by doublet Weyl field 
$$q_=\begin{pmatrix}
u_{L}\\d_{L}
\end{pmatrix}$$
lives in the $\left( \frac{1}{2}, \frac{1}{6} \right)$ representation of $\mathrm{SU(2)\times U(1)}$. The right-handed quarks are singlet Weyl fields where $u_{R}$ lives in $\left( 0, \frac{2}{3} \right)$, $d_{R}$ lives in $\left( 0, -\frac{1}{3} \right)$.

As before, a Yukawa coupling with Higgs field is required to introduce mass terms for quarks. The allowed Yukawa term in Standard Model is
$$\mathcal{L}_{\mathrm{Yukawa}}=-\frac{1}{\sqrt{ 2 }}d_{R}^{\dagger}y_{d}\varepsilon^{ij}\varphi_{i}q_{j}-\frac{1}{\sqrt{ 2 }}u_{R}^{\dagger}y_{u}\varphi_{i}^{\dagger}q_{i}+\mathrm{h.c.}$$
After SSB, one has
$$\mathcal{L}_{\mathrm{Yukawa}}=-\frac{1}{2}(v+H)d^{\dagger}_{R}y_{d}d_{L}-\frac{1}{2}(v+H)u^{\dagger}_{R}y_{u}u_{L}+\mathrm{h.c .}$$
Here each Weyl spinor $u_{R/L},d_{R /L}$ are all color triplets, so $y_{d},y_{u}$ are also $3\times3$ matrices. 

Follow the representations of quarks, we have
$$\begin{align}
&T^{3}u_{L}=\frac{1}{2}u_{L},T^{3}d_{L}=-\frac{1}{2}d_{L},T^{3}u_{R}=T^{3}d_{R}=0, \\
&Yu_{L}=\frac{1}{6}u_{L},Yd_{L}=\frac{1}{6}d_{L},Yu_{R}=\frac{2}{3}u_{R},Yd_{R}=-\frac{1}{3}d_{R}, \\
&Qu_{L}=\frac{2}{3}u_{L},Qd_{L}=-\frac{1}{3}d_{L},Qu_{R}=\frac{2}{3}u_{R},Qd_{R}=-\frac{1}{3}d_{R}.
\end{align}$$
We can also define the currents for quarks.
$$\begin{align}
&J^{+\mu}=u_{L}^{\dagger}\bar{\sigma}^{\mu}d_{L},J^{-\mu}=d^{\dagger}_{L}\bar{\sigma}^{\mu}u_{L}, J_{\mathrm{EM}}^{\mu}=\frac{2}{3}(u^{\dagger}_{L}\bar{\sigma}^{\mu}u_{L}+u^{\dagger}_{R}\bar{\sigma}^{\mu}u_{R})-\frac{1}{3}(d^{\dagger}_{L}\bar{\sigma}^{\mu}d_{L}+d^{\dagger}_{R}\bar{\sigma}^{\mu}d_{R}) \\
&J_{Z}^{\mu}=\frac{2}{\sin 2\theta_{W}}\left[ \left( \frac{1}{2}-\frac{2}{3}\sin ^{2}\theta_{W} \right) u^{\dagger}_{L}\bar{\sigma}^{\mu}u_{L}+\left( -\frac{1}{2}+\frac{1}{3}\sin ^{2}\theta_{W} \right)d^{\dagger}_{L}\bar{\sigma}^{\mu}d_{L}-\frac{2}{3}\sin ^{2}\theta_{W}u^{\dagger}_{R}\bar{\sigma}^{\mu}u_{R}+\frac{1}{3}\sin ^{2}\theta_{W} d^{\dagger}_{R}\bar{\sigma}^{\mu}d_{R}\right].
\end{align}$$

### Generations of Quarks
There are three generations of quarks. When diagonalizing the mass matrices, one needs to introduce four unitary matrices
$$Y_{u}=U_{R}^{\dagger}\mathrm{diag}(m_{u},m_{c},m_{t})U_{L},Y_{d}=D_{R}^{\dagger}\mathrm{diag}(m_{d},m_{s},m_{b})D_{L}.$$
The weak charged current will now introduce the mixing across the generations, 
$$J^{+\mu}=(U_{L}^{\dagger}D_{L})_{IJ}u^{\dagger}_{L,I}\bar{\sigma}^{\mu}d_{L,J},J^{-\mu}=(D_{L}^{\dagger}U_{L})_{IJ}d_{L,I}^{\dagger}\bar{\sigma}^{\mu}u_{L,J}.$$
The [[Cabbibo-Koyabashi-Maskawa Matrix|CKM matrix]] is defined by $V=D^{\dagger}_{L}U_{L}$ representing the mixing.

