# Week 8

## Systems

A system is a process that transforms input signal(s) into output signal(s).

### Example of a Discrete Time Signal

- Investment account
- Interest compounded monthly ($\delta$%)
- Possible deposit each month

$$
y(n)-\left(1+\frac{\delta}{100}\right)y(n-1)=x(n)
$$

## Properties of Systems

- Memory
- Invertibility
- Causality
- Stability
- Time Invariance
- Linearity

Most systems covered in EE321 are LTI systems (linear time-invariant). We want all systems to be LTI, causal, stable, and invertible.

## Memory

- Memoryless System
- - Output at a given time depends only on inputs at that given time
- - $y(n) = 8[x(n)+2x^3(n)]$

- System With Memory
- - Output depends on previous inputs
$$
y(t)=\frac{1}{C}\int_{-\infty}^{t}{x(t)dt}\\\ \\
y(n)=\frac{1}{L}\sum_{k=0}^{L-1}{x(n-k)}
$$

## Invertibility

A system $h(\cdot)$ is invertible if it is possible to create a system $h_1(\cdot)$ such that

$$
x(\cdot)\rarr [h(\cdot)]\rarr y(\cdot)\rarr [h_1(\cdot)]\rarr w(\cdot)=x(\cdot)
$$

- $y(t)=3x(t)$ hence $w(t)=h_1(y(t))\implies h_1(3x(t))=x(t) \implies w(t)=\frac{y(t)}{3}=x(t)$
- $y[n]=x^4(n)$ is non invertible

## Causality

Outputs of causal systems depend on **current and past** values of inputs only.
- Most real systems are causal
- All memoryless systems are causal

Examples of non-causal systems:

1. $y(t)-2y(t-1)=x(t+2)$
2. $y[n]=\frac{1}{2N+1}\sum_{k=-N}^{N}{x[n-k]}$

## Stability

A signal is stable if it produces bounded outputs for all bounded inputs. A signal $x(t)$ is bounded if for some $M\lt\infty, |x(t)|\leq M$ for all $t$.

- For $n\geq 0$, $y(n)=0.8^nx(n)$, $0.8^n \leq 1$. If $|x(n)|=B<\infty$ then $y(n)\leq B$
- For $n\geq 0$, $y(n)=1.1^nx[n]$, $1.1^n\rarr\infty$ thus this $y(n)$ is not stable.

## Time Invariance

A system whose characteristics do not change over time is time invariant. A system is time-invariant if

$$
x(t) \rarr y(t) \implies x(t-t_0) \rarr y(t-t_0)\\
x[n] \rarr y[n] \implies x[n-n_0] \rarr x[n-n_0]
$$

Verify whether the following systems are time invariant (TI) or time variant (TV):

1. $y(t)=cos[x(t)]$ 
2. $y(t)=3x(t)$
3. $y(n)=(n+1)x(n)$
4. $y(t)=x(3t)$

## Linearity

A function is linear if it has these properties:

1. Homogeneity (scaling): $f(ax)=af(x)$
2. Additivity: $f(x_1+x_2)=f(x_1)+f(x_2)$

These two properties together are known as the **principle of superposition.**