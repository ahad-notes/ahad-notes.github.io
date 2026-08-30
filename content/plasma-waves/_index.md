---
title: "plasma waves"
---
*Textbook:
[Plasma Waves 2nd Edition by Gary Swanson](https://acrobat.adobe.com/id/urn:aaid:sc:US:7364d982-0977-4099-89bb-3284a89b9f60)*

*Solutions adopted from coursework in the University of Washington's AA 556 - Space and Laboratory Plasma Physics.*

**Some things I wish I grasped intuitively before ever starting to study plasma waves:**

> How do waves occur in plasmas? Well, a wave is governed by a restoring force, and in a plasma that restoring force may come from electric fields, magnetic tension, pressure gradients (like sound waves), or a combination of them. 

> A sinusoidal wave is usually written as $\propto e^{i(\mathbf{k} \cdot \mathbf{r} - \omega t)} $. $k = 2\pi / \lambda $ tells us the spatial scale and $\omega = 2\pi f$ tells us how fast the disturbance oscillates in time.

> The above assumption is so nice because the derivatives become simple multiplication - $\frac{\partial}{\partial t} \to -i \omega, \quad \nabla \to i k$. So differential equations like Maxwell's equations or fluid equations become algebraic equations.

> You will hear the term "dispersion relation" at a frequency of 1178263718236123187 Hz. It's just (not to marginalize it) an equation relating $\omega$ and $k$ via the form $D(\omega, k) =0$. It says: if you try to launch a disturbance with wavelength $2\pi / k$, these are the frequencies at which the plasma can naturally support it. A dispersion relation can have multiple roots where each root is a different physical wave branch. So ONE dispersion relation mathematical equation can therefore contain Langmuir waves, ion waves, electromagnetic waves, whistler waves, cyclotron modes, etc etc. 

> The shape of a $\omega (k)$ curve tells us a lot of physics. A flat branch means frequency barely depends on wavelength. A linear branch, like $\omega = vk$, describes a wave traveling at a constant speed. 

> Phase velocity is $v_{\phi} = \frac{\omega}{k}$ and it's the velocity of a wave crest. Group velocity is $v_g = \frac{d\omega}{dk}$ and it's the velocity of a wave packet and it's the velocity at which energy propagates. For an electromagnetic wave, the phase velocity can be larger than the group velocity which is the speed of light. In other words, we can only send information at the speed of light (obeying the laws of the universe), and not at a potentially faster phase velocity existing in the electric or magnetic field.

> A plasma is called dispersive when waves of different $k$ travel differently, meaning $\omega / k$ (phase velocity!) depends on $k$. Plasma waves are very often dispersive because the particles have natural frequencies and length scales.

> The electron plasma frequency $\left(\omega_{pe} = \sqrt{\frac{n_e e^2}{m_e \varepsilon_0}} \right)$ is the natural oscillation frequency of electrons against relatively stationary ions. If electrons are displaced slightly, charge separation creates an electric field that pulls them back. This process repeats to create an electron plasma frequency.

> The cyclotron frequency is $\omega_{c, s} = \frac{|q_s| B_0}{m_s}$ which is the natural gyrofrequency of a species $s$ around a magnetic field. Because electrons are much lighter, $|\omega_{c,e}| \gg |\omega_{c,i}|$.

> This immediately divides plasma wave physics into frequency regimes. For instance, at very low frequencies both ions and electrons can respond to the magnetic field. And at frequencies above $\omega_{ci}$, ions may no longer follow the oscillation well, while electrons still can.

> A magnetic field makes a plasma anisotropic. Parallel to $\mathbf{B_0}$, particle move relatively freely. Perpendicular to $\mathbf{B_0}$, their motion is constrained by gyromotion. Therefore, the angle between $k$ and $B_0$ changes the wave physics dramatically. 

> If $\mathbf{k} \parallel \mathbf{B_0}$, the wave propagates along the field. If $\mathbf{k} \perp \mathbf{B_0}$, it propagates across it. 

> The baseline plasma waves model is cold plasma theory, where the response of the plasma current from an applied electromagnetic perturbation is summarized by a dielectric tensor: $\mathbf{D} = \overset{\leftrightarrow}{\mathbf{\varepsilon}} \cdot \mathbf{E}$. It is a tensor rather than a scalar because magnetized plasma responds differently parallel and perpendicular to $\mathbf{B_0}$.

> The cold plasma dispersion relation (CPDR) is basically obtaining by considering the particle equation of motion, the current response (see bullet point above), and Maxwell's equations. We solve for which combinations of $\omega$, $k$, and polarization allow for a nonzero electromagnetic field. 

> Polarization tells us how the electric field oscillates. It might be linear, circular, or elliptical. In magnetized plasma, right-handed and left-handed circularly polarized waves behave different because charged particle themselves gyrate in a preferred direction. You will find plasma waves that will be left-handed and right-handed. 

> A strong interaction happens when the wave frequency appraoches a particle's natural gyrofrequency: $\omega ~ \omega_{c ,s}$. This is cyclotron resonance - the particle can repeatedly receive energy from the wave because the wave rotates at roughly the same rate as the particle. 

> A cutoff is a frequency below or above which a particular wave cannot propagate, usually giving imaginery $k$. Conversely, a resonance is where the plasma response becomes very large. Cutoffs and resonances are central features of cold plasma dispersion diagrams. 

> Now - fluids. A fluid description does not track individual particles, but replaces them with fields such as $n_s(\mathbf{x}, t)$ (species number density), $\mathbf{u}_s (\mathbf{x}, t)$ (species fluid bulk velocity), $P_s(\mathbf{x}, t)$ (species pressure). 

> The basic fluid equations are just conservation laws. Continuity says particles are conserved: $\frac{\partial n}{\partial t} + \nabla \cdot (n \mathbf{u}) = 0$.

> The fluid momentum equation is basically Newton's second law for a whole species: $m n \frac{d \mathbf{u}}{d t} = qn (\mathbf{E} + \mathbf{u} \times \mathbf{B}) - \nabla P$. Electric fields, magnetic fields, and pressure gradients accelerate the fluid. 

> Adding pressure introduces a new restoring mechanism. Density compression raises pressure, which pushes the plasma back outward. That's why thermal effects produce sound like plasma waves.

> Furthermore, ion-acoustic waves are basically sound waves for a plasma. The ions provide most of the inertia, while electron pressure provides much of the restoring force: $\omega = k c_s$. 

> You'll also hear about Alfvén waves a lot, which are magnetic-tensino waves. The magnetic field behaves kind of like a stretched string, and bending that field line creates magnetic tension, and plasma mass provides inertia via the Alfvén speed: $v_A = \frac{B_0}{\sqrt{\mu_0 \rho}}$, $\omega = k v_A$. 

> You'll find that a lot of the set up of our problems look something like this: $n = n_0 + n_1$, $\mathbf{u} = \mathbf{u}_0 + \mathbf{u}_1$, $\mathbf{E} = \mathbf{E}_0 + \mathbf{E}_1$. This is our equilibrium, where the subscript 1 quantities are small perturbations. And linearization means discarding products of small perturbations. For instance if $n_1$ and $u_1$ are both small then $n_1 u_1$ is second-order small and is neglected.

> The third description of plasmas we'll look into in our problem sets is the kinetic description, which replaces $n$, $\mathbf{u}$, $P$ with a distribution function $f(\mathbf{x}, \mathbf{v}, t)$. Instead of asking what's the average velocity? We ask how many particles have each velocity. 

> Density is recovered from kinetic theory by integration over velocity: $n= \int f d^3 v $. We can take moments of this to get fluid velocity and pressure. 

> The collisionless kinetic equation is the Vlasov equation: $\frac{\partial f}{\partial t} + \mathbf{v} \cdot \nabla f + \frac{q}{m} (\mathbf{E} + \mathbf{v} \times \mathbf{B}) \cdot \nabla_v f =0$. 

> Landau damping is a special physics derived from kinetic plasmas where, for instance in Maxwellian distribution, the wave transfers its energy into particles, causing the wave amplitude to decay even without collisions. 

> A kinetic dispersion relation often gives $\omega = \omega_r + i \gamma$. The real part $\omega_r$ is the oscillation frequency. The imaginary part tells you whether the wave grows or damps. $\gamma > 0$: instability, $\gamma < 0$: damping. 

> Plasma instabilities are basically waves that extract free energy from a non-equilibrium plasma. Some energy sources could be beams, temperature anisotropy, density gradients, currents, and velocity shear. 