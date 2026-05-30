---
tags:
  - Area/Physics/StringTheory
---
In this note, we discuss topics about the action of bosonic string, the classical solutions and associated constraints.

## Classic bosonic string
String is a one-dimensional object, a mathematical curve. We consider both open strings, which have end points, and closed strings that are circles from a topological viewpoint. We denote $(\sigma,\tau)$ to be the coordinates of world-sheet of strings. For simplicity, we take $0\leq\sigma\leq \pi$ to be the spatial coordinate, and $\tau\in \mathbb{R}$ to be the time coordinate. The world-sheet is parameterized using $X^{\mu}(\sigma,\tau)$ in the physical spacetime. From now on, we will call the physical spacetime as the *target space*, and the world-sheet as the *base space*.

By the idea advocated by Nambu and Goto, the action for strings is simply proportional to the area of world-sheet:
$$S_{\mathrm{NG}}=-T\int \mathrm{d}^{2}\sigma \sqrt{ \dot{X}^{2}X'^{2}-(\dot{X}\cdot X')^{2} },$$
where 
$$\dot{X}^{\mu}=\frac{\partial X^{\mu}}{\partial \tau},X'^{\mu}=\frac{\partial X^{\mu}}{\partial \sigma}.$$
This formula is slightly troublesome to deal with because of the square root. An equivalent and far more convenient form of the action can be written if one introduces an auxiliary metric $h_{ab}$ of the world-sheet. The more convenient form is the [[Polyakov Action|Polyakov action]]:
$$S_{\mathrm{Pol}}=-\frac{T}{2}\int \mathrm{d^{2}\sigma}\sqrt{ h }h^{ab}\partial _{a}X\cdot \partial _{b}X,$$
where $h=\det(h_{ab})$ and $h^{ab}$ is the inverse of the metric. $T$ is the tension of the string, and is related to the Regge slope parameter by $T=(2\pi\alpha')^{-1}$.

There are few more equivalent perspectives for this action:
1. This action never requires the target space to be 4-dimensional. On the other hand, the consistent of this theory requires for $26$-dimensional spacetime.
2. This action also can be used to describe a field theory on the $1+1$ spacetime with $N$ massless scalar fields $X^{\mu}(\sigma,\tau)$. The Poincaré invariance is then an internal symmetry of this field theory. 
3. Because of the metric term, this action also describe a $1+1$-dimensional gravity theory.

This action admits following symmetries:
1. The Poincaré invariance of the target space $\delta X^{\mu}=a^{\mu}_{~~\nu}X^{\nu}+b^{\mu}$.
2. Reparameterization invariance of the base space: $\sigma,\tau\to\sigma'(\sigma,\tau),\tau'(\sigma,\tau)$.
3. Weyl-scaling invariance of the base space: $h_{ab}(\sigma,\tau)\to \Lambda(\sigma,\tau)h_{ab}$.
With the latter two symmetries, one can determine the three independent components of $h_{ab}$ completely by fixing the gauge. 

### EOM and boundary conditions
The equations of motion for $X^{\mu}$ and $h_{ab}$ are given by variation of the action:
$$-\frac{2}{T}\frac{\delta S_{\mathrm{Pol}}}{\delta X^{\mu}}=\partial _{a}(\sqrt{ h }h^{ab}\partial _{b}X_{\mu})=0, -\frac{2}{T} \frac{1}{\sqrt{ h }} \frac{\delta S_{\mathrm{pol}}}{\delta h^{ab}}=T_{ab}=\partial _{a}X\cdot\partial _{b}X-\frac{1}{2}h_{ab}h^{cd}\partial _{c}X\cdot \partial _{d}X=0.$$
Since $h_{ab}$ is not dynamic, the variation w.r.t. $h^{ab}$ results in a conserved quantity $T_{ab}$, the energy-momentum tensor on the 2-dimensional base space. The equation $T_{ab}=0$ becomes a constraint over the fields $X^{\mu}$. Alongside, the tensor is traceless $h^{ab}T_{ab}=0$ as a consequence of Weyl invariance.

There is one thing we have ignored in the above derivation when varying $X^{\mu}$: the boundary term. Explicitly it is
$$\int \mathrm{d}^{2}\sigma \partial _{a}(\sqrt{ -h }h^{ab}\partial _{b}X\cdot\delta X).$$
Evaluating such term will result in additional conditions for solving the EOM.

Now, before actually attempting to solve the EOM for $X^{\mu}$, let's first fix the gauge for simplicity. We have stated that the reparameterization invariance and Weyl invariance allow us to completely determine the metric $h_{ab}$ for the world-sheet, thus now we will use the flat gauge: $h_{ab}=\eta_{ab}$. In this case, the EOM is the 2-dimensional wave equation:
$$\left( \frac{\partial^{2}}{\partial \sigma^{2}}-\frac{\partial^{2}}{\partial \tau^{2}} \right)X^{\mu}=0.$$
At the same time, the boundary term is
$$\int \mathrm{d}\sigma \mathrm{d}\tau[\partial _{\sigma}(\partial _{\sigma}X\cdot\delta X)-\partial _{\tau}(\partial _{\tau}X\cdot\delta X)]=0.$$
Since the boundary of coordinate $\tau$ is at infinity, we are confident to set the second term to zero, leaving the spatial boundary term:
$$\int \mathrm{d}\tau\Big(X'\cdot\delta X\big|_{\sigma=\pi}-X'\cdot\delta X\big|_{\sigma=0}\Big)=0.$$
For closed string, the periodicity conditions $X^{\mu}(\sigma=0)=X^{\mu}(\sigma=\pi),X'_{\mu}(\sigma=0)=X_{\mu}'(\sigma=\pi)$ directly vanishes this term. But for open string, we must impose extra boundary conditions:
1. Neumann boundary conditions: $X'_{\mu}(\sigma=0)=X_{\mu}'(\sigma=\pi)=0$.
2. Dirichlet boundary conditions: $\delta X_{\mu}(\sigma=0)=\delta X_{\mu}(\sigma=\pi)=0$. This means the two ends of an open string are attached on two hyperplane in target space.
3. Mixed boundary conditions

As usual in 2-dimension, the general solution to the massless wave equation can be written as
$$X^{\mu}(\sigma,\tau)=X^{\mu}_{\mathrm{R}}(\sigma^{-})+X_{\mathrm{L}}^{\mu}(\sigma^{+})$$
where $\sigma^{\pm}=\tau\pm\sigma$ are the *lightcone coordinates*. The arbitrary function $X_{\mathrm{R}}^{\mu}(\sigma^{-})$ is called the *right-moving modes*, while $X_{\mathrm{L}}^{\mu}(\sigma^{+})$ is called the *left-moving modes*. Now in lightcone coordinates, the constraint is
$$(\partial _{+}X)^{2}=(\partial _{-}X)^{2}=0\implies \dot{X}_{\mathrm{R}}^{2}=\dot{X}^{2}_{\mathrm{L}}=0$$
The tracelessness is automatically satisfied by the constraints.

### Mode expansion
One can solve the EOM in lightcone coordinates using Fourier expansion. We need to discuss separately the open string with different boundary conditions and closed string.

For closed string, we must impose periodicity conditions, that leads to a Fourier decomposition of the general solution:
$$\begin{align}
X_{\mathrm{R}}^{\mu}(\sigma^{-})&=\frac{1}{2}x^{\mu}+\alpha'p^{\mu}\sigma ^{-}+\mathrm{i}\sqrt{ \frac{\alpha'}{2} }\sum_{n\neq0} \frac{1}{n}\alpha^{\mu}_{n}\mathrm{e}^{ -2\mathrm{i}n\sigma^{-} }, \\
X_{\mathrm{L}}^{\mu}(\sigma^{+})&=\frac{1}{2}x^{\mu}+\alpha'p^{\mu}\sigma ^{+}+\mathrm{i}\sqrt{ \frac{\alpha'}{2} }\sum_{n\neq0} \frac{1}{n}\tilde{\alpha}^{\mu}_{n}\mathrm{e}^{ -2\mathrm{i}n\sigma^{+} }.
\end{align}$$
The requirement for $X^{\mu}$ being real function leads to
$$x^{\mu},p^{\mu}\in \mathbb{R},\alpha^{\mu}_{-n}=(\alpha^{\mu}_{n})^{\dagger},\tilde{\alpha}^{\mu}_{-n}=(\tilde{\alpha}_{n}^{\mu})^{\dagger}.$$
The integral constants $x^{\mu},p^{\mu}$ stands for the average position and momentum of the string.

