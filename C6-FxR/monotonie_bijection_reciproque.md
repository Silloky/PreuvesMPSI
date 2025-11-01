---
anki_linked: 0
raisonnements:
  - absurde
outils:
  - bijection
kh_n:
  - "4"
display_title: Monotonie bijection réciproque
---
# Monotonie de la bijection réciproque d'une fonction monotone

> [!objectif]
> Soit $f:I\to J$ une bijection monotone. Sa bijection réciproque $f^{-1}$ est monotone et de même sens de variation que $f$
### Démonstration

Soit $f:I\to J$ une bijection monotone, donc $f^{-1}$ existe.

***Si $f$ est croissante*** :
Soit $(y_{1},y_{2})\in J$ ; on suppose que $y_{1}<y_{2}$.
On suppose par l'absurde que $f^{-1}(y_{1})\ge f^{-1}(y_{2})$
Comme $f$ est croissante, $f(f^{-1}(y_{1}))\geq f(f^{-1}(y_{2}))$, donc $y_{1}\geq y_{2}$, ce qui est absurde.
Donc $f^{-1}(y_{2})\ge f^{-1}(y_{1})$.
Donc $f^{-1}$ est croissante sur $J$

***Idem si $f$ est décroissante***


#### Remarques


