# 1 Introduction

> We derive facts about magnetic moments from elementary classical and quantum physics.
## 1.1 Magnetic Moments

- Fundamental object in magnetism is the *magnetic moment*, equivalent to a current loop in classical electromagnetism.
$$\textbf{d}\mu = I\textbf{d}S.$$ $\textbf{d}\mu$ - magnetic moment, $I$ - infinitesimal current, $\textbf{d}S$ - area of small loop.

- Sometimes called *magnetic dipole* because it behaves analogously to electric dipoles. 
- Adding up multiple moments in a large surface we get $$\mu = \int{\textbf{d}\mu} = I\int{\textbf{d}S}.$$
### 1.1.1 Magnetic moments and angular momentum

- In atoms $\bf{\mu}$ is associated with orbiting electron, same direction as its angular momentum $\textbf{L}.$
$$\mu = \gamma\bf{L}$$
where $\gamma$ is the *gyromagnetic ratio*. 
### 1.1.2 Precession

- Energy of a magnetic moment $\mu$ in $\bf{B}$:
$$E = -\mu \cdot \bf{B},$$
so that energy is minimized when they are aligned.

- Torque enacted on the magnetic moment:
$$\bf{G} = \mu \times \bf{B},$$
so that moments would turn to be aligned with the field.

- Utilize the relationship between $\mu$ and $\bf{L}$ to get:
$$\cfrac{d\mu}{dt} = \gamma \mu \times \bf{B}.$$
So we get precession and $|\mu|$ is time-independent. *Larmor frequency* $\omega_L = \gamma \bf{B}$ is the frequency of precession. Note that it is independent of polar angle between $\mu$ and $\bf{B}$.
### 1.1.3 The Bohr magneton
> Estimating the size of atomic magnetic moments and atomic gyromagnetic ratio.

$$\mu=\pi r^2I = -\cfrac{e\hbar}{2m_e} \equiv -\mu_B$$
where $\mu_B$ is the Bohr magneton defined by
$$\mu_B = \cfrac{e\hbar}{2m_e}.$$
We assume $\textbf{L} = \hbar$ so $\gamma = -e/2m_e$ and $\omega_L = e\textbf{B}/2m_e.$
### 1.1.4 Magnetization and field
> A magnetic solid consists of many atoms with magnetic moments

- Define magnetization $\textbf{M}$ as magnetic moment per unit volume. Typically on a length-scale where $\textbf{M}$ is a smooth vector field.
- Recall in free space $$\textbf{B} = \mu_0\textbf{H},$$
  while in a magnetic solid $$B = \mu_0(\textbf{H} + \textbf{M}).$$
- In the special case where $\textbf{M}$ and $\textbf{H}$ point in the same direction the solid is called a *linear material* and we can write $$\textbf{M} = \chi\textbf{H}.$$
  where $\chi$ is the *magnetic susceptibility*. We call $\mu_r = 1+\chi$ the relative permeability of the material, just like the relative permittivity $\epsilon_r$. 
- When a magnetic material is placed inside an applied magnetic field $B_a, H_a$, the interior magnetic field generated by the applied magnetic field equals $$H_i = H_a - N\textbf{M}$$ where $N$ is the demagnetizing factor. Thus $$B_i = \mu_0(\textbf{H}_i + \textbf{M}) = \textbf{B}_a + \mu_0(1-N)\textbf{M}.$$
- Note that when magnetization is small (i.e. diamagnetic materials) this effect can largely be ignored. However, in ferromagnetic materials this effect cannot be ignored.

## 1.2 Classical mechanics and magnetic moments
>We describe the effects of applied magnetic fields on charges using purely classical arguments

### 1.2.1 Canonical momentum
- Lorentz force $$\textbf{F} = q(E + \textbf{v} \times \textbf{B}).$$
- We can modify this slightly in a magnetic field, assuming $\textbf{F} = m\cfrac{d\textbf{v}}{dt}$, $\textbf{B} = \nabla \times \textbf{A}$, and $E = -\nabla V - \cfrac{\partial\textbf{A}}{\partial t}$ where $V$ is the electric potential, $\textbf{A}$ is the magnetic vector potential and $m$ is the mass of the particle.  $$m\cfrac{d\textbf{v}}{d t} = -q\nabla V- q\cfrac{\partial \textbf{A}}{\partial t} + q\textbf{v} \times \nabla \times \textbf{A}.$$
  simplifies to $$\cfrac{d}{dt} (m\textbf{v} + q\textbf{A}) = -q\nabla(V - \textbf{v} \cdot \textbf{A}).$$
- Note how this takes the form of a change in momentum $(m\textbf{v} + q\textbf{A})$ corresponds to a negative gradient of a quantity that looks like potential energy $(V - \textbf{v} \cdot \textbf{A})$. This motivates us to define *canonical momentum* $$\textbf{p} = m\textbf{v} + q\textbf{A}$$ and an effective potential energy of $$q(V-\textbf{v}\cdot\textbf{A}).$$
### 1.2.2 The Bohr-van Leeuwen theorem
> In a classical system there is no thermal equilibrium magnetization.

- Magnetization is proportional to the rate of change of energy of the system with applied magnetic field.
- But, no work can be done by an external magnetic field, so there can be no magnetization via classical theory
## 1.3 Quantum mechanics of spin
> Review some results concerning quantum mechanics of electron spin

### 1.3.1 Orbital and spin angular momentum

