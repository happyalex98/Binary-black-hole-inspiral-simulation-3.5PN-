# Binary-black-hole-inspiral-simulation-3.5PN-
An interactive simulation of binary black hole merger events inspiral stage using post-Newtonian correction up to 3.5 term integrated with a Runge-Kutta 4 integrator

<img width="846" height="500" alt="스크린샷 2026-09-15 09 34 26" src="https://github.com/user-attachments/assets/b9815073-e5c6-4460-b987-c3a529611027" />

The simulation set up starts from placing the two black holes side by side with their center of mass between them. The gravitational forces between the black holes acts as the radial accelerations, which constantly changes both the magnitude and the direction of the velocity vectors. Runge-Kutta integrator is used to integrate the velocity and position vectors of the black holes.

<img width="846" height="529.41" alt="스크린샷 2026-09-15 09 38 49" src="https://github.com/user-attachments/assets/989bab1c-a543-4999-a5c3-85481ddfb101" />

We take small Δt to change the velocity and position accordingly. The gravitational force between inspiralling binary black holes is extremely strong that small Δt step and accurate integrator is necessary.

The gravitational acceleration of the black holes were calculated using post-Newtonian correction up to 3.5PN (0, 1, 2, 2.5, 3, 3.5PN) from Luc Blanchet's Gravitational Radiation from Post-Newtonian Sources and Inspiralling Compact Binaries[1]. 

We implemented Runge-Kutta 4 integrator whose global error scales as O(h^4).

References
[1] Blanchet, L. Gravitational Radiation from Post-Newtonian Sources and Inspiralling Compact Binaries. Living Rev. Relativ. 17, 2 (2014). https://doi.org/10.12942/lrr-2014-2
