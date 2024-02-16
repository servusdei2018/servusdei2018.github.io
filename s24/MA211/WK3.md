# Week 3 - Sets

## Sets
A set is a collection of objects.

> E.g. 1: $\{a,b\}$ is a set whose elements are $a$ and $b$.

> E.g. 2: $\{1,2,3\}$ is the set whose elements are the first three natural numbers.

> E.g. 3: $A=\{1,2\}$ defines $A$ as said set.

### Set Notation

### Axiom of Extensionality
Two sets are equal iff they have the same elements.

> E.g. 4: $A=\{1,2\}$, $B=\{2,1\}$. $A=B$ since they have the same elements, regardless of the elements' order.

> E.g. 5: $A=\{1,2,2\}$, $B=\{1,2,2,1\}$ are the same set since they have the same elements and are both equal to $\{1,2\}$.

Note: We use $\in$ to denote set membership or to identify an element of a set. Or conversely, $\notin$.

Note: $x\in A$ reads "x is an element of set A" or "x belongs to set A." Conversely, $x\notin A$ reads "x is not an element of A."

### Subsets

Given sets $A,B$ we say $A$ is a subset of $B$ if every element of $A$ Is an element of $B$ or $A\subseteq B$. Or conversely, $A\nsubseteq B$

#### Examples
- Integers $\Z$
- Positive integers $\Z^+=\{1,2,3,\ldots\}$.
- Nonnegative integers/natural numbers: $\N=\{0,1,2,3,\ldots\}$
- Rational numbers
- Irrational numbers

### Set Builder Notation

$$
\{x\in D\,|\,p(x)\}
$$

Set of all $x$ in $D$ such that $p(x)$ is true.

> E.g. $\{x\in \R\,|\,x>1\}$ is the set of all real numbers such that $x>1$.

## Predicate

A predicate is a sentence which becomes a statement when specific values are substituted for specific variables in the sentence. The **domain** of a predicate variable is the set of all values that may be inserted in place of the variable.

## Truth Set

If $p(x)$ is a predicate and $x$ has domain $D$, the truth set of the predicate is the set of all elements of $D$ which make $p(x)$ true.

$$
\{x\in D\,|\,p(x)\}
$$

## Universal Quantifier

The universal quantifier $\forall$ "for all" applies to universal statements (e.g. $\forall x\in D,Q(x)$ -- for all values of $x$ in $D$, some $Q(x)$ is true). Such statements are true iff $Q(x)$ is true for every $x\in D$ and false iff $Q(x)$ is false for at least one $x\in D$ (counterexample).

> E.g. $\forall x\in D, x^2\geq x$
> 1. When $D=\{1,2,3\}$ is true, because it can be verified in each case
> 2. $D=\R$ is false by counterexample: $\frac{1}{2}=\frac{1}{4}\lt\frac{1}{2}$

## Existential Quantifier

The existential quantifier $\exists$ "there exists" applies to existential statements. E.g. $\exists x\in D\,s.t.\,Q(x)$ - there exists $x$ in $D$ such that $Q(x)$ is true. Such statements are true iff $Q(x)$ is true for at least one $x$ and false iff it's always false for all $x\in D$.

> E.g. let $Q(n)$ be the predicate statement "$n$ is a factor of $8$". Find the truth set for this statemen for two cases:
> 
> 1. where the domain of $Q(n)$ is $\Z^+$: $\{1,2,4,8\}$
> 2. where the domain of $Q(n)$ Is $\Z$: $\{-1,-2,-4,-8,1,2,4,8\}$
> 

> E.g. true/false
> 1. $\exists m\in\Z^+\,s.t.\, m^2=m$ true since $1\in\Z^+\,and\,1^2=1$.
> 2. $\exists m\in\{2,3,4\}\,s.t.\,m^2=m$ false since for each case $m^2\neq m$.

## Translating between Formal and Informal Language

Rewrite informally:

1. $\forall x\in\R,\,x^2\geq 0$ "Every real number's square is greater than or equal to zero"

2. $\forall x\in\R,\,x^2\neq -1$ "Every real number's square is not equal to minus one" or "There is no real number whose square is minus one"

3. $\exists x\in\Z^+\,s.t.\, x\in\Z$ "A positive integer is an integer"

Write formally:

1. "All triangles have three sides" $\forall t\in T\,s.t.\, t\in 3S$ Or *$t$ has three sides, $\forall$ triangles $t$*

2. "No dogs have wings" $\forall d\in D,\,s.t.\, d\notin W$ Or *$\forall$ dogs $d$, $d$ does not have wings*

Rewrite informally:

1. $\forall x\in\R$, if $x\gt 2$ then $x^2\gt 4$ "If a real number is greater than two then its square is greater than four"

Rewrite formally:

1. "No fire trucks are green" $\forall t\in T,\,s.t.\, t\notin G$ or *$\forall$ fire trucks $f$, $f$ is not green*

## Negation of Universal/Existential Statements

1. $\lnot(\forall x\in D, Q(x)) \equiv \exists x\in D\,s.t.\, \lnot Q(x) $
2. $\lnot(\exists x\in D, Q(x)) \equiv \forall x\in D,\,\lnot Q(x)$

And for conditional statements:

3. $\lnot(\forall x\in D,\,p(x)\leadsto q(x)) \equiv \exists x\in D\, s.t.\, \lnot(p(x)\leadsto q(x))$

Recall $\lnot(p\leadsto q)\equiv \lnot(\lnot p\lor q) \equiv p\land\lnot q$

Therefore

$$
\lnot(\forall x\in D,\,p(x)\leadsto q(x)) \equiv \exists x\in D\, s.t.\, p(x)\land\lnot q(x)
$$

