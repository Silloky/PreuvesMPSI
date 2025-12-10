---
anki_linked: 0
raisonnements:
outils:
  - limites
  - voisinages
kh_n:
  - "9"
display_title: Théorème du passage à la limite (fonctions)
---
# Théorème du passage à la limite (fonctions)

> [!objectif]
> Soit $f:I\to \mathbb{R}$, $g:I\to \mathbb{R}$ et $a\in \bar{I}$ tel que $a\in \mathbb{R}$.
> On suppose que :
> * $f(x)\xrightarrow[x\to a]{}l$
> * $g(x)\xrightarrow[x\to a]{}l'$
> * $f(x)\leq g(x)$ au voisinage de $a$
> 
> Alors $l\leq l'$
### Démonstration

Par l'absurde, on suppose que $l'<l$.
On pose $\varepsilon=\frac{l-l'}{3}$.

On a :
* $f(x)\xrightarrow[x\to a]{}l$ donc il existe $\eta>0$ tel que $\forall x \in I,|x-a|\leq \eta\implies |f(x)-l|\leq\varepsilon$
* $g(x)\xrightarrow[x\to a]{}l'$ donc il existe $\eta'>0$ tel que $\forall x \in I, |x-a|\leq \eta'\implies |g(x)-l'|\leq\varepsilon$
* $f(x)\leq g(x)$ au voisinage de $a$, donc il existe $\eta''>0$ tel que $\forall x \in I,|x-a|\leq \eta''\implies f(x)\leq g(x)$

$a\in \bar{I}$, donc il existe $x_{0}\in I\cap [a-\min(\eta,\eta',\eta''),a+\min(\eta,\eta',\eta'')]$ tel que :
* $|f(x_{0})-l|\leq \varepsilon$ donc $l-\varepsilon\leq f(x_{0})$
* $|g(x_{0})-l'|\leq\varepsilon$ donc $g(x_{0})\geq l'+\varepsilon$
* $f(x_{0})\leq g(x_{0})$
Donc $l-\varepsilon\leq f(x_{0})\leq g(x_{0})\leq l'+\varepsilon$, donc $l'\geq l$, ce qui est absurde.

D'où $l\leq l'$.

#### Remarques


