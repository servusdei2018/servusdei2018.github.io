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