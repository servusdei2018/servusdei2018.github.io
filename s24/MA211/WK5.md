# Week 5 - Basic Assumptions and Axioms

## Contradiction

To prove a statement $p$ by way of contradiction (BWOC) 

1. Assume that $p$ is false
2. Show that 1 leads to a contradiction
3. Done.

> Recall, $\lnot p\leadsto c$ therefore $p$.

For example, this special case: to prove a $\forall, A\leadsto B$:

1. Assume $\lnot(\forall, A\leadsto B)$ i.e. $\exists$ such that $A\land\lnot B$
2. Show that 1 leads to contradiction
3. Done

### Examples

E.g. there is no greatest integer.

Proof.

Suppose BWOC there is a greatest integer $N\in\Z$ such that $\forall n\in\Z$, $n\leq N$.

But take $m\in\Z$ such that $m=N+1$. Then $m>N$, since $N+1>N$; however, this contradicts $m\leq N$ as given. Thus both $m\leq N$ and $m>N$, contradiction.

---

E.g. there is no least integer.

Proof.

Suppose BWOC there is a least integer $N\in\Z$

Then $\forall n\in\Z$, $N\leq n$

Let $m=N-1$, then $m<N$ but also $m\in\Z$ so $m\geq N$, contradiction.

---

E.g. there is no least positive rational number.

Proof.

Suppose BWOC there is a least positive rational $r\in\mathbb{Q}^+$.

Then $\forall s\in\mathbb{Q}^+$, $r\leq s$.

But $t:=\frac{r}{2}$, then $t<r$ (since $\frac{r}{2}<r$) but also $r\in\mathbb{Q}^+$ so $r\leq t$, contradiction.

---

E.g. there is no integer which is both even and odd.

Suppose BWOC there is an integer $m\in\Z$ such that $m$ is both even and odd.

By def (even) $m=2k$

By def (odd) $m=2l+1$

For some integers $k,l$.

Thus $m=2k=2l+1=m$ and

$$
2k=2l+1\\
2(k-l)=1\\
k-l=\frac{1}{2}
$$

so $k,l$ are integers whose difference is a fraction but the difference of two integers is an integer, contradiction.

---

E.g. the sum of any rational and any irrational is irrational.

Proof.

$\forall r,s\in\R$ if $r\in\mathbb{Q}$ and $s\in\mathbb{Q}$ then $r+s\notin\mathbb{Q}$

BWOC suppose $\equiv \exists r,s\in\R$ such that $r\in\mathbb{Q}\land s\notin\mathbb{Q}$. But $r+s\in\mathbb{Q}$.

Since $r\in\mathbb{Q}$, $\exists m,n\in\Z$, $n\neq 0$ such that $r=\frac{m}{n}$;

Further, $r+s\in\mathbb{Q}$ so $\exists l,k\in\Z$, $k\neq 0$ such that $r+s=\frac{l}{k}$.

Hence $\frac{m}{n}+s=\frac{l}{k}$ so

$$
s=\frac{l}{k}-\frac{m}{n}\\
=\frac{ln-mk}{kn}
$$

and we see $s\in\mathbb{Q}$ which contradicts our assumption that $s\notin\mathbb{Q}$.

---

E.g. the product of any (non-zero) rational and any irrational is irrational.

## Quotient Remainder / Proof by Division into Cases

Theorem: Given any integer $n$ and positive integer $d$, there exist unique integers $q, r$ such that $n=dq+r, 0\leq r<d$.

E.g. $n=-54,d=4$, $-54=4(-14)+2$

## Representation of Integers (Parity Property of Integers)

Any integer is even or odd.

$\forall n\in\Z$, $n=2k \lor n=2k+1$.

Proof.

Apply the quotient remainder theorem to $n\in\Z$ with $d=2$:

$n=2q+r$, $0\leq r<2$

Note there are two cases, $r=0$ and $r=1$.

Case 1: $r=0,n=2q$ where $q\in\Z$ hence $n$ is even

Case 2: $r=1,n=2q+1$ where $q\in\Z$ hence $n$ is odd

In either case, the result follows.

Note: We proved in 4.5 that $n\in\Z$ can't be both even and odd.

## Parity of Consecutive Integers

Any two consecutive integers have opposite parity.

Proof.

Suppose $n\in\Z$, hence $n+1$ is the successor of $n$. Then $n$ is either even or odd.

Case 1: $n$ even. If $n$ is even, $\exists k\in\Z$ such that $n=2k$ so $n+1=2k+1$ is odd.

Case 2: $n$ odd. If $n$ is odd, $\exists k\in\Z$ such that $n=2k+1$ so $2k+1+1=2k+2=2(k+1)$; so $n+1$ is even.

Since cases 1 and 2 are exhaustive (by quotient remainder theorem), the result follows.

##  