- *Orbital angular momentum* deals with the angular momentum of an electron revolving around the nucleus, and depends on the electronic state occupied by the electron. 
- $m_l\hbar$ represents the angular momentum along a single axis (e.g. $L_z$) while $\sqrt{l(l+1)}\hbar$ represents the total magnitude of the angular momentum $\textbf{L}$.
- Even though the electron is a point particle, we find that it has intrinsic *spin angular momentum*. Electrons are either $1/2$ or $-1/2$ and the magnitude of the angular momentum is $\sqrt{s(s+1)}\hbar = \sqrt{3}\hbar/2$.
- In general, the *g-factor* relates the angular momentum of a particle/atom to the magnetic moment. $$\boldsymbol\mu = g\cfrac{e}{2m}\textbf{S} = g\mu_Bm_s.$$
- Further, the energy of an electron in a magnetic field B is $$E=g\mu_Bm_sB.$$ This effect is called *Zeeman splitting*.
### 1.3.2 Pauli spin matrices and spinors

- The three *Pauli spin matrices* form an algebra $$\hat{\sigma}_x = \begin{pmatrix} 0 & 1\\  1 & 0 \end{pmatrix}, \quad \hat{\sigma}_y = \begin{pmatrix} 0 & -i\\  i & 0 \end{pmatrix}, \quad \hat{\sigma}_z = \begin{pmatrix} 1 & 0\\ 0&-1 \end{pmatrix}.$$ Let $\boldsymbol\sigma = (\hat{\sigma}_x. \hat{\sigma}_y, \hat{\sigma}_z).$
- If $$\textbf{a} = \begin{pmatrix}a_1\\a_2\\a_3\end{pmatrix},$$ then multiplying component-wise we have $$\boldsymbol\sigma \cdot \textbf{a} = \begin{pmatrix}a_3 & a_1-ia_2 \\ a_1 + ia_2 & -a_3\end{pmatrix}.$$
- Other properties include $$(\boldsymbol\sigma \cdot \textbf{a})(\boldsymbol\sigma \cdot \textbf{b}) = \textbf{a}\cdot\textbf{b} + i\boldsymbol\sigma\cdot(\textbf{a}\times\textbf{b})$$and $$(\boldsymbol\sigma \cdot \textbf{a})^2 = |\textbf{a}|^2.$$
- We define spin angular momentum operator as $$\hat{\textbf{S}} = \cfrac{1}{2}\hat{\boldsymbol\sigma}.$$where we have dropped the $\hbar$ from the operator. Note $$\hat{S}_x = \cfrac{1}{2}\hat{\sigma}_x, \quad \hat{S}_y = \cfrac{1}{2}\hat{\sigma}_y. \quad \hat{S}_z = \cfrac{1}{2}\hat{\sigma}_z.$$
- Each axis has it's own eigenstates that correspond the spin-up and spin-down states. *Spinor representation* represents the wave function as a combination of these two states $$|\psi\rangle = \begin{pmatrix}a \\ b\end{pmatrix} = a|\uparrow_z\rangle + b|\downarrow_z\rangle.$$ It is typical to normalize $a$ and $b$ such that $|a|^2 = |b|^2 = 1.$
### 1.3.3 Raising and lower operators

- Raising and lowering operators $$\begin{aligned} \hat{S}_+ = \hat{S}_x + i\hat{S}_y \\ \hat{S}_- = \hat{S}_x - i\hat{S}_y \end{aligned}$$ are not hermitian so do not correspond to observable but are still useful.
- Useful relations $$\begin{align} [\hat{S}_+,\hat{S}_-] = 2\hat{S}_z, \\ [\hat{S}_z,\hat{S}_\pm] = \pm\hat{S}_\pm \end{align}$$ and $$[\hat{\textbf{S}}^2,\hat{S}_\pm] = 0.$$
- Explicitly $$\begin{align}\hat{S}_+ = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}\\ \hat{S}_- = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix} \end{align}$$
- Note $$\hat{\textbf{S}}^2|\psi\rangle = \left(\hat{S}^2_x + \hat{S}^2_y + \hat{S}^2_z\right)|\psi\rangle = \left(\cfrac{1}{4} + \cfrac{1}{4} + \cfrac{1}{4}\right)|\psi\rangle =\cfrac{3}{4}|\psi\rangle.$$
### 1.3.4 The coupling of two spins

- Two spin-$1/2$ particles coupled by an interaction can be described by $$\hat{\mathcal{H}} = A\hat{\textbf{S}}^a \cdot \hat{\textbf{S}}^b$$ where $\hat{\textbf{S}}^a$ and $\hat{\textbf{S}}^b$ are the spin operators for the respective particles $a$ and $b$.
- For two spin-$1/2$ particles, the spin quantum number $s$ can become $0$ or $1$. $$s(s+1) = (\hat{\textbf{S}}_{\text{tot}})^2 = (\hat{\textbf{S}}_a)^2 + (\hat{\textbf{S}}_b)^2 + 2\hat{\textbf{S}}_a\cdot\hat{\textbf{S}}_b.$$Note that $s(s+1) can either be either $(0,2)$ if $s = (0,1)$, respectively.
- Since the eigenvalues of both $(\hat{\textbf{S}}_a)^2$ and $(\hat{\textbf{S}}_b)^2$ are $3/4$, we have that $$\hat{\textbf{S}}_a \cdot \hat{\textbf{S}}_b = \left(\frac{1}{4},-\frac{3}{4}\right)$$again with respect to $s = (0,1)$. 
- Looking back at the Hamiltonian equation, we see that there are two options for energy - $$E = \left(\frac{A}{4}, -\frac{3A}{4}\right).$$
- The degeneracy of each state is given by $2s+1$, counting $-s, -s+1, ..., s-1, s$. Hence, $s=0$ is the singlet state while $s=1$ is the triplet state.
#### 1.3.4.??? Symmetry and Antisymmetry
> Guys I need help

