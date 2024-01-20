# Week 2 - Review of Linear Algebra

## Matrix Multiplication
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

### Determinants
The determinant of a $2\times 2$ matrix is

$$
{\begin{vmatrix}a&b\\c&d\end{vmatrix}}
=
ad-bc
$$

- The determinant of the $2\times 2$ identity matrix is 1
- The determinant is 0 if both rows are the same: $${\begin{vmatrix}a&b\\a&b\end{vmatrix}}=ab-ba=0$$

### Identity Matrix
The identity matrix is a square matrix that has ones along the main diagonal and zeros elsewhere.

E.g.

$$
{\begin{bmatrix}1&0\\0&1\end{bmatrix}}
$$

- The identity matrix $I$ has the special property that $A\cdot I = I\cdot A = A$

## Eigenvectors & Eigenvalues
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

For each eigenvalue $\lambda$ is a corresponding eigenvector. To find the eigenvector, each eigenvalue may be transferred into the equation $v(A-\lambda)=0$, the matrix $A-\lambda$ evaluated, and then the eigenvector $v$ deduced therefrom.

## Matrix Division

$P/Q \equiv PQ^{-1}$

Suppose given $Ax=B$ we wish to find $x$.

$A^{-1}Ax=A^{-1}B\\Ix=A^{-1}B \implies \textrm{solution for }x$


### Cramer's Rule

Let $\Delta = |A|$, $\Delta_1=|A_1|$ replace 1st column of $A$ with $B$, $...$, $\Delta_n = |A_n|$ replace $n$ -th column of A with B.

## Other (see also)
- Matrix rank
- Matrix normalization
- Condition number

## Impulses

### The Unit Impulse (Dirac Delta)
$$
{\displaystyle \delta (x)\simeq {\begin{cases}+\infty ,&x=0\\0,&x\neq 0\end{cases}}}
$$
which is constrained to satisfy the identity
$$
\int_{t=-\infin}^{\infin}{\delta(t)\,dt=1}
$$

Note that $\partial(t) = 0 \textrm{ if } t\neq 0$.

### The Unit Impulse (Kronecker Delta)

### Scaled Impulse
$$
\int_{-\infin}^{\infin}{A\delta(t)\,dt}=A\int_{-\infin}^{\infin}{\delta(t)\,dt}=A(1)=A
$$

### Time Shifted Impulse
$$

$$

## Properties of the Unit Impulse

#### Sifting Property
(see also https://lpsa.swarthmore.edu/BackGround/ImpulseFunc/ImpFunc.html#sifting)

$$
x(t)\delta (t-t_0)=x(t_0)\delta(t-t_0)
$$