---
created_at: 2024-10-01
updated_at: 2024-10-02T14:06:02-03:00
tags:
  - note/literature/proposition
aliases: 
---

> [!important] Proposition: The [[Rational Numbers|rational numbers]] set has gaps
> $A=\{p\in\mathbb{Q}^{*+}|p^2<2\},B=\{p\in\mathbb{Q}^{*+}|p^2>2\}\implies\nexists\text{largest}(A),\text{smallest}(B)$

An equivalence to the conclusion is:
$$
\forall p\in A,\exists q\in A|q>p
$$
and
$$
\forall p\in B,\exists q\in B|q<p
$$
## Proofs

### Personal

By a geometric approach, in the case which $p\in A$ we can take $q^2$ being the point in the middle of the segment $[p^2,2]\in\mathbb{Q}$:

![[The rational numbers set has gaps proof - geometric intuition]]

so that:
$$
q^2=\frac{2-p^2}{2}\implies q^2-2=-\frac{p^2+2}{2}\implies q^2<2\implies q>p\wedge q\in A
$$
And the same reasoning to $p\in B$:
$$
q^2=\frac{p^2-2}{2}\implies q^2-2=\frac{p^2+2}{2}\implies q^2>2\implies q<p\wedge q\in B
$$
### [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=13&selection=102,0,132,18&color=yellow|Walter Rudin - Principles of Mathematical Analysis, p.13]]

