---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - limites
kh_n:
  - "10"
display_title: Lipschitzienne => continue (éciproque fausse)
---
# Lipschitzien $\implies$ continu (réciproque fausse)

> [!objectif]
> Soit $I$ un intervalle et $f:I\to \mathbb{R}$.
> Si $f$ est lipschitzienne sur $I$, alors elle est continue sur $I$.
### Démonstration

***Sens $\implies$*** :
On suppose $f$ lipschitzienne sur $I$, donc il existe $k\geq 0$ tel que $\forall (x,y)\in I^{2},|f(x)-f(y)|\leq k|x-y|$.
Soit $a\in I$. Pour tout $x \in I$, $0\leq|f(x)-f(a)|\leq k |x-a|\xrightarrow[x\to a]{} 0$.
Donc par encadrement, $f(x)-f(a)\xrightarrow[x\to a]{}0$, donc $f(x)\xrightarrow[x\to a]{}f(a)$.
Donc $f$ est continue en $a$.

***Sens $\impliedby$ (faux)*** :
La fonction $x\mapsto x^{2}$ est un contre-exemple.
Par l'absurde, on suppose que la fonction carré est lipschitzienne, donc qu'il existe $k\in \mathbb{R}_{+}$ tel que $\forall (x,y)\in \mathbb{R}^{2}, |x^{2}-y^{2}|\leq k|x-y|$.
En particulier, $\forall x \in \mathbb{R}, |(x+1)^{2}-x^{2}|\leq k|(x+1)-x|$, donc $|2x+1|\leq k$.
Or $|2x+1|\xrightarrow[x\to +\infty]{}+\infty$, ce qui est absurde, donc $x\mapsto x^{2}$ est continue mais pas lipschitzienne.

#### Remarques

