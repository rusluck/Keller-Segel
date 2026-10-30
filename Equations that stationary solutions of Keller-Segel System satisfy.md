Taken from Section 2 of [[Schaaf-1985.pdf]]
Also worth mentioning that $u$ and $v$ are defined only on positive solutions on $\Omega$, Don't want to define that as it uses Banach Spaces and Holder Spaces in the definition.
Suppose that $r(s)$ always has a unique solution $r:\mathbb{R}^+\to\mathbb{R}^+$
$$r'(s)=\dfrac {\chi(r,s)}{\mu(r,s)}=\left( \frac{\chi}{\mu} \right)(r,s)$$ for any initial condition $r(s_{0})=r_{0},\quad r_{0},s_{0}\in \mathbb{R}^+$.
Let $\phi(s,\lambda)$ be defined as
$$\phi(s,\lambda)=r(s),\quad r'(s)=\left( \frac{\chi}{\mu} \right)(r,s),\quad r(1)=\lambda$$
Schaaf denotes $\partial_{1}$ and $\partial_{2}$ as the deriatives with respect to the first and second derivative. This happens to be very useful notation.
$$\partial_{1}\phi(s,\lambda)=r'(s)=\left( \frac{\chi}{\mu} \right)(r,s)=\left( \frac{\chi}{\mu} \right)(\phi(s,\lambda),s)$$
Applying the second derivative and applying Clairaut's Theorem,
$$\partial_{1}\partial_{2}\phi=\partial_{2}\partial_{1}\phi=\partial_{2}\left( \frac{\chi}{\mu} \right)(\phi(s,\lambda),s)=\left(\partial_{1}\frac{\chi}{\mu} \right)(\phi(s,\lambda),s)\partial_{2}\phi(s,\lambda),$$
$$\partial_{1}\partial_{2}\phi=\left(\partial_{1}\frac{\chi}{\mu} \right)(\phi(s,\lambda),s)\partial_{2}\phi(s,\lambda)$$
by the Chain Rule.

Therefore $\partial_2 \phi$ solves a [[Linear ODE]], and $\partial_{2}\phi$ must always be positive.

**Theorem 2.1** (Schaaf) If $(u,v)$ is a solution of KS, then there is some positive function $\psi\in C^2(\Omega)$ such that
$$u(x)=\phi(v(x),\lambda) \quad\text{for all }x\in\overline\Omega$$
and $$\nu_{0}\Delta v+k(\phi(v,\lambda),v)=0$$
*Proof.* Let $u$ and $v$ be positive solutions. Then for every $x\in \bar{\Omega}$, there exists a function $r_x:\mathbb{R}^+\to\mathbb{R}^+$ that satisfies $$r_{x}'(s)=\left( \frac{\chi}{\mu} \right)(r_{x},s),\quad r_x(v(x))=u(x)$$
Note that $r_x$ means that $r_x$ is chosen based on $x$, NOT that $r_x$ is the partial derivative of $r$ with respect to $x$.
Anyways, define $\psi(x)=r_{x}(1)$. Then we can define $\phi$ like before as 
$$\phi(s,\lambda)=r_{x}(s),\quad r_{x}(1)=\lambda.$$Then using the two stuff above,
$$u=\phi(v,\psi).$$
From the third Keller-Segel equation, the boundary equations,
$$\begin{aligned}
0&=\partial_{\nu}u \\
 & =\partial_{1}\phi(v,\psi)\partial_{\nu}v+\partial_{2}\phi(v,\psi)\partial_{\nu}\psi  \quad &\text{By Multivariable Chain Rule} \\
 & = \partial_{2}\phi(v,\psi)\partial_{\nu}\psi \quad &\text{By Neumann Boundary Condition}
\end{aligned}$$
Since $\partial_2\phi(v,\psi)\neq 0$ since it is the solution of a linear ODE and is therefore greater than $0$, $\partial_{\nu}\psi=0$, i.e. $\psi$ satisfies the Neumann Boundary Condition.