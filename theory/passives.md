# Passive IC Devices

## Resistance

Resistance calculation of metal or semiconductor material is fundamental to IC engineering.
Consider a block of metal or semiconductor material with dimensions $L, W$ and $h$. Let $n$ be the charge per unit volume.
To calculate the current $I_R$ for an applied voltage $V_R$ across the length of the material, we will consider an incremental cross section of the material with length $\Delta x$. 
The current can be written as the total charge in the incremental volume in time $\Delta t$: 

$I_R = \frac{\Delta Q}{\Delta t} = \frac{Q_S \Delta x}{\Delta t} = Q_S v_d$

$I_R = Sheet Charge \times Average Velocity$ or, 

where, $Q_S = nWh$ is the sheet-charge or the charge per unit length,

$v_d$ is the average velocity of the electrons:

$v_d= \frac{\Delta x}{\Delta t} = \mu E$, and 

where, $E = \frac{\Delta v}{\Delta x}$, and $\mu$ is the _mobility_ of the material.

Therefore, $I_R = \mu Q_S \frac{\Delta v}{\Delta x}$

The incremental resistance can be expressed as 

$\Delta R = \Delta v / I_R = \rho \Delta x/W$

where, $\rho = 1/(Q_S \mu)$ is the _Specific resistivity_ ($\rho$) is a property of the material that can be defined as the resistance per unit volume expressed in SI units of $\Omega m$ but more conveniently as $\Omega cm$. 

The total resistance of the volume can be found by summing up all incremental resistances $\Delta R$:

$R = \rho L/A$

where, $L$ is the length and $A$ is the cross-sectional area.

In integrated circuit design, the height of the metal routing is fixed and is typically in the range of $0.1$ to $5$ micrometers ($\mu m, 10^{-6} m)$ and the resistance is measured in square units as _ohms per square_ or $\Omega/\square$.

$R = (\rho/h) (L/W)$

Where, $\rho/h$ is typically called sheet-rho ($\rho_{sheet}$)

The specific resistance (in $\Omega cm$) and unit resistance (in $\Omega/\square$) of typical metals used in integrated circuits such as aluminum (Al), copper (Cu) and gold (Au) are tabulated:

| | $\mu -\Omega$ cm | $m\Omega/\square$ |
|----------|---------|---------|
| Al | 2.65 | 26.5 |
| Cu | 1.68 | 16.8 |
| Au | 2.44 | 24.4 |
