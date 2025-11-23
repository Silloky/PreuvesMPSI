---
anki_linked: 0
raisonnements:
  - absurde
outils:
  - suites
kh_n:
  - "7"
display_title: Unicité de la limite d'une suite
---
# Unicité de la limite d'une suite

> [!objectif]
> Si une suite admet une limite alors elle est unique.
### Démonstration

Soit $(l,l')\in \mathbb{R}^{2}$. On suppose que $l<l'$.

Par l'absurde, on suppose que $u_{n}\to l$ et que $u_{n}\to l'$.
On pose $\varepsilon=\frac{l'-l}{2}>0$.
Or :
* $u_{n}\to l$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq\varepsilon$
* $u_{n}\to l'$ donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},|u_{n}-l'|\leq\varepsilon$
On pose $M=\max(N_{1},N_{2})$.
Alors :
* $M\geq N_{1}$ donc $|u_{M}-l|\leq\varepsilon$ donc en particulier $u_{M}\leq\varepsilon+l$
* $M\geq N_{2}$ donc $|u_{M}-l'|\leq\varepsilon$ donc en particulier $u_{M}\geq l'-\varepsilon$
Ainsi $l'-\varepsilon\leq u_{M}\leq\varepsilon+l$, donc $l'-\varepsilon\leq\varepsilon+l$, donc $l'\leq l$, ce qui est absurde.

Donc $l=l'$.


#### Remarques


