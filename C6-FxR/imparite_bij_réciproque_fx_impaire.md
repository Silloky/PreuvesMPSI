---
anki_linked: 0
raisonnements:
outils:
kh_n:
display_title: Imparité de la bijection réciproque d'une fonction impaire
---
# Imparité de la bijection réciproque d'une fonction impaire

> [!objectif]
> Soit $f:I\to J$ une bijection impaire. Alors $f^{-1}$ est impaire.
### Démonstration

Soit $f:I\to J$ une bijection.
On suppose $f$ impaire, donc $I$ est centré en $0$.
Soit $y \in J$. $f$ est bijective, donc il existe un unique $x \in I$ tel que $f(x)=y$.
Or $I$ est centrée sur $0$, donc : $-x \in I$, i.e. $-f^{-1}(y)\in I$.
Ainsi, on peut appliquer la fonction $f$ est impaire : $f(-f^{-1}(y))=-f(f^{-1}(y))=-y \in J$ (donc $J$ est centré sur $0$ aussi).
De plus, $f(f^{-1}(-y))=-y$, puisque $-y \in J$.
Or $f$ est injective, donc comme on a $f(f^{-1}(y))=f(-f^{-1}(y))$, on peut dire que $f^{-1}(y)=-f^{-1}(y)$.
Autrement dit, $f^{-1}$ est impaire.

#### Remarques


