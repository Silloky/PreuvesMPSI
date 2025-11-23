---
anki_linked: 0
raisonnements:
outils:
  - suites
kh_n:
  - "7"
display_title: Bornée APCR <=> Bornée
---
# Bornée APCR $\Longleftrightarrow$ Bornée

> [!objectif]
> Pour toute suite $u$, $u \text{ bornée}\;APCR\Longleftrightarrow u\text{ bornée}$
### Démonstration

Soit $u$ une suite.

***Sens $\implies$*** :
On suppose $u$ bornée $APCR$.
Donc il existe $M\geq 0$ tel qu'il existe $N\in \mathbb{N}$ tel que $\forall n\geq N, |u_{n}|\leq M$.
On pose $M'=\max(|u_{0}|,|u_{1}|,\dots,|u_{N-1}|,M)$.
Soit $n\in \mathbb{N}$.
Si $n\leq N-1$ : $|u_{n}|\leq M'$
Si $n\geq N$ : $|u_{n}|\leq M\leq M'$.
Donc dans tous les cas, $\forall n\in \mathbb{N}, |u_{n}|\leq M'$.
Donc $u$ est bornée.

***Sens $\Longleftarrow$*** :
Evident : si $u$ est bornée, elle est bornée *à partir* de $0$.

#### Remarques


