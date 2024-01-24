# Week 2 - Background Material

## Review of Complex Numbers

A complex number $z$ may be represented in Cartesian/rectangular form as

$$
z=a+jb
$$

where $a$ is called the *abscissa* and $b$ the *ordinate*. $a$ is the real part of $z$, and is denoted as $\Re(z)$; $b$ is the imaginary part of $z$ and is denoted $\Im(z)$.

### Polar Coordinates
If $(r,\theta)$ are the polar coordinates of $z=a+jb$ then

$$
a=rcos(\theta)\\
b=rsin(\theta)
$$

Consequently, 

$$
z=a+jb=r(cos(\theta)+jsin(\theta))
$$

### Euler's Formula

$$
e^{j\theta}=cos(\theta)+jsin(\theta)
$$

thus, 

$$
z=re^{j\theta}
$$

### Reciprocal of a Complex Number
The reciprocal of a complex number is given by $\frac{1}{z}=\frac{1}{r}e^{-j\theta}$.

### Conjugate of a Complex Number
The conjugate of a complex number is given by $z^*=re^{-j\theta}$.

- Observe $z^*$ is a mirror of $z$ about the horizontal axis.
- To find the conjugate of any number, we need only replace $j$ with $-j$ in that number.

### Properties of the Conjugate
- The sum of a complex number and its conjugate is a real number equal to twice the number's real part:

$$
z+z^* = 2a = 2\Re(z)
$$

- Thus, the real part of a complex number may be found thus:

$$
\Re(z)=\frac{z+z^*}{2}
$$

- Similarly, the imaginary part of a complex number may be found by

$$
\Im(z)=\frac{z-z^*}{2j}
$$

- The prouct of a complex number $z$ and its conjugate is the square of the number's magnitude:

$$
z\cdot z^*=|z|^2
$$

### Computing Angles w/ Calculators
When computing the angle of a complex number using $tan^{-1}
$, the calculator will return a valid result in the first and fourth quadrants. If the angle appears in the second or third quadrants, the correct answer is arrived at by adding or subtracting $180\degree$ to the output. 

### Arithmetical Operations on Complex Numbers
To add and subtract complex numbers, convert into Cartesian form and add the Real and Imaginary components separately. The remainder of the operations may be performed in either Cartesian form or polar form; polar form is generally easier.

#### Multiplication

$$
z_1z_2=r_1r_2e^{j(\theta_1+\theta_2)}
$$

#### Division

$$
\frac{z_1}{z_2}=\frac{r_1}{r_2}e^{j(\theta_1-\theta_2)}
$$

#### Exponentiation

$$
z^n=r^ne^{jn\theta}
$$

and

$$
z^{1/n}=r^{1/n}e^{j\theta/n}
$$

## Review of Linear Algebra

### Matrix Multiplication
- Given matrices $\bf A_{mn}$ and $\bf B_{np}$, with A's columns equalling B's rows $m=p$. 
- The resulting matrix $\bf C_{nm}$ has the same number of rows as $\bf A$ and the same number of columns as $\bf B$.
- With each element of C such that:

$$
C_{ij}
=
\sum _{k=1}^{n}a_{ik}b_{kj}
$$

E.g.

$$
{\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}}
{\begin{bmatrix}7&8\\9&10\\11&12\end{bmatrix}}
=
{\begin{bmatrix}58&64\\139&154\end{bmatrix}}
$$

where $58 = (1,2,3)\cdot(7,9,11)$, $64 = (1,2,3)\cdot(8,10,12)$, etc.

It is important to note that in matrix multiplication, the **commutative property does not hold.** That is, $AB\neq BA$

### Determinants
The determinant of a $2\times 2$ matrix is

$$
{\begin{vmatrix}a&b\\c&d\end{vmatrix}}
=
ad-bc
$$

- The determinant of the $2\times 2$ identity matrix is 1
- The determinant is 0 if both rows are the same: 

$$
{\begin{vmatrix}a&b\\a&b\end{vmatrix}}=ab-ba=0
$$

The determinant of a $3\times 3$ matrix is

$$
{\begin{vmatrix} a&b&c\\d&e&f\\g&h&i\end{vmatrix}}=
a{\begin{vmatrix} e&f\\h&i\end{vmatrix}}+
b{\begin{vmatrix} d&f\\g&i\end{vmatrix}}+
c{\begin{vmatrix} d&e\\g&h\end{vmatrix}}
$$

### Identity Matrix
The identity matrix is a square matrix that has ones along the main diagonal and zeros elsewhere.

E.g.

$$
{\begin{bmatrix}1&0\\0&1\end{bmatrix}}
$$

- The identity matrix $I$ has the special property that $A\cdot I = I\cdot A = A$

