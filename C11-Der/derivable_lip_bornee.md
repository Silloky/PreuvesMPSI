---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - dérivation
kh_n:
  - "10"
display_title: Equivalence (dérivable & lipschitzienne) et (bornée)
---
# Equivalence (dérivable & lipschitzienne) et (bornée)

> [!objectif]
> Soit $I$ un intervalle et $k\geq 0$. Soit $f:I\to \mathbb{R}$. On suppose $f$ dérivable sur $I$.
> 1. $f$ $k$-lipschitzienne sur $I$ $\iff$ $|f'|\leq k$ sur $I$
> 2. $f$ lipschitzienne sur $I$ $\iff$ $f'$ bornée sur $I$
### Démonstration

##### 1. $k$-lipschitzienne

***Sens $\implies$***:
On suppose que $f$ est $k$-lipschitzienne sur $I$.
Soit $a\in I$.
$f$ est $k$-lipschitzienne, donc pour tout $x \in I$ on a $|f(x)-f(a)|\leq k|x-a|$.
Donc pour tout $x \in I\setminus \{ a \}$, $\left| \frac{f(x)-f(a)}{x-a} \right|\leq k$.
Par [[theo_passage_lim_fx|passage à la limite]], on en déduit que $|f'(a)|\leq k$.
Donc $|f'|\leq k$ sur $I$.

***Sens $\impliedby$*** :
On suppose que $|f'|\leq k$ sur $I$.
Soit $(x,y)\in \mathbb{R}^{2}$, on suppose que $x<y$.
$f$ est continue sur $[x,y]\subset I$ et dérivable sur $]x,y[\subset I$ donc d'après le théorème des [[theo_accroissements_finis|accroissements finis]], il existe $c \in]x,y[$ tel que $f'(c)=\frac{f(x)-f(y)}{x-y}$.
Or $c \in I$, donc $|f'(c)|\leq k$, et donc $\left| \frac{f(x)-f(y)}{x-y} \right|\leq k$.
Ainsi $|f(x)-f(y)|\leq k|x-y|$, donc $f$ est $k$-lipschitzienne.

##### 2. Lipschitzienne

***Sens $\implies$*** :
On suppose $f$ lipschitzienne, donc il existe $k\geq 0$ tel que $f$ soit $k$-lipschitzienne.
D'après le point précédent, $|f'|\leq k$ sur $I$, donc $f'$ est bornée sur $I$.

***Sens $\impliedby$***:
On suppose $f$ bornée sur $I$. Donc il existe $k\geq 0$ tel que $|f'|\leq k$.
D'après le point précédent, $f$ est alors $k$-lipschitzienne, donc $f$ est lipschitzienne.

#### Remarques


