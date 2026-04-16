---
tags:
  - Area/Physics/StringTheory
---
In this note, we discuss topics about the action of bosonic string, the classical solutions and associated constraints.

## Action of string
String is a one-dimensional object, a mathematical curve. We consider both open strings, which have end points, and closed strings that are circles from a topological viewpoint. We denote $(\sigma,\tau)$ to be the coordinates of world-sheet of strings. For simplicity, we take $0\leq\sigma\leq \pi$ to be the spatial coordinate, and $\tau\in \mathbb{R}$ to be the time coordinate. The world-sheet is parameterized using $X^{\mu}(\sigma,\tau)$ in the physical spacetime. From now on, we will call the physical spacetime as the *target space*, and the world-sheet as the *base space*.

By the idea advocated by Nambu and Goto, the action for strings is simply proportional to the area of world-sheet:
$$S_{\mathrm{NG}}=-T\int \mathrm{d}^{2}\sigma \sqrt{ \dot{X}^{2}X'^{2}-(\dot{X}\cdot X')^{2} },$$
where 
$$\dot{X}^{\mu}=\frac{\partial X^{\mu}}{\partial \tau},X'^{\mu}=\frac{\partial X^{\mu}}{\partial \sigma}.$$
This formula is slightly troublesome to deal with because of the square root. A equivalent but far more convenient form of the action can be written if one introduces an auxiliary metric of the world-sheet $h_{ab}$. The more convenient form is the Polyakov action:
$$S_{\mathrm{Pol}}=-\frac{T}{2}\int \mathrm{d^{2}\sigma}\sqrt{ -h }h^{ab}\partial _{a}X\cdot \partial _{b}X,$$
where $h=\det(h_{ab})$ and $h^{ab}$ is the inverse of the metric. $T$ is the tension of the string, and is related to the Regge slope parameter by $T=(2\pi\alpha')^{-1}$.

There are few more equivalent perspectives for this action:
1. This action never requires the target space to be 4-dimensional. On the other hand, the quantum mechanics requires for $26$-dimensional spacetime.
2. This action also can be used to describe a field theory on the $1+1$ spacetime with $N$ massless scalar fields $X^{\mu}(\sigma,\tau)$. The Poincaré invariance is the internal symmetry of this field theory. 
3. Because of the metric term, this action also describe a $1+1$-dimensional gravity theory.

This action admits following symmetries:
1. The Poincaré invariance of the target space.
2. Reparameterization invariance of the base space: $\sigma,\tau\to\sigma'(\sigma,\tau),\tau'(\sigma,\tau)$.
3. Weyl-scaling invariance of the base space: $h_{ab}(\sigma,\tau)\to \Lambda(\sigma,\tau)h_{ab}$.
With the latter two symmetries, one can determine the three independent components of $h_{ab}$ completely by fix the gauge. 

The infinitesimal variance of the reparameterization is
$$\delta \sigma^{a}=\xi^{a},\delta X^{\mu}=\xi^{a}\partial _{a}X^{\mu},\delta h^{ab}=\xi^{c}\partial _{c}h^{ab}-\partial _{c}\xi^{a}h^{cb}-\partial _{c}\xi^{b}h^{ac}.$$
and the Weyl scaling is
$$\delta h^{ab}=\Lambda h^{ab}.$$
### EOM and constraints
The equations of motion for $X^{\mu}$ and $h_{ab}$ are given by variation of the action:
$$-\frac{2}{T}\frac{\delta S_{\mathrm{Pol}}}{\delta X^{\mu}}=\partial _{a}(\sqrt{ -h }h^{ab}\partial _{b}X_{\mu})=0, -\frac{2}{T} \frac{1}{\sqrt{ -h }} \frac{\delta S_{\mathrm{pol}}}{\delta h^{ab}}=T_{ab}=\partial _{a}X\cdot\partial _{b}X-\frac{1}{2}h_{ab}h^{cd}\partial _{c}X\cdot \partial _{d}X.$$
Since $h_{ab}$ is not dynamic, the variation w.r.t. $h^{ab}$ results in a conserved quantity $T_{ab}$, the energy-momentum tensor on the 2-dimensional base space. The equation $T_{ab}=0$ becomes a constraint over the fields $X^{\mu}$. Alongside, the tensor is traceless $h^{ab}T_{ab}=0$ as a consequence of Weyl invariance.

There is one thing we have ignored in the above derivation when varying $X^{\mu}$: the boundary term. Explicitly it is
$$\int \mathrm{d}^{2}\sigma \partial _{a}(\sqrt{ -h }h^{ab}\partial _{b}X\cdot\delta X).$$
Evaluating such term will result in additional conditions for solve the EOM.

Now, before actually attempting to solve the EOM for $X^{\mu}$, let's first fix the gauge for simplicity. We have stated that the reparameterization invariance and Weyl invariance allow us to completely determine the metric $h_{ab}$ for the world-sheet, thus now we will use the flat gauge: $h_{ab}=\eta_{ab}$. In this case, the EOM is the 2-dimensional wave equation:
$$\left( \frac{\partial^{2}}{\partial \sigma^{2}}-\frac{\partial^{2}}{\partial \tau^{2}} \right)X^{\mu}=0.$$
At the same time, the boundary term is
$$\int \mathrm{d}\sigma \mathrm{d}\tau[\partial _{\sigma}(\partial _{\sigma}X\cdot\delta X)-\partial _{\tau}(\partial _{\tau}X\cdot\delta X)]=0.$$
Since the boundary of coordinate $\tau$ is at infinity, we are confident to set the second term to zero, leaving the spatial boundary term:
$$\int \mathrm{d}\tau\Big(X'\cdot\delta X\big|_{\sigma=\pi}-X'\cdot\delta X\big|_{\sigma=0}\Big)=0.$$
For closed string, the periodicity conditions $X^{\mu}(\sigma=0)=X^{\mu}(\sigma=\pi),X'_{\mu}(\sigma=0)=X_{\mu}'(\sigma=\pi)$ directly vanishes this term. But for open string, we must impose extra boundary conditions:
1. Neumann boundary conditions: $X'_{\mu}(\sigma=0)=X_{\mu}'(\sigma=\pi)=0$.
2. Dirichlet boundary conditions: $X_{\mu}(\sigma=0)=X_{\mu}(\sigma=\pi)=0$.
3. Mixed boundary conditions

As usual in 2-dimension, the general solution to the massless wave equation can be written as
$$X^{\mu}(\sigma,\tau)=X^{\mu}_{\mathrm{R}}(\sigma^{-})+X_{\mathrm{L}}^{\mu}(\sigma^{+})$$
where $\sigma^{\pm}=\tau\pm\sigma$ is the *lightcone coordinates*. The arbitrary function $X_{\mathrm{R}}^{\mu}(\sigma^{-})$ is called the *right-moving modes*, while $X_{\mathrm{L}}^{\mu}(\sigma^{+})$ is called the *left-moving modes*. Now in lightcone coordinates, the constraint is
$$(\partial _{+}X)^{2}=(\partial _{-}X)^{2}=0\to \dot{X}_{\mathrm{R}}^{2}=\dot{X}^{2}_{\mathrm{L}}=0$$
The tracelessness is automatically satisfied by the constraints.

Now for closed string, we must impose periodicity conditions, that leads to a Fourier decomposition of the general solution:
$$X_{\mathrm{R}}^{\mu}(\sigma^{-})=\frac{1}{2}x^{\mu}+\alpha'p^{\mu}\sigma ^{-}+\mathrm{i}\sqrt{ \frac{\alpha'}{2} }\sum_{n\neq0} \frac{1}{n}\alpha^{\mu}_{n}\mathrm{e}^{ -2\mathrm{i}n\sigma^{-} },$$
$$X_{\mathrm{L}}^{\mu}(\sigma^{+})=\frac{1}{2}x^{\mu}+\alpha'p^{\mu}\sigma ^{+}+\mathrm{i}\sqrt{ \frac{\alpha'}{2} }\sum_{n\neq0} \frac{1}{n}\tilde{\alpha}^{\mu}_{n}\mathrm{e}^{ -2\mathrm{i}n\sigma^{+} }.$$
The requirement for $X^{\mu}$ being real function leads to
$$x^{\mu},p^{\mu}\in \mathbb{R},\alpha^{\mu}_{-n}=(\alpha^{\mu}_{n})^{\dagger},\tilde{\alpha}^{\mu}_{-n}=(\tilde{\alpha}_{n}^{\mu})^{\dagger}.$$
For opens strings, we have similar formulae after imposing boundary conditions. As an example, $X'^{\mu}(\sigma=0)=X'^{\mu}(\sigma=\pi)=0$ leads to
$$X^{\mu}(\sigma,\tau)=x^{\mu}+2\alpha'p^{\mu}\tau+\mathrm{i}\sqrt{ 2\alpha' }\sum_{n\neq0} \frac{1}{n}\alpha_{n}^{\mu}\mathrm{e}^{ -\mathrm{i}n\tau }\cos n\sigma.$$
It is a standing wave solution. The constants $x^{\mu},p^{\mu}$ stands for the position and momentum of the string.