### Eigenvectors & Eigenvalues
Given $A\cdot v=\lambda \cdot v$ where $A$ is a $n\times n$ matrix, $v$ is a non-zero vector in the $n$-th dimension, and $\lambda$ is scalar; any value of $\lambda$ for which this equation has a solution is an eigenvalue and $v$ its eigenvector.


Proceeding from the first equation, we may arrive thus:

$$
A\cdot v=\lambda\cdot v\\
A\cdot v-\lambda\cdot v=0\\
A\cdot v-\lambda\cdot v\cdot I=0\\
v(A-\lambda\cdot I)=0\\
$$

If $v$ is non-zero, this equation only has a solution if 

$$
|A-\lambda\cdot I|=0
$$

This is called the **characteristic equation** of $A$ and is a monic polynomial of degree $n$; ergo, it has at most $n$ roots which are the eigenvalues of $A$. 

For each eigenvalue $\lambda$ is a corresponding eigenvector. To find the eigenvector, each eigenvalue may be transferred into the equation $v(A-\lambda\cdot I)=0$, the matrix $A-\lambda\cdot I$ evaluated, and then the eigenvector $v$ deduced therefrom.

## The Unit Impulse

### The Dirac Delta
The unit impulse function (also known as the Dirac delta) is defined as $\delta(t)=0$ iff $t\neq 0$, or equivalently:

$$
{\displaystyle \delta (t)\simeq {\begin{cases}+\infty ,&t=0\\0,&t\neq 0\end{cases}}}
$$

which is constrained to satisfy the identity

$$
\int_{t=-\infin}^{\infin}{\delta(t)\,dt=1}
$$

The Dirac delta function is an example of a *continuous-time* signal; for, it is specified for every value of $t$.

### The Kronecker Delta
The discrete-time impulse function (also known as the Kronecker delta) serves as the discrete-time counterpart to the continuous-time Dirac delta function and is defined thus:

$$
\delta[n]={\begin{cases}1 ,&n=0\\0,&n\neq 0\end{cases}}
$$

A *discrete-time* signal is specified only at discrete values of time. Ordinarily, the independent variable for discrete-time signals is represented by the integer $n$. Here, $n$ takes integer values and for a discrete-time signal $x[n]$, $x[n]$ denotes the $n$-th number in said sequence. Fundamentally, a discrete-time signal is a sequence of numbers, and may arise as a result of sampling continuous-time signals in sampled data systems and digital filtering.

### Scaled Impulse
The unit impulse function may be scaled to some height $A$ through multiplication:

$$
\int_{-\infin}^{\infin}{A\delta(t)\,dt}=A\int_{-\infin}^{\infin}{\delta(t)\,dt}=A(1)=A
$$

Additionally, the unit impulse may be mirrored across the horiontal axis by changing the sign of the impulse:

$$
\int_{-\infin}^{\infin}{-\delta(t)\,dt}=-1
$$

### Time Shifted Impulse
The unit impulse function may be shifted, either to the left or right, by some value $t_0$:

$$
\delta(t\pm t_0)
$$

## Properties of the Unit Impulse

As previously mentioned, the integral of the unit impulse $=1$. We may express this more generally:

$$
\int_{a}^{b}{\delta(t)\,dt}={\begin{cases}1 ,&a<0<b\\0,&otherwise\end{cases}}
$$

That is, the integral of the unit impulse *across a region including the origin* (where the impulse lies) is 1, and 0 otherwise.

We may likewise express a time-shifted impulse as

$$
\int_{a}^{b}{\delta(t-\lambda)\,dt}={\begin{cases}1 ,&a<\lambda<b\\0,&otherwise\end{cases}}
$$

Let us now consider the integral of a function $f(t)$ product of the impulse $\delta(t)$ at the origin:

$$
\int_{-\infin}^{\infin}{\delta(t)\cdot f(t)\, dt}
$$

We may simplify this integral to

$$
\int_{-\infin}^{\infin}{\delta(t)\cdot f(0)\, dt}
$$

because the impulse is $0$ for $t\neq 0$. This is especially significant: for, it allows us to replace the product of two functions with the product of a function and a constant $f(0)$.

Factoring the constant $f(0)$ out of our integral, we end up with a scaled impulse

$$
f(0)\cdot\int_{-\infin}^{\infin}{\delta(t)\,dt}
$$

which $=f(0)$.

### Sifting Property

From the above discussion, it follows that

$$
\int_{a}^{b}{\delta(t)\cdot f(t)\,dt}={\begin{cases}f(0) ,&a<0<b\\0,&otherwise\end{cases}}
$$

And for a time-shifted impulse:

$$
\int_{a}^{b}{\delta(t-\lambda)\cdot f(t)\,dt}={\begin{cases}f(\lambda) ,&a<
\lambda<b\\0,&otherwise\end{cases}}
$$

This property of the unit impulse is known as the **sifting property**. That is, the impulse function "sifts" through the function $f(t)$ and pulls out the value $f(0)$ or, for a time-shifted impulse, $f(\lambda)$.