For opens strings, we can choose Neumann condition or Dirichlet condition at each end, which leads to four solutions in total:
1. NN: $X_{\mu}'(\sigma=0)=X_{\mu}'(\sigma=\pi)=0$.$$X^{\mu}(\sigma,\tau)=x^{\mu}+2\alpha'p^{\mu}\tau+\mathrm{i}\sqrt{ 2\alpha' }\sum_{n\neq0} \frac{1}{n}\alpha_{n}^{\mu}\mathrm{e}^{ -\mathrm{i}n\tau }\cos n\sigma.$$
2. DD: $X_{\mu}(\sigma=0)=a_{\mu}(\tau), X_{\mu}(\sigma=\pi)=b_{\mu}(\tau)$. $$X^{\mu}(\sigma,\tau)=a^{\mu}+ \frac{b^{\mu}-a^{\mu}}{\pi}\sigma+\mathrm{i}\sqrt{ 2\alpha' }\sum_{n\neq 0} \frac{1}{n}\alpha_{n}\mathrm{e}^{ -\mathrm{i}n\tau } \sin n\sigma.$$
3. ND: $X_{\mu}'(\sigma=0)=0, X_{\mu}(\sigma=\pi)=b_{\mu}(\tau)$. $$X^{\mu}(\sigma,\tau)=b^{\mu}+\mathrm{i}\sqrt{ 2\alpha' }\sum_{r\in \mathbb{Z}+1 /2} \frac{1}{r}\alpha_{r}\mathrm{e}^{ -\mathrm{i}r\tau }\cos r\sigma.$$
4. DN: $X_{\mu}(\sigma=0)=a_{\mu}(\tau),X_{\mu}'(\sigma=\pi)=0$. $$X^{\mu}(\sigma,\tau)=a^{\mu}+\mathrm{i}\sqrt{ 2\alpha' }\sum_{r\in \mathbb{Z}+1 /2} \frac{1}{r}\alpha_{r}\mathrm{e}^{ -\mathrm{i}r\tau }\sin r\sigma$$
There are standing wave solutions. 