With all these solutions, we are able to derive the Hamiltonian for strings:
$$H=\frac{1}{4\pi\alpha'}\int_{0}^{\pi}\mathrm{d}\sigma(\dot{X}^{2}+X'^{2})=\left\{\begin{align}
&\frac{1}{2}\sum_{-\infty}^{\infty}\alpha_{-n}\cdot\alpha_{n}\qquad\qquad\qquad\quad\text{(open strings)} \\
&\frac{1}{2}\sum_{-\infty}^{\infty}(\alpha_{-n}\cdot\alpha_{n}+\tilde{\alpha}_{-n}\cdot\tilde{\alpha}_{n})\qquad\text{(closed strings)} 
\end{align}\right.$$

The last thing is to consider the constraints concretely. Use the mode expansions for closed string we have
$$\begin{align}
\dot{X}_{\mathrm{R}}^{2}&= 2\alpha'\sum_{n,m}\alpha_{n}\cdot\alpha_{m}\mathrm{e}^{ -2\mathrm{i}(n+m)\sigma^{-} }, \\
\dot{X}_{\mathrm{L}}^{2}&=2\alpha'\sum_{n,m}\tilde{\alpha}_{n}\cdot\tilde{\alpha}_{m}\mathrm{e}^{ -2\mathrm{i}(n+m)\sigma^{+} }.
\end{align}$$
where $\alpha_{0}^{\mu}=\sqrt{ \frac{\alpha}{2} }p^{\mu}$ . We can further define the Fourier components as
$$L_{m}=\frac{1}{2}\sum_{n}\alpha_{m-n}\cdot\alpha_{n},\tilde{L}_{m}=\frac{1}{2}\sum_{n}\tilde{\alpha}_{m-n}\cdot\tilde{\alpha}_{n}.$$
The above discussion is similar for open string. Here one has $H=L_{0}$ for open strings and $H=L_{0}+\tilde{L}_{0}$ for closed strings. The constraint equations state the vanishing of each Fourier components, especially:
$$L_{0}=\frac{1}{2}\left( \alpha'p_{\mu}p^{\mu}+\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n} \right)=0.$$
Thus the mass for oscillator modes is
$$M^{2}=-p_{\mu}p^{\mu}=\frac{1}{\alpha'}\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n} .$$
And for closed strings
$$M^{2}=\frac{2}{\alpha'}\sum_{n=1}^{\infty}(\alpha_{-n}\cdot\alpha_{n} +\tilde{\alpha}_{-n}\cdot\tilde{\alpha}_{n} ).$$

The Fourier modes of the energy-momentum tensor $L_{m},\tilde{L}_{m}$ are called *Virasoro operators*. They furnish a algebra by their Poisson brackets:
$$[L_{m},L_{n}]_{\mathrm{PB}}=\mathrm{i}(m-n)L_{m+n},[\tilde{L}_{m},\tilde{L}_{n}]=\mathrm{i}(m-n)\tilde{L}_{m+n}.$$
This is called **Virasoro algebra**. The algebra arises as the residual conformal symmetry after fixing the gauge.