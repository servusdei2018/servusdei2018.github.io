# Week 5

## Operations on Signals

- Signal Addition
- Time Reversal
- - Reflects about $t=0$
- Time Scaling
- - Compared to the graph of $x(t)$, $x(2t)$ twice as twice as narrow and $x(t/2)$ is twice as wide

## Precedence of Time-Shift, Reflection and Scalling

### Method I - Parenthesis Method

1. Express $x(at+b)$ as $x(a(t+b/a))$
2. Apply scaling (and reflection, if $a$ is negative), by the factor $a$
3. Apply the time-shift by the factor $\frac{b}{a}$

### Method II - Direct Method

1. Start with $x(at+b)$
2. Apply the time-shift factor $b$
3. Apply scaling (and reflection, if $a$ is negative) by the factor $a$

## Even and Odd Symmetry

### Even Symmetry

$$
x(t)=x(-t)
$$

### Odd Symmetry

$$
x(t)=-x(-t)
$$

- For an odd function, $f(-x)=-f(x)$

## Rewriting Signals using Symmetry

Any signal may be separated into even and odd components

$$
x_{even}(t)=\frac{1}{2}\left[ x(t)+x(-t) \right]\\
x_{odd}(t)=\frac{1}{2}\left[ x(t)-x(-t) \right]
$$

- Signals may neither be even nor odd, yet possess even and odd components.
- In that case, $x_{even}+x_{odd}=x(t)$
