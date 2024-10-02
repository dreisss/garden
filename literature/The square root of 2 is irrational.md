---
created_at: 2024-10-01
updated_at: 2024-10-01
tags:
  - note/literature/proposition
aliases:
---

> [!important] Proposition: The square root of 2 is irrational
> $\sqrt2\notin\mathbb{Q}\text{ or }\nexists p\in\mathbb{Q}|p^2=2$

## Proofs

### [[Walter Rudin - Principles of Mathematical Analysis.pdf#page=13&selection=15,0,15,29&color=red|Walter Rudin - Principles of Mathematical Analysis, p.13]]

We shall prove that doesn't exist any [[Rational Numbers|rational number]] $p$ such that $p^2=2$:
$$
\nexists p\in\mathbb{Q}|p^2=2
$$
we can prove by contradiction, assuming exists a $p$ with this properties. By definition:
$$
p\in\mathbb{Q}\implies\exists{m,n}\in\mathbb{Z},n\ne0,m\text{ and }n\text{ are not both even}|p=\frac{m}{n}
$$
so:
$$
(\frac{m}{n})^2=2\implies m^2=2n^2
$$
this means that $m$ is an [[Even Number]]. So that:
$$
m=2k,k\in\mathbb{Z}\implies m^2=4k^2\implies 4k^2=2n^2\implies n^2=2k^2
$$
and again, makes $n$ even, which is contradictory to the definition.