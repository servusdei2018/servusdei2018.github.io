# Week 1 - Introduction to Differential Equations

## General Solutions for Four Fundamental Equations  
1. $\frac{dy}{dx}=ky$ for some constant $k > 0$. This equation's general solution is $$y(x)=Ce^{kx}$$

2. $\frac{dy}{dx}=-ky$ for some constant $k > 0$. This equation's general solution is $$y(x)=Ce^{-kx}$$

3. $\frac{d^2y}{dx^2}=k^2y$ for some constant $k>0$. This equation's general solution is $$y(x)=C_1e^{kx}+C_2e^{-kx}=D_1cosh(kx)+D_2sinh(kx)$$

4. $\frac{d^2y}{dx^2}=-k^2y$ for some constant $k>0$. This equation's general solution is $$y(x)=C_1cos(kx)+C_2sin(kx)$$

## The Differential Equation
A differential equation is an equation that involves the derivative(s) of an unknown function. A solution to a differential equation is a function that satisfies the equation.

## Classification of Differential Equations
- *Ordinary differential equations* (ODE) are equations where the derivatives are taken with respect to only one variable; i.e., there is only one independent variable.
- *Partial differential equations* (PDE) are equations that depend on partial derivatives of several variables; i.e., there are several independent variables.

### Order
- An equation or system of equation's order is the order of the largest derivative contained therein.

### Linear
- An equation is linear if the dependent variable(s) and their derivatives appear linearly, that is, only as first powers, they are not multiplied together, and no other functions of the dependent variables appear.
- Linear ODEs may be put in the form $$a_n(x)\frac{d^ny}{dx^n}+a_{n-1}(x)\frac{d^{n-1}y}{dx^{n-1}}+\ldots+a_1(x)\frac{dy}{dx}+a_0(x)y=b(x)$$ where the functions $a_0\ldots a_n$ are called the coefficients. Note that $y$ and its derivatives only appear linearly.
- If the coefficients of a linear equation are constant functions, the equation is said to have constant coefficients.

### Homogenous
- A linear equation is homogenous if all terms depend on the dependent variable; i.e., if no term is a function of the independent variable(s) alone.
- Otherwise, it is nonhomogenous.

### Atonomous
- An equation or system of equations is called autonomous if it does not depend on the independent variable.