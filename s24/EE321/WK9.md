# Week 9

## LTI Circuits

Because [L]inear, [T]ime-[I]nvariant circuits possess these properties, then if

$$
x(t) = a_1x_1(t-t_1)+a_2x_2(t-t_2)+\cdots
$$

then it follows from its linearity that a system's response to an input $x(t)$ is

$$
y(t) = a_1y_1(t-t_1)+a_2y_2(t-t_2)+\cdots
$$

## Convolution

Convolution is a mathematical operation on two functions (e.g. $x(t)$ and $h(t)$) that produces a third function $y(t) = x(t) \mathord{*}h(t)$. Intuitively, convolution represents the amount of overlap between two functions.

We define convolution to be equal to the integral

$$
y(t) = x(t) \mathord{*}h(t) = \int_{-\infty}^{\infty}x(\tau)h(t-\tau)d\tau
$$

and, vice versa,

$$
y(t) = h(t) \mathord{*}x(t) = \int_{-\infty}^{\infty}h(\tau)x(t-\tau)
d\tau
$$

## Properties of Convolution

- Commutative: $ f\mathord{*}g = g\mathord{*}f $
- Associative
- Distributive