4. $\lnot(\exists x\, D,\,p(x)\leadsto q(x)) \equiv \forall x\in D,\, \lnot(p(x)\leadsto q(x)) \equiv \forall x\in D,\, p(x)\land\lnot q(x)$

#### Examples

- $\lnot$($\forall$ primes $p$, $p$ is odd) $\equiv$ $\exists$ a prime $p$ such that $p$ is not odd

## Integers

1. An integer is *even* if $\exists m\in\Z$ such that $n=2m$
2. An integer is *odd* if $\exists m\in\Z$ such that $n=2m+1$

> E.g. $2$ is even because $2=2(1)$ where $n=2$ and $m=1$
>
> E.g. $3$ is odd since $3=2(1)+1$ where $n=3$ and $m=1$

## Constructive Proof of Existence

#### #4

E.g. show $\exists m,n\in\Z$ such that $m>1,n>1$ and $\frac{1}{m}+\frac{1}{n}\in\Z$

For example, $m=2,n=2$ then $\frac{1}{m}+\frac{1}{n}=\frac{1}{2}+\frac{1}{2}=1\in\Z$.

- Note: if $m>1,n>1$ then $\frac{1}{m}+\frac{1}{n}=\frac{n+m}{mn}$ would be an integer if $n+m$ is divisble by $mn$.

#### #6

E.g. $\exists a,b\in\R$ such that $\sqrt{a+b}=\sqrt{a}+\sqrt{b}$.

One such solution is $a=0,b=0$ for which $\sqrt{0+0}=0=\sqrt{0}+\sqrt{0}$

Alternatively, let $a\in\R,b=0$ for which $\sqrt{a+0}=\sqrt{a}=\sqrt{a}+\sqrt{0}$ or vice versa, $a=0,b\in\R$ such that the aforementioned still holds.

## Disproving a Universal Statement by Counterexample

#### #12

Disprove: $\forall n\in\Z$, if $n$ is odd then $\frac{n-1}{2}$ is odd.

This is false, by counterexample $n=5$ for which $\frac{5-1}{2}=\frac{4}{2}=2$ and $2$ is even.

The negation of the above statement $\lnot(\forall,p\leadsto q) \equiv \exists$ such that $p\land\lnot q$. In this case, $\exists n\in\Z$ such that $n$ is odd but $\frac{n-1}{2}$ is even.

Observe that finding a counterexample is equivalent to finding a case for which the negation of a universal statement holds true.

#### #13

Disprove: $\forall m,n\in\Z$ if $2m+n$ is odd then $m,n$ are both odd.

This is false. The negation of the above statement is $\exists (m,n\in\Z)$ such that $2m+n$ is odd but at least one of $m,n$ is not odd (i.e. even).

Note: $m=n=0$ satisfies this negation.

Another example is $(m=2,\,n=1)\lor(m=0,\,n=1)$.

## Proving Universal Statements

#### #28

Prove: for all integers $n$, if $n$ is odd then $n^2$ is odd

Proof.

1. Let $n\in\Z$ such that $n$ is odd
2. Since $n$ is odd, \exists m\in\Z$ such that $n=2m+1$ (by definition of odd)
3. Consider 

$$
n^2=(2m+1)^2\\= 4m^2+4m+1
$$

## Real Numbers

A real number $r$ is rational ($r\in\mathbb{Q}$) if

$$
\exists m,n\in\Z,\,n\neq 0
$$

such that

$$
r=\frac{m}{n}
$$

- A real number is irrational if it is not rational $r\notin\mathbb{Q}$

> E.g. is $0$ rational? Yes, because you can write $0$ as $\frac{0}{n}\,\forall n\in\Z$

> E.g. is $\frac{1}{0}$ rational? No, 1/0 is not even a real number

> E.g. is $0.23$ rational? Yes because $0.23=\frac{23}{100}$.

> E.g. is $\sqrt{2}$ rational? No, but not trivial

> E.g. if $m,n\in\Z$, $n\neq 0$, $m\neq 0$, is $\frac{m+n}{mn}$ rational? Yes since $m+n$ and $mn$ are integers (sum, product respectively); also, $m\neq 0$ and $n\neq 0\,\implies\, mn\neq 0$ (zero product property).

### Zero Product Property

If $mn=0$ then $m=0$ or $n=0$.

Contrapositive: If $\lnot(m=0 \lor n=0)$ then $\lnot(mn=0) \equiv$ if $m\neq 0 \land n\neq 0$ then $mn\neq 0$.

### Theorem: Every integer is a rational number

Proof: Suppose $n\in\Z$, then $n=\frac{n}{1}$ therefore $n$ is rational (by definition of rational).

### Theorem: The sum of two rational numbers is rational

Proof: Let $r,s\in\mathbb{Q}$.

Since $r\in\mathbb{Q}$, $\exists m,n\in\Z$, $n\neq 0$ such that $=\frac{m}{n}$.

Since $s\in\mathbb{Q}$, $\exists k,l\in\Z$, $l\neq 0$ such that $s=\frac{k}{l}$

Consider $r+s=\frac{m}{n}+\frac{k}{l} =\frac{ml+kn}{nl}$.

It follows that $r+s$ is a ratio of integers, and the denominator $nl\neq 0$ (since $n\neq 0$ and $l\neq 0$ by the zero product property). Hence, $r+s\in\mathbb{Q}$ as required. QED.

### Corollary (of the above theorem): The double of any rational number is a rational number [$\forall r\in\R$ if $r\in\mathbb{Q}$ then $2r\in\mathbb{Q}$]

Proof.

$r\in\mathbb{Q}$ then $2r=r+r$ is a sum of rationals.

Therefore by the last proof, QED.