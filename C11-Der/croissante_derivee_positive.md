---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - dérivation
kh_n:
  - "10"
display_title: Croissante <=> Dérivée positive
---
# Croissante $\iff$ Dérivée positive

> [!objectif]
> Soit $I$ un intervalle et $f:I\to \mathbb{R}$ dérivable sur $I$.
> Alors on a : $f$ croissante sur $I$ $\iff$ $f'$ positive sur $I$
### Démonstration

***Sens $\implies$***:
On suppose $f$ croissante.
Soit $a \in I$, et pour tout $x>a$, $\frac{\overbrace{ f(x)-f(a) }^{ \geq 0\text{ car} f\nearrow }}{\underbrace{ x-a }_{ >0 }}\geq 0$ 
Or $f$ est dérivable sur $I$, donc en $a\in I$ donc par passage à la limite, $f'(a)\geq 0$

***Sens $\impliedby$*** :
On suppose $f'$ positive sur I.
Soit $(x,y)\in I^{2}$. On suppose $x\leq y$.
Le cas $x=y$ est évident, donc on suppose $x<y$.
D'après le théorème des [[theo_accroissements_finis|accroissements finis]], il existe $c\in]x,y[$ tel que $f'(c)=\frac{f(x)-f(y)}{x-y}$
Or $x<y$ et $c\in]x,y[\subset I$, donc par hypothèse, $f'(c)\geq 0$.
Ainsi $f(x)-f(y)\leq 0$, donc $f(x)\leq f(y)$.
Donc $f$ est croissante sur $I$.

#### Remarques


