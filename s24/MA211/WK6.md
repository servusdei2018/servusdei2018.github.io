# Review

- Truth table
- Negation/contrapositive/converse
- Example/counterexample
- Proof by contradiction/contraposition
- Divisibility
- Even/odd/irrational
- Quotient remainder theorem

---

Eg. show that the negative of any irrational is irrational

- Use contradiction

1. Assume statement false $\lnot(\forall ,p\leadsto q)\equiv \exists$ such that $p\land\lnot q$
2. Show that 1 leads to a contradiction $\forall r\in\R$, if $r\notin\mathbb{Q}$ then $-r\notin\mathbb{Q}$.

E.g. show that the negative of any irrational is irrational.

Suppose BWOC that $\exists r\in\R$ such that $r\notin\mathbb{Q}$ and $-r\in\mathbb{Q}$

Suppose $-r\in\mathbb{Q}$, $\exists m,n\in\Z,n\neq 0$ such that $-r=\frac{m}{n}$

Then $r=-\frac{m}{n}=\frac{(-1)m}{n}$ hence $r\in\mathbb{Q}$ (ratio of two integers with nonzero denominator)

Contradiction. This contradicts our assumption that $r\notin\mathbb{Q}$.

---

QR theorem: given $n=dq+r$, $0\leq r\lt d$ ($d$ amount of cases)

Cases: $r:=0\to(d-1)$

---

E.g. show the square of any integer may be written in the form $4k$ or $4k+1$.

---

## Divisibility

E.g. show that $\forall a,b,c\in\Z$ if $\frac{ab}{c}$ then $a/c$ and $b/c$.

Definition: $d/n \equiv \exists k\in\Z$ such that $n=dk$ or $\frac{n}{d}=k$.

Suppose $a,b,c\in\Z$ and $ab/c$ (we show $a/c$ and $b/c$)

Since $ab/c$, $\exists k\in\Z$ such that $c=abk$.

Then $c=(ab)k$ (i.e. $a/c$) and $c=(ba) k$ ($b/c$)