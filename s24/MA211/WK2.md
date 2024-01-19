# Week 2 - Symbolic Logic

## Logical Symbols
- $\sim$ not (also $\lnot$)
- $\land$ and
- $\lor$ or
- $\equiv$ equivalent
- $\not\equiv$ not equivalent

## Truth Table
| P | ~P |
| - | -- |
| T | F  |
| F | T  |

## de Morgan's Laws
1. $\lnot(P\land Q) \equiv \lnot P\lor \lnot Q$
2. $\lnot(P\lor Q) \equiv \lnot P\land \lnot Q$

## Tautology
- A tautology is a statement that is always true. E.g. $P\lor \lnot P$

## Contradiction
- A tautology is a statement that is always false. E.g. $P\land \lnot P$

## Conditional Statements

$P \leadsto Q$ "if P then Q"

#### Truth Table
| P | Q | $P\leadsto Q$ |
| - | - | - |
| T | T | T |
| T | F | F |
| F | T | T |
| F | F | T |

## Negation

Notice this statement is only false when hypothesis is true and conclusion is false. This is *vacuously true*, or true by default.

E.g.
| P | q | $P \land \lnot Q$ | $P\land \lnot Q \leadsto \lnot P$ |
| - | - | - | - |
| T | T | F | T |
| T | F | T | F |
| F | T | F | T |
| F | F | F | T |

### Representation of if-then ($\leadsto$) in terms of $\lor$

**Important** Claim: $p\leadsto q \equiv \lnot p \lor q$

#### Negation of $p \leadsto q$, i.e. $\lnot(p \leadsto q)$

$$
\lnot(p \leadsto q) \equiv \lnot(\lnot p \lor q)\\
[\lnot(A \lor B)\equiv \lnot A \land \lnot B]\\
\equiv \lnot(\lnot p) \land \lnot q\\
\equiv p \land \lnot q
$$

i.e. $\lnot(p\leadsto q)$ is $p\land \lnot q$.

## Negation

For example:

> Negate: if x>2 then x>1
> $$\lnot(x>2 \leadsto x>1)\\
> \equiv x>2 \land x \leq 1
> $$

Or:

> Negate" if n is prime then n>1
> $$\lnot(\textrm{n is prime }\leadsto n>1)\equiv \textrm{n is prime } \land n \leq 1$$

Or:

> Negate: if n is prime then n > 1 and n has no divisors other than 1 and itself
> $$\lnot(\textrm{statement above}) \equiv \textrm{n is prime and n }\leq 1\textrm{ or n has a divisor other than itself and 1}$$

Also: $A\land (B\lor C) \equiv (A \land B)\lor(A\land C)$

## Contrapositive
Given $p\leadsto q$, $\lnot q \leadsto \lnot p$

E.g. "if it snows tonight, then I will be unhappy"

Contrapositive: If I will be happy, then it will not snow tonight.

## Converse
Given $p\leadsto q$, $q\leadsto p$

E.g. "if it snows tonight, then I will be unhappy"

Converse: If I will be unhappy, then it will snow tonight.

## Inverse
Given $p\leadsto q$, $\lnot p \leadsto \lnot q$

E.g. "if it snows tonight, then I will be unhappy"

Inverse: If it does not snow tonight, then I will be happy.

## Examples

> 1. If $\det A \neq 0$ then $A$ is invertible
- Contrapositive: If $A$ is not invertible, then $\det A = 0$
- Converse: If $A$ is invertible then $\det A \neq 0$
- Inverse: If $\det A=0$ then $A$ is not invertible

## Two Important Claims
- Note that $p\leadsto q\equiv\lnot q \leadsto\lnot p$
- Additionally, $q\leadsto p\equiv\lnot p\leadsto\lnot q$.

## Conditions

- Necessary Condition: $p$ is necessary for $q$ means $\lnot p\leadsto\lnot q \equiv q\leadsto p$
- Sufficient Condition: $p$ is sufficient for $q$ means $p\leadsto q$
- Biconditional: $p \iff q$ reads "$p$ if and only if $q$" means $(p\leadsto q)\land(q\leadsto p)$ or $p \iff q$.

P is necessary and sufficient for q means $p\iff q$.

## Modus Ponens

1. $p\leadsto q$
2. $p$
3. $\therefore q$

### Truth table for Modus Ponens
| $p$ | $q$ | $p\leadsto q$ (premise 1) | $p$ (premise 2) | $q$ (conclusion) |
| - | - | - | - | - |
| T | T | T | T | T |
| T | F | F | T | F | 
| F | T | T | F | T |
| F | F | T | F | F |

the first row in the truth table is called the **critical row**.

Invalid (converse error): $p\leadsto q$, $q$, $\therefore p$. This is a fallacious syllogism.

## Modus Tollens
1. $p\leadsto q$
2. $\lnot q$
3. $\therefore\lnot p$

*Modus tollens* is the contrapositive of *modus ponens*.

> E.g.:
> 1. If I'm tall then I wear socks
> 2. I don't wear socks
> 3. Therefore I am not tall

Fallacy (Inverse Error):
1. $p\leadsto q$
2. $\lnot p$
3. $\therefore\lnot q$

> E.g.:
> 1. If $n>2$ then n is positive
> 2. $n\leq 2$
> 3. $\therefore n$ is not positive

## Generalization
1. $p$
2. $\therefore p\lor q$

OR

1. $q$
2. $\therefore p\lor q$

Such that the truth trable is

| $p$ | $q$ | $p\lor q$ |
| - | - | - |
| T | T | T |
| F | T | T |
| T | F | T |
| F | F | F |

## Specialization

1. $p\land q$
2. $\therefore p$

OR

1. $p\land q$
2. $\therefore q$

Worded as "we have P and Q therefore we have P;" or, vice versa.

## Elimination

1. $p\lor q$
2. $\lnot q$
3. $\therefore p$

OR

1. $p\lor q$
2. $\lnot p$
3. $\therefore q$

> E.g.
> 1. $p\lor q\lor r$
> 2. $\lnot q\land\lnot r$
> 3. $\therefore p$

## Transitivity

1. $p\leadsto q$
2. $q\leadsto r$
3. $\therefore p\leadsto r$

> E.g.
> 1. If I am home on Saturday I will be bored
> 2. If I'm bored on Saturday then I will eat pizza
> 3. Therefore if I'm home on Saturday then I will eat pizza

## Division into Cases
1. $p\lor q$
2. $p\leadsto r$
3. $q\leadsto r$
4. $\therefore r$

## Contradiction Rule
1. $\lnot p\leadsto c$
2. $\therefore p$

where $c$ is a contradiction (always-false).

| $p$ | $\lnot p\leadsto c$ | $p$ (conclusion) |
| - | - | - |
| T | F |
| F | T |

(not p -> c is false when the statement p is true, because a conditional is false when the premise is true and the conclusion is false)

> E.g.
> Claim: $\pi+1$ is irrational
> Proof:
> 1. Suppose *by way of contradiction* (BWOC) that $\pi + 1$ is rational
> 2. Since $\pi +1$ is rational, we can find two integers $m$ and $n$ such that $\pi +1=\frac{m}{n}$.
> 3. Then it's the case that $\pi=\frac{m}{n}-1=\frac{m-n}{n}$ so it's the case that $\pi$ is rational
> 4. Hence, by this contradiction is proven that $\pi +1$ is irrational