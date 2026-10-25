# UGACadathon26

*STEP file is in folder above.

## Inspiration

A car’s suspension faces different demands while driving. For example, it needs to be able to accommodate bumps and potholes while still being able to support stable cornering. An anti-roll bar allows one's vehicle to resist body roll, but it also couples the suspension’s response to uneven wheel inputs.

We wanted to mainly explore whether the connection to that bar could adapt mechanically, without sensors, motors, or electronic control, to reduce vibrations (for structural integrity) and enhance driver experience.

Our inspiration came from research on **countersnapping structures**: elastic networks that can suddenly contract under increasing tension. Researchers demonstrated that these networks can switch between configurations with different stiffnesses and, in laboratory experiments, passively escape resonance. We then asked: **could this behavior be applicable/incorporated into an automotive suspension?**

## What Our Project Does

Our concept replaces a conventional anti-roll-bar end link with a **countersnapping mechanism**, integrated into a MacPherson suspension assembly.

Suspension-induced loading can trigger a change in the mechanism’s internal configuration. This changes its tangent stiffness—the resistance it provides to small additional movements:

$$
k_t=\frac{dF}{du}
$$

Changing stiffness can shift the natural frequency of a participating vibration mode. For a simplified single-degree-of-freedom model:

$$
f_n=\frac{1}{2\pi}\sqrt{\frac{k_{\mathrm{eff}}}{m_{\mathrm{eff}}}}
$$

Our goal is to investigate whether this shift can move the suspension away from repeated excitation that amplifies vehicle motion, particularly during uneven-road cornering.

## How We Built It

We began with a literature review of countersnapping, switchable stiffness, and passive vibration isolation. We then developed hand sketches to translate the published mechanism into an automotive end-link concept.

The elastic network combines five functional elements:

- Two softening elements.
- Two stiffening elements.
- One nonmonotonic element that enables instability-driven switching.

We developed CAD models of the mechanism, connectors, and integration into a right-front MacPherson suspension assembly. Assembly views, cross-sections, and exploded drawings helped us examine packaging and explain the internal load paths.

For the proposed metallic mechanism, we selected **17-7 PH stainless spring strip in condition CH900** as our initial material candidate. Computational validation would have to remain the next stage; nonlinear structural analysis will characterize the mechanism, followed by MATLAB/Simulink evaluation of its suspension response.

## What We Learned

We learned that adaptive mechanical behavior can come from geometry rather than electronics. Combining elastic elements with different force–displacement responses can create behavior that none provides alone.

We also learned that stiffness switching and damping perform different roles. Our mechanism changes elastic resistance; the existing shock absorber remains responsible for dissipating energy.

Most importantly, a promising material behavior must be evaluated within the complete system. A large stiffness change inside the cartridge may produce a smaller change in the suspension because the anti-roll bar and surrounding components also contribute compliance.

## Challenges We Faced

Our biggest challenge was translating a laboratory mechanism into a realistic suspension connection. Packaging, articulation, load direction, and available travel all affect whether the mechanism can switch as intended.

Tension and compression also require separate evaluation. A mechanism that countersnaps under tension cannot automatically be assumed to behave identically under compression.

We approached these challenges by defining a focused integration concept and a validation path. The result is a research-driven CAD design with a clear question to test: **can passive countersnapping provide useful adaptive stiffness in an automotive application for suspension end links?**



