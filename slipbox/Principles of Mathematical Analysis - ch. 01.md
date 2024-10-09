---
created_at: 2024-10-01
updated_at: 2024-10-09T19:43:10-03:00
tags:
  - note/literature/book-chapter
aliases:
  - PMA ch. 01
  - Baby Rudin ch. 01
---
# The Real and Complex Number Systems

## Introduction

- We shall define the [[Real Numbers]] to have satisfactory studying of [[Real Analysis]].

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=12&selection=14,0,16,22&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.12]]
> > A satisfactory discussion of the main concepts of analysis (such as convergence, continuity, differentiation, and integration) must be based on an accurately defined number concept

- The [[Rational Numbers]] is not sufficient to use concepts like [[Convergence]], [[Continuity]], [[Differentiation]] and [[Integration]].

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=12&selection=40,0,41,28&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.12]]
> > The rational number system is inadequate for many purposes, both as a field and as an ordered set.
> 
> 

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=12&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.12]]
> > For instance, there is no rational p such that $p^2 = 2$. (We shall prove this presently.) This leads to the introduction of so-called "[[Irrational Numbers|irrational numbers]]" which are often written as infinite decimal expansions and are considered to be "approximated" by the corresponding finite decimals. Thus the sequence
> > 
> > $1 , 1 .4, 1 .41 , 1 .414, 1 .4142, . . .$
> > 
> > "tends to $\sqrt2$." But unless the [[Irrational Numbers|irrational number]] $\sqrt2$ has been clearly defined, the question must arise: Just what is it that this sequence "tends to" ?
> > 
> > This sort of question can be answered as soon as the so-called "[[Real Numbers|real number system]]" is constructed.
> 

- [[The square root of 2 is irrational]] 
- [[The rational numbers set has gaps]]
- The [[Real Numbers|real number]] system fills these gaps
- [[Ordered Set]] and [[Field]] are fundamental concepts to analysis study
- Some [[Set]] operations and notations will be used in this book:

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=14&selection=24,0,35,1&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.14]]
> > If A is any [[Set|set]] (whose elements may be numbers or any other objects), we write $x\in A$ to indicate that x is a member (or an element) of A. ([[Set Element]])

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=14&selection=37,0,43,2&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.14]]
> > If x is not a member of A, we write: $x\notin A$ . ([[Set Element]])

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=14&selection=45,0,52,9&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.14]]
> > The set which contains no element will be called the [[Empty Set|empty set]]. If a set has at least one element, it is called [[Nonempty Set|nonempty set]].

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=14&selection=54,0,107,2&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.14]]
> > If A and B are sets, and if every element of A is an element of B, we say that A is a ***[[Subset|subset]]*** of B, and write $A\subset B$, or $B\supset A$. If, in addition, there is an element of B which is not in A, then A is said to be a ***[[Proper Subset|proper subset]]*** of B. Note that $A\subset A$ for every set A.

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=14&selection=109,0,131,1&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.14]]
> > If $A\subset B$ and $B\supset A$, we write $A=B$. Otherwise $A\ne B$

- Definition: [[Order]]
- Definition: [[Ordered Set]]
- Definition: [[Bounded Set]]
- Definition: [[Infimum and Supremum]]
- Examples:

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=15&selection=125,0,125,3&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.15]]
> $$A=\{p\in\mathbb{Q}|p^2<2\}\text{, }B=\{p\in\mathbb{Q}|p^2>2\}$$
> $A$ is [[Bounded Set|bounded above]]. The upper bounds of $A$ are the members of $B$. Since $B$ has no smallest member, $A$ has no [[Infimum and Supremum|least upper bound]] in $\mathbb{Q}$.
> 
> The same logic applies to $B$.

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=15&selection=191,0,191,3&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.15]]
> If $\alpha=\text{sup }E$ exists, then $\alpha$ may or may not be a member of $E$. Let
> $$E_1=\mathbb{Q}^{-*}, E_2=\mathbb{Q}^{-}$$
> Then
> $$\text{sup }E_1=\text{sup }E_2=0\text{ | }0\notin E_1\text{, }0\in E_2$$
> 

> [!PDF|yellow] [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=15&selection=270,0,270,3&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.15]]
> $$
> E=\{\frac{1}{n}|n\in\mathbb{N}^*\}\implies
> \begin{cases}
> \text{sup }E=1\in E\\
> \text{inf }E=0\notin E
> \end{cases}
> $$
> 

