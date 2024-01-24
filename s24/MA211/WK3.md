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

## Existential Quantifier

The existential quantifier $\exists$ "there exists" applies to existential statements. E.g. $\exists x\in D\,s.t.\,Q(x)$ - there exists $x$ in $D$ such that $Q(x)$ is true. Such statements are true iff $Q(x)$ is true for at least one $x$ and false iff it's always false for all $x\in D$.

> E.g. let $Q(n)$ be the predicate statement "$n$ is a factor of $8$". Find the truth set for this statemen for two cases:
> 
> 1. where the domain of $Q(n)$ is $\Z^+$: $\{1,2,4,8\}$
> 2. where the domain of $Q(n)$ Is $\Z$: $\{-1,-2,-4,-8,1,2,4,8\}$
> 
