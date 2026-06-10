---
tags:
  - Area/Physics/ParticlePhysics
  - Area/Physics/FieldTheory
  - Area/Math/Algebra/AssociativeAlgebra
---
## Representations
1. Dirac representation$$\gamma^{0}=\begin{pmatrix}
1&0\\0&-1
\end{pmatrix},\gamma^{i}=\begin{pmatrix}
0&\sigma^{i}\\-\sigma^{i}&0
\end{pmatrix},\gamma^{5}=\begin{pmatrix}
0&1\\1&0
\end{pmatrix}$$
2. Weyl representation$$\gamma^{0}=\begin{pmatrix}
0&1\\1&0
\end{pmatrix},\gamma^{i}=\begin{pmatrix}
0&\sigma^{i}\\-\sigma^{i}&0
\end{pmatrix},\gamma^{5}=\begin{pmatrix}
-1&0\\0&1
\end{pmatrix}.$$

## Traces
$$\begin{align}
&\mathrm{tr}(1)=4 \\
&\mathrm{tr}(\text{odd number of gamma matrices})=0 \\
&\mathrm{tr}(\gamma^{\mu}\gamma^{\nu})=4g^{\mu \nu} \\
&\mathrm{tr}(\gamma^{\mu}\gamma^{\nu}\gamma^{\rho}\gamma^{\sigma})=4(g^{\mu \nu}g^{\rho\sigma}-g^{\mu\rho}g^{\nu\sigma}+g^{\mu\sigma}g^{\nu\rho}) \\
 & \mathrm{tr}(\gamma^{5})=0 \\
 & \mathrm{tr}(\gamma^{\mu}\gamma^{\nu}\gamma^{5})=0 \\
& \mathrm{tr}(\gamma^{\mu}\gamma^{\nu}\gamma^{\rho}\gamma^{\sigma}\gamma^{5})=-4\mathrm{i}\epsilon^{\mu \nu\rho\sigma}
\end{align}$$


## Contractions
$$\begin{align}
 & \gamma^{\mu}\gamma_{\mu}=4 \\
 & \gamma^{\mu}\gamma^{\nu}\gamma_{\mu}=-2\gamma^{\nu} \\
 & \gamma^{\mu}\gamma^{\nu}\gamma^{\rho}\gamma_{\mu}=4g^{\nu\rho} \\
 & \gamma^{\mu}\gamma^{\nu}\gamma^{\rho}\gamma^{\sigma}\gamma_{\mu}=-2\gamma^{\sigma}\gamma^{\rho}\gamma^{\nu}
\end{align}$$
$$\begin{align}
p\!\!\!/\gamma^{\mu}p\!\!\!/&=p_{\nu}p_{\rho}(2\eta^{\mu \nu}\gamma^{\rho}-\gamma^{\mu}\gamma^{\nu}\gamma^{\rho}) \\
&=2p^{\mu}p\!\!\!/-p^{2}\gamma^{\mu}
\end{align}$$
$$\begin{align}
p\!\!\!/\gamma^{\mu}q\!\!\!/+q\!\!\!/\gamma^{\mu}p\!\!\!/&=2p^{\mu}q\!\!\!/-\gamma^{\mu}p\!\!\!/q\!\!\!/+2q^{\mu}p\!\!\!/-\gamma^{\mu}q\!\!\!/p\!\!\!/ \\
&=2(p^{\mu}q^{\nu}+q^{\mu}p^{\nu})\gamma_{\nu}-\gamma^{\mu}p_{\rho}q_{\sigma}(\gamma^{\rho}\gamma^{\sigma}+\gamma^{\sigma}\gamma^{\rho}) \\
&=2(p^{\mu}q\!\!\!/+q^{\mu}p\!\!\!/)-2\gamma^{\mu}p\cdot q \\
&=2(p^{\mu}q_{\nu}+q^{\mu}p_{\nu}+\delta^{\mu}_{~\nu})\gamma_{\nu}
\end{align}$$