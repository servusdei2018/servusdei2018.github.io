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
- Note that sinc is 0 at $t=n$-th values of $\pi$.

### Sketching $sin(\omega_0(t-t_0))$

- First crossing at $t=t_0$
- For $sin(\omega_0 t-\omega_0 t_0)$, $w_0 t_0$ is constant and the phase shift.
- $w_0 t$=$n\pi$, thus $t=\frac{n\pi}{\omega_0}$. The spacing between crossings therefore is $\frac{\pi}{\omega_0}$.

## Exponentials

Exponential signals take the form

$$
x(t)=Ae^{\beta t}
$$

- When $\beta>0$, the signal is increasing
- When $\beta<0$, the signal is decreasing
- When $t=0$, we have our y-intercept at $y=A$.

### Multiplying Signals with Exponentials

- Growing sinusoid: $x(t)=Ae^{\Beta t}cos(\omega_0 t),\, \beta >0$
- Decaying sinusoid:  $x(t)=Ae^{\Beta t}cos(\omega_0 t),\, \beta <0$

## Complex Exponentials / Complex Sinusoids

From Euler's formula, we have

$$
re^{j\omega_0 t}=r[cos(\omega_0 t)+jsin(\omega_0 t)]\\
Re[re^{j\omega_0 t}=rcos(\omega_0 t)\\
Im[re^{j\omega_0 t}=rsin(\omega_0 t)]
$$

Magnitude and phase:
$$
|re^{j\omega_0 t}|=|r|\sqrt{cos(\omega_0 t)^2+sin(\omega_0 t)^2}=r\\
\angle{re^{j\omega_0 t}}=arctan(\frac{rsin(\omega_0 t)}{rcos(\omega_0 t)})=\omega_0 t
$$

### Operations on Complex Sinusoids

The conjugate of a complex sinusoid is:

$$
(e^{j\omega_0 t})^*=e^{-j\omega_0 t}=cos(\omega_0 t)-jsin(\omega_0 t)\\
Re[conj]=cos(\omega_0 t)\\
Im[conj]=-sin(\omega_0 t)\\
|conj| = 1\\
\angle{conj}=-\omega_0 t
$$