# Week 2 - Integrals as Solutions

## Solving Differential Equations
When solving a differential equation, e.g. 

$$
\frac{dy}{dx}=5y
$$

our goal is to find a function $y(x)$ that satisfies the differential equation.

### Verifying Differential Equations
It is relatively straightforward to verify that a function is a solution to a differential equation. For example:

> Verify that $x(t)=sin(t)+cos(t)$ is a solution to the differential equation $\frac{dx}{dt}+x=2cos(t)$
>
> 1. Take the derivative of the proposed solution:
> $$
> \frac{d}{dt}(sin(t)+cos(t)) + (sin(t)+cos(t))\\
> = cos(t) - sin(t) + sin(t) + cos(t)\\
> = 2cos(t)
> $$
> 2. Thus, $x(t)$ is indeed a solution to the differential equation $\frac{dx}{dt}+x=2cos(t)$ because it satisfies the differential equation.

 ## Solving First Order Differential Equations
Some first order differential equations take the form $\frac{dy}{dx}=f(x)$ or $\frac{dy}{dx}=g(y)$. This type of differential equation is trivial to solve, by integrating both sides of the equation. For example:

> Solve the differential equation $y'=4x^3$
>
> 1. Integrate both sides: $\int y' dx = \int 4x^3 dx$
> 2. Therefore $y(x) = x^4+C$

The equation $y(x)=x^4+C$ is the general solution to this differential equation.

### Initial Conditions
Sometimes, an initial condition might be specified. This allows us to solve for $C$ and thereby arrive at a particular solution. For example:

> Solve the differential equation $y'=4x^3$ such that $y(0)=1$
>
> 1. Integrate both sides: $\int y' dx = \int 4x^3 dx$
> 2. Therefore $y(x) = x^4+C$
> 3. Evaluate the general solution at the condition: $y(0) = 1 = (0)^4 + C$
> 4. Solve for C: $C=1$
> 5. Thus the particular solution is $y(x)=x^4+1$

## Trivial Differential Equations
Consider equations of the form 
$$
\frac{dy}{dx}=f(y)
$$
where $f(y)=0$. In this case, the solution is trivial: $y(x)=C$.

If, however, $f(y)\neq 0$ then
$$
\int \frac{dy}{f(y)}=\int dx + C\\
= \int \frac{dy}{f(y)} = x + C
$$

For example:

> Consider $y'=5y$ such that $y(0)=2$. Find the particular solution.
>
> 1. Rewrite: $\frac{dy}{dt}=5y$
> 2. Rearrange: $\frac{dy}{y}=5 dt$
> 3. Integrate: $\int \frac{dy}{y} = \int 5 dt$
> 4. Solve:
> $$
> \ln|y|=5t+C\\
> \textrm{Exponentiate: }e^{ln|y|}=e^{5t+C}\\
> |y|=e^{5t}\cdot e^C\\
> \textrm{Observe } e^C \textrm{ is constant}\\
> |y|=Ce^{5t}\\
> \therefore y(t) = \pm Ce^{5t}
> $$
> 5. Using the initial condition, $y(0)=2=C\cdot 1 \implies C=2$