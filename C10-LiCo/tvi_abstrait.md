---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - tvi
kh_n:
  - "9"
display_title: Théorème des Valeurs Intermédiaires (Abstrait)
---
# Théorème des valeurs intermédiaires (Abstrait)

> [!objectif]
> Soit $I$ un intervalle et $f$ une fonction continue sur $I$. Alors $f(I)$ est un intervalle.
### Démonstration

Soit $(y_{1},y_{2})\in f(I)^{2}$. On suppose que $y_{1}<y_{2}$.
* $y_{1}\in f(I)$ donc il existe $x_{1}\in I$ tel que $f(x_{1})=y_{1}$
* $y_{2}\in f(I)$ donc il existe $x_{2}\in I$ tel que $f(x_{2})=y_{2}$
Soit $y\in[y_{1},y_{2}]$.

***Cas $x_{1}<x_{2}$*** :
$f$ est continue sur $[x_{1},x_{2}]\subset I$ et $y\in[f(x_{1}),f(x_{2})]$.
Donc d'après le [[tvi_annulation|TVI]], il existe $x \in[x_{1},x_{2}]\subset I$ tel que $y=f(x)$.
Or $x \in I$, donc $y=f(x)\in f(I)$.
Ainsi $f(I)$ est un intervalle.

***Les autre cas sont similaires***

Donc $f(I)$ est un intervalle.

#### Remarques


