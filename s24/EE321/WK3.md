# Week 3 - Basic Impulse and Unit Functions

## The Unit Step Function
The continuous-time unit step function $u(t)$ is defined as:

$$
u(t)={\begin{cases}1,&t\geq 0\\0,&otherwise\end{cases}}
$$

- Discontinuous at $t=0$
- Differentiation:

$$
\frac{du}{dt}={\begin{cases}0,&t\neq 0\\\infin,& t=0 \end{cases}}
$$

### Operations with the Unit Step Function

- Time Shift:

$$
u(t-t_0) = {\begin{cases}1,&t\geq t_0\\0,&otherwise\end{cases}}
$$

- Time-limited Pulse

$$
p(t)=u(t)-u(t-t_0)
$$

- - This pulse has finite energy
- - It has many applications, e.g. binary transmission 