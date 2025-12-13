---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - dérivation
kh_n:
  - "10"
display_title: Constante <=> Dérivée nulle
---
# Constante $\iff$ Dérivée nulle

> [!objectif]
> Soit $I$ un intervalle et $f:I\to \mathbb{R}$ dérivable sur $I$
> Alors $f$ constante sur $I$ $\iff$ $f'$ nulle sur $I$.
### Démonstration

***Sens $\implies$***:
Soit $x \in I$
$f$ est constante sur $I$, donc pour tout $y\in I$, $f(x)=f(y)$
$f$ est dérivable sur $I$, donc pour tout $x \in I$, $f'(x)=\lim_{ y \to x }\frac{f(y)-f(x)}{y-x}=0$.
Donc $f'$ est nulle sur $I$.

***Sens $\impliedby$***:
On suppose que pour tout $x \in I$, $f'(x)=0$.
Soit $(x,y)\in I^{2}$, on suppose $x<y$.
$[x,y]$ est un intervalle et $[x,y]\subset I$, donc $f$ est continue sur $[x,y]$ et dérivable sur $]x,y[$.
Donc d'après le théorème des [[theo_accroissements_finis|accroissements finis]], il existe $c \in]x,y[$ tel que $f'(c)=\frac{f(x)-f(y)}{x-y}$.
Or $c \in I$, donc $f'(c)=0$, donc $f(x)-f(y)=0$.
Ainsi $f$ est constante sur $I$.


#### Remarques