With all these solutions, we are able to derive the Hamiltonian for strings:
$$H=\frac{1}{4\pi\alpha'}\int_{0}^{\pi}\mathrm{d}\sigma(\dot{X}^{2}+X'^{2})=\left\{\begin{align}
&\alpha'p^{2}+\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n}&\text{(NN open strings)}  \\
&\frac{(b-a)^{2}}{4\pi^{2}\alpha'}+\sum_{n=1}^{\infty} \alpha_{-n}\cdot\alpha_{n} &(\text{DD open strings})  \\
&\sum_{r\in \mathbb{Z}_{+}+ 1 /2} \alpha_{-r}\cdot\alpha_{r}&(\text{ND\& DN open strings})\\
&\frac{1}{2}\alpha'p^{2}+\sum_{n=1}^{\infty}(\alpha_{-n}\cdot\alpha_{n}+\tilde{\alpha}_{-n}\cdot\tilde{\alpha}_{n})&\text{(closed strings)} 
\end{align}\right.$$

### Constraints
The last thing is to consider the constraints $h^{ab}T_{ab}=0$ concretely. In conformal gauge and lightcone coordinates, the constraint equations are $T_{--}=T_{++}=0$. Use the mode expansions one can rewrite them. Take the closed string for example
$$\begin{align}
T_{++}=\frac{1}{\alpha'}\partial _{+}X\cdot \partial _{+}X=\frac{1}{2}\sum_{m,n\in \mathbb{Z}} \tilde{\alpha}_{m}\cdot\tilde{\alpha}_{n}\mathrm{e}^{ -\mathrm{i}(m+n)\sigma^{+} }, \\
T_{--}=\frac{1}{\alpha'}\partial _{-}X\cdot \partial _{-}X=\frac{1}{2}\sum_{m,n\in \mathbb{Z}} {\alpha}_{m}\cdot{\alpha}_{n}\mathrm{e}^{ -\mathrm{i}(m+n)\sigma^{-} }.
\end{align}$$
We can further define the Fourier components as
$$L_{m}=\frac{1}{2}\sum_{n}\alpha_{m-n}\cdot\alpha_{n},\tilde{L}_{m}=\frac{1}{2}\sum_{n}\tilde{\alpha}_{m-n}\cdot\tilde{\alpha}_{n}.$$
such that $T_{++}=\sum_{n\in \mathbb{Z}} \tilde{L}_{n} \mathrm{e}^{ -\mathrm{i}n\sigma^{+} },T_{--}=\sum_{n\in \mathbb{Z}} {L}_{n} \mathrm{e}^{ -\mathrm{i}n\sigma^{-} }$. Here we denote $\alpha_{0}^{\mu}=\tilde{\alpha}_{0}^{\mu}= \sqrt{ \alpha' /2 }p^{\mu}$. The above discussion is similar for open string. One sees that $H=L_{0}$ for open strings and $H=L_{0}+\tilde{L}_{0}$ for closed strings. The constraint equations state the vanishing of every Fourier components $L_{n}=\tilde{L}_{n}=0$, especially:
$$L_{0}=\frac{1}{2}\left( \alpha'p_{\mu}p^{\mu}+\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n} \right)=0.$$
Thus the mass for oscillator modes is
$$M^{2}=-p_{\mu}p^{\mu}=\frac{1}{\alpha'}\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n} .$$
And for closed strings
$$M^{2}=\frac{1}{\alpha'}\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n}=\frac{1}{\alpha'}\sum_{n=1}^{\infty}\tilde{\alpha}_{-n}\cdot\tilde{\alpha}_{n}  .$$

The Fourier modes of the energy-momentum tensor $L_{m},\tilde{L}_{m}$ are called *Virasoro operators*. They furnish a algebra by their Poisson brackets:
$$[L_{m},L_{n}]_{\mathrm{PB}}=\mathrm{i}(m-n)L_{m+n},[\tilde{L}_{m},\tilde{L}_{n}]_{\mathrm{PB}}=\mathrm{i}(m-n)\tilde{L}_{m+n}.$$
This is called **Virasoro algebra**. The algebra arises as the residual conformal symmetry after fixing the gauge.


## Old covariant quantization
Now we discuss the covariant quantization of bosonic string, which is *old* compared to modern BRST quantization. This quantization requires us to lift every thing in classic theory into operators over a Hilbert space. First one needs the commutators for $X^{\mu}$ and its conjugate momentum
$$[X^{\mu}(\sigma',\tau),\dot{X}^{\nu}(\sigma,\tau)]=2\mathrm{i}\pi\alpha'\delta(\sigma-\sigma')\eta^{\mu \nu},[\dot{X}^{\mu}(\sigma,\tau),\dot{X}^{\nu}(\sigma',\tau)]=[X^{\mu}(\sigma,\tau),X^{\nu}(\sigma',\tau)]=0.$$
Following one lifts the Fourier modes to operators with commutators (for closed strings):
$$[x^{\mu},p^{\mu}]=\mathrm{i}\eta^{\mu \nu},[\alpha_{m}^{\mu},\alpha_{n}^{\nu}]=[\tilde{\alpha}^{\mu}_{m},\tilde{\alpha}_{n}^{\nu}]=m\delta_{m+n}\eta^{\mu \nu},[\alpha_{m}^{\mu},\tilde{\alpha}^{\nu}_{n}]=0.$$
The formulas for open strings are much similar. Naturally, $\alpha_{m}^{\mu}$ and $\tilde{\alpha}^{\nu}_{m}$ are referred to raising and lowering operators, that create ($m>0$) or annihilate ($m<0$) closed string oscillating modes in target space. The ground state $\ket{0,p}$ is defined as the state that is annihilated by $\alpha_{m}^{\mu},m> 0$. It also carries a quantum number as the eigenvalue of $p^{\mu}$.

There is a big flaw in our quantization. The state $\alpha^{0}_{-m}\ket{0,p}$ has negative norm for $m>0$. One can easily see that by $\braket{ 0 |\alpha_{m}^{0}\alpha_{-m}^{0}|0  }=\braket{ 0 |[\alpha_{m}^{0},\alpha_{-m}^{0}]|0  }=-m$. The states with negative norm are called *ghosts*. A consistent theory must be free of ghosts for a sensible causality.

Skip the problem of ghosts for a well, let's see the Virasoro operators. They are products of oscillator modes. In covariant quantization, there is an ambiguity in ordering the products. We denote the correct ordering by *normal ordering*, with a pair of $:$ indicating that, as:
$$L_{m}=\frac{1}{2}\sum_{-\infty}^{\infty}:\alpha_{m-n}\cdot\alpha_{n}:$$
Since $\alpha_{m-n}$ commutes with $\alpha_{n}$ unless $m=0$, the only such ambiguity arises in $L_{0}$. Suppose $L_{0}=\frac{1}{2}\alpha_{0}^{2}+\sum_{n=1}^{\infty}\alpha_{-n}\cdot\alpha_{n}-a$.

Further more, because of the ordering ambiguity, we allow a deformation in algebra from the classic version:
$$[L_{m},L_{n}]=(m-n)L_{m+n}.$$
The quantum effect for this commutator can only come from exchanging oscillators $[\alpha_{m},\alpha_{n}]\propto\delta_{m+n}$, then we are guaranteed to have
$$[L_{m},L_{n}]=(m-n)L_{m+n}+A(m)\delta_{m+n}$$
for some $m$-dependent c-number $A(m)$. This is known as **Virasoro algebra**. Evidently one has $A(-m)=-A(m)$ and $A(0)=0$. To compute the constant, one first notices that $\braket{ 0 |[L_{m},L_{-m}]|0  }=2m\braket{ 0 | L_{0}|0 }+A(m)=A(m)$. Explicitly compute the first one
$$\begin{align}
\braket{ 0 | [L_{m},L_{-m}]|0 }&=\braket{ 0 |L_{m}L_{-m}|0  } \\
&=\frac{1}{4}\sum_{j,k=1}^{m-1} \braket{ 0 |(\alpha_{k}\cdot\alpha_{m-k}) (\alpha_{j-m}\cdot\alpha_{-j})|0  } \\
&=\frac{D}{12}(m^{3}-m).   
\end{align}$$
For convenience, we have
$$[L_{n},\alpha_{m}^{\mu}]=-m\alpha^{\mu}_{m+n},$$
### Remove ghosts
Now we want to solve the problem of ghosts. Our main result will be that, in a certain regime of the value of $D$, the theory will be free of ghosts. The full theorem is call *no ghost theorem*, which is complicated to prove, thus we will derive the boundary of the regime by some analysis, but will not discuss that explicitly every negative-norm state is get rid of.

Let's start with the constraints for Virasoro operators in quantized theory. The classic equation $L_{n}=\tilde{L}_{n}=0$ now should be eased into $L_{n}\ket{\phi}=\tilde{L}_{n}\ket{\phi}=0$ for physical states. For $L_{0}\ket{\phi}=0$ one can find the mass formula for physical states
$$\left( \frac{1}{2}\alpha_{0}^{2}+\sum_{n=1}^{\infty} \alpha_{-n}\cdot\alpha_{n}-a \right)\ket{\phi}=0\implies \frac{\alpha'}{4}M^{2}=N-a, $$
where $N\ket{\phi}=\sum_{n=1}^{\infty} \alpha_{-n}\cdot\alpha_{n}\ket{\phi}$. This is similar in what we do in Gupta-Bleuler quantization for electromagnetic fields. 

So to get rid of ghosts as $\alpha_{-m}^{0}\ket{0,p}$, we want to examine when will they become unphysical. Compute:
$$L_{n}\alpha_{-m}^{0}\ket{0,p}=[L_{n},\alpha_{-m}^{0}]\ket{0,p}=m\alpha_{n-m}^{0}\ket{0,p}.   $$
For $m>1$, set $n=1$, then such state can't always vanish since $\alpha_{n-m}^{0}$ is creation operator. Especially when $m=1,n=1$:
$$L_{1}\alpha_{-1}^{0}\ket{0,p} =\sqrt{ 2\alpha' }p^{0}\ket{0,p}. $$
This state vanishes for $p^{0}=0$. Conversely, if one has $a>1$, then $\alpha_{-1}^{0}\ket{0,p}$ is a tachyon $M^{2}=4(1-a) /\alpha'<0$. For such state, one can find a frame where $p^{0}>0$, meaning such ghost state is physical in that frame. This will leads to a requirement that $a\leq1$. This is very direct necessary condition for the ghost states to be unphysical.

The no ghost theorem states that there is no ghost in bosonic string when $a=1,D=26$, or $a<1,D<25$.

## Lightcone quantization
Now we discuss another quantization that is quite convenient. We begin by introducing lightcone coordinates in target space, for vector $v^{\mu}$
$$v^{\pm}=(v^{0}\pm v^{D-1}) /\sqrt{ 2 },$$
and leave others unchanged. In this coordinates, the metric is
$$\mathrm{d}s^{2}=-2\mathrm{d}x^{+}\mathrm{d}x^{-}+\mathrm{d}x^{i}\mathrm{d}x_{i},$$
and the inner product for $v^{\mu},w^{\mu}$ is
$$v\cdot w=v^{i}w_{i}+v^{+}w_{+}+v^{-}w_{-}.$$

After one imposed the conformal gauge, there is still a residual symmetry of reparameterization symmetry as
$$\sigma^{\pm}\to\tilde{\sigma}^{\pm}(\sigma^{\pm}).$$
Now we choose a gauge such that
$$X^{+}(\sigma,\tau)=x^{+}+p^{+}\tau.$$
Once we fix this gauge, the Virasoro constraint becomes $\dot{X}^{-}\pm X'^{-}=(\dot{X}^{i}\pm X'^{i})^{2} /2p^{+}$. So $X^{-}$ is solved in terms of $X^{i}$. We are now left with $D-2$ d.o.f. for $X^{i}$. Explicitly, the Fourier modes of $X^{-}$ can be expressed as
$$\alpha_{n}^{-}=\frac{1}{p^{+}}\left(\frac{1}{2}\sum_{m=-\infty}^{\infty} :\alpha_{n-m}^{i}\alpha^{i}_{m}:-a\delta_{n} \right).$$
Again, the mass formula is given by $n=0$ as
$$M^{2}=(2p^{+}p^{-}-p^{i}p^{i})=2(N-a)$$
for $N=\sum_{n=1}^{\infty}\alpha_{-n}^{i}\alpha^{i}_{n}$. Here the anomaly constant $a$ can be directly computed as one resolve the normal ordering using commutator as
$$\begin{align}
L_{0}&=\frac{1}{2}\sum_{n=-\infty}^{\infty} :\alpha_{-n}^{i}\alpha_{n}^{i}: \\
&=\frac{\alpha'}{4}p^{2}+N+\frac{1}{2}\sum_{n=1}^{\infty}[\alpha_{n}^{i},\alpha_{-n}^{i}] \\
&=\frac{\alpha'}{4}p^{2}+N-\frac{D-2}{24}.
\end{align}$$
This shows that $a=(D-2) /24$. This is the first time we see the critical dimension of bosonic string as $D=26$ for $a=1$.


## Analysis of spectrum

### Open strings
For critical theory with $D=26$, the vacuum is a tachyon with $M^{2}=-4 /\alpha'$. Next, the first excited state is $\alpha_{-1}^{i}\ket{0,p}$ that is massless. It carries a vector index, so we expect it transforms as the fundamental representation of group $\mathrm{SO}(24) \lhd \mathrm{SO}(1,25)$. This is a massless vector boson with $24$ physical d.o.f.

The second excited states are $\alpha_{-1}^{i}\alpha_{-1}^{j}\ket{0,p}$ and $\alpha_{-2}^{i}\ket{0,p}$, with mass $M^{2}=4 /\alpha'$. The first one transforms as the symmetric rank-2 representation of $\mathrm{SO}(24)$, and the second one is in the fundamental representation again. The total d.o.f. is $324$. Correspondingly, they furnish a symmetric rank-2 representation of $\mathrm{SO}(25)$, the little group for massive spin-2 particles.

Repeat this analysis for the third excited states. They furnish a direct sum representation of $\mathrm{SO}(25)$ with one symmetric rank-3 and one anti-symmetric rank-2.

### Closed strings

For critical closed bosonic string with $D=26$, the level-matching condition requires $N=\widetilde N$. The mass formula is
$$  
M^2=\frac{4}{\alpha'}(N-1)  
=\frac{4}{\alpha'}(\widetilde N-1).  
$$

The vacuum $\ket{0,p}$ is again a tachyon with $M^2=-\frac{4}{\alpha'}$. A closed-string state at level $N=\widetilde N$ is obtained by tensoring a left-moving open-string-like state at level $N$ with a right-moving open-string-like state at level $\widetilde N$.

The first excited state is $\alpha_{-1}^{i}\widetilde{\alpha}_{-1}^{j}\ket{0,p}$. It is massless. For little group $\mathrm{SO}(24)$, it's in the direct product representation $24\otimes24\cong \mathrm{Sym}^{2}(24) \oplus \Lambda^{2}(24) \oplus 1$. So it contains a spin-2 massless boson, an anti-symmetric 2-form field and a singlet called *dilaton*.

The analysis for higher excited states is complicate but similar.
