---
created_at: 2024-10-01
updated_at: 2024-10-03T19:53:22-03:00
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

Consider:
$$
q=p-\frac{p^2-2}{p+2}=\frac{2p+2}{p+2}
$$
and:
$$
q^2-2=\frac{2(p^2-2)}{(p+2)^2}
$$
we have two cases:
$$
\begin{cases}
p\in A\implies p^2-2<0\implies q^2<2\implies q\in A\\
p\in B\implies p^2-2>0\implies q^2>2\implies q\in B\\
\end{cases}
$$Here is a representation of the q (blue) number as a function of p and q² (red):

```desmos-graph
left=0; right=2
top=2;bottom=0
---
f(x)=\sqrt{2}|green|dashed
x(y)=\sqrt{2}|green|dashed
q(p)=(2p+2)/(p+2)|blue
q_2(p)=q(p)^2|red
```
