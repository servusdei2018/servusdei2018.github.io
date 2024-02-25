# Sources of Electric Potential

An electric potential difference is created by separating positive and negative charges.

## Batteries

Batteries "lift" positive charges from the negative terminal to the positive terminal.

The work done to lift one charge is the EMF (electro motive force) whose units are volts:

$$
\epsilon = \frac{W_{chemical\ reactions}}{q}
$$

In ideal batteries, $\Delta V = \epsilon$ but in reality, $\Delta V < \epsilon$ however the difference is so small that in most cases, batteries may be considered ideal.

A battery may be represented by two parallel lines, one of which (the positive side) is longer than the other.

## Capacitors

A capacitor is any two separated charged conductors. It may be represented by two parallel lines of equal length.

A pair of electrodes charged with $\pm Q$ has a net charge of $0$ but there exists a potential difference $V_{cap}$ between the electrodes such that

$$
Q = CV
$$

where $C$ is capacitance. The SI unit of capacitance is the Farad, and $1F = 1\frac{C}{V}$.

## Equivalent Capacitance

Capacitors may be linked in parallel or in series. Capacitors thereby linked together may be represented by a single equivalent capacitance, or $C_{eq}$.

In parallel,

$$
C_{eq} = C_1 + C_2 + \cdots
$$

And in series,

$$
\frac{1}{C_{eq}} = \frac{1}{C_1}+\frac{1}{C_2}+\cdots
$$

## Solving Capacitor Circuit Problems

1. Write a **charge equation** for each net conductor (isolated portion of circuit). E.g. $Q_{eq}=Q_1+Q_2+Q_n$ or $Q_4=Q_3+Q_5$. Think about in vs out. Then place $+/-$ signs on each capacitor.

2. Write **voltage (loop) equations** by walking closed paths around the circuit. E.g. "$+V-V_1=0$" or "$+V-V_5-V_4=0$".

3. Write **connecting equations** for each capacitor ($q_1=V_1C_1$, etc.) and for the total charge ($q_{eq}=VC_{eq}$)

4. Solve the system of equations for the unknowns

## Energy Stored in a Capacitor

The energy stored in a capacitor is equal to

$$
U=\frac{1}{2}CV^2
$$

where $C$ is its capacitance and $V$ the voltage across the capacitor.

$U$ may also be rewritten as

$$
U=\frac{1}{2}\frac{Q^2}{C}
$$

## Dielectric Insulation

A dielectric, situated in an electric field, is a type of insulator. The term "dielectric" refers to the induced excess of positive and negative charges on each surface of the insulating material. This charge separation occurs due to the creation of a dipole induced by a parallel plate capacitor. When a dielectric is introduced into an electric field, it becomes polarized, and the induced dipole moment contributes to the material's ability to store electrical energy.

The dielectric constant $\kappa$ (kappa) represents the relative permittivity of a material. The dielectric constant is defined as the ratio of the electric field ($E_0$) in a vacuum to the electric field ($E$) in the material:

$$
\kappa \equiv \frac{E_0}{E}
$$

The dielectric capacitance is equal to

$$
C_{dielectric} = \kappa C_0
$$

where $C_0$ is the capacitance without the dielectric.