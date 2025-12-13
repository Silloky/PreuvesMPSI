---
anki_linked: 0
raisonnements:
outils:
  - derivation
kh_n:
  - "10"
display_title: Dérivable implique continue
---
# Dérivable $\implies$ continue

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ et $a\in I$.
> Si $f$ est dérivable en $a$ alors elle est continue en $a$.
### Démonstration

On suppose $f$ dérivable en $a$.
D'après la [[caract_epsilon_derivabilite|caractérisation epsilonesque de la dérivabilité]], il existe $m=f'(a)$ et $\varepsilon:I\to \mathbb{R}$ tels que $\varepsilon(x)\xrightarrow[x\to a]{}0$ et $\forall x \in I,f(x)=f(a)+m(x-a)+\varepsilon(x)(x-a)$
Or $m(x-a)\xrightarrow[x\to a]{}0$ et $\varepsilon(x)\xrightarrow[x\to a]{}0$.
Donc $f(x)\xrightarrow[x\to a]{}f(a)$, ainsi $f$ est continue en $a$

#### Remarques


