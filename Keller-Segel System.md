Source: [[Horstmann-2003.pdf]]

The Keller-Segel System is described by the following equations

$$\left.\begin{aligned}
u_{t}  & =   \nabla \cdot (k_{1}(u,v)\nabla u-k_{2}(u,v)\nabla v) & x \in \Omega,t>0 \\
v_{t}   &= k_{c}\nabla v-k_{3}(v)v+uf(v) & x\in \Omega, t>0 \\
\dfrac{ \partial u }{ \partial n } &=  \dfrac{ \partial v }{ \partial n } = 0 & x\in\partial \Omega,t>0 \\
\end{aligned}\right\}$$
where $u$ is the cell density and $v$ is the chemoattractant density, and $n$ is the normal of the boundary $\Omega$.

Renate Schaaf ([[Schaaf-1985.pdf]]) defines the Keller-Segel system as $$\left.\begin{aligned}
u_{t}  & =   \nabla \cdot (\mu(u,v)\nabla u-\chi(u,v)\nabla v) & x \in \Omega,t>0 \\
v_{t}   &= \nu_0\nabla v+k(u,v) & x\in \Omega, t>0 \\
\dfrac{ \partial u }{ \partial \nu } &=  \dfrac{ \partial v }{ \partial \nu } = 0 & x\in\partial \Omega,t>0 \\
\end{aligned}\right\}$$
Note that the letter $\nu$ (pronounced 'Nu') is overloaded - in line 2, $\nu_0$ refers to a coefficient, while in line 3, $\nu$ refers to the outward normal of the boundary $\partial \Omega$.
For the [[Stationary Keller-Segel]] click here