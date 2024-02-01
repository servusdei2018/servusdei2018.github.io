# Week 4

## Periodic Pulses

A periodic pulse has the general equation

$$
x(t+T)
$$

## Sinusoidal Signals

$$
sin(\omega_0t)=sin(2\pi f_0t)=sin(2\pi\frac{t}{T_0})
$$

where $\omega=2\pi f_0=2\pi\frac{t}{T_0}$ is the angular velocity, and $f_0$ is the linear frequency.

A sinusoidal signal may be expressed in terms of cosine such that

$$
cos(\omega_0t)=cos(2\pi f_0t)=cos(2\pi\frac{t}{T_0})
$$

whose graph is shifted to the left/right of sin by $\frac{\pi}{2}$ (sin has a peak at $\frac{\pi}{2}$, cos has a peak at $0$).

## Phase Shifted Cosine

$$
x=A\,cos(\omega_0+\phi)
$$

where $T_0=\frac{2\pi}{\omega_0}$

## Truncated Signal

A signal may be truncated by multiplying it by a pulse. The resulting signal is defined within the window bounded by the pulse.

## Sinc Function

The $sinc()$ function is defined as

$$
sinc(t)=\frac{sin(t)}{t}
$$

It is important to note that $sinc(0)=1$, for 

$$
\lim_{t\to 0} sin(t)=t
$$

therefore

$$
\lim_{t\to 0} \frac{sin(t)}{t}=\lim_{t\to 0}\frac{t}{t}=1
$$

- We shall later see that $sinc()$ and the rectangular pulse are related through the Fourier transformation.