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

E.g. show $\exists m,n\in\Z$ such that $m>1,n>1$ and $\frac{1}{m}+\frac{1}{n}\in\Z$

For example, $m=2,n=2$ then $\frac{1}{m}+\frac{1}{n}=\frac{1}{2}+\frac{1}{2}=1\in\Z$.

- Note: if $m>1,n>1$ then $\frac{1}{m}+\frac{1}{n}=\frac{n+m}{mn}$. 