---
anki_linked: 0
raisonnements:
outils:
  - limites
  - voisinages
kh_n:
  - "9"
display_title: Théorème d'encadrement (fonctions)
---
# Théorème d'encadrement (fonctions)

> [!objectif]
> Soit $f:I\to \mathbb{R}$, $g:I\to \mathbb{R}$, $h:I\to \mathbb{R}$ et $a\in \bar{I}$ tel que $a\in \mathbb{R}$.
> On suppose que :
> * $f(x)\xrightarrow[x\to a]{}l$
> * $h(x)\xrightarrow[x\to a]{}l$
> * $f(x)\leq g(x)\leq h(x)$ au voisinage de $a$
> 
> Alors $g(x)\xrightarrow[x\to a]{}l$
### Démonstration

Soit $\varepsilon>0$.
On a :
* $f(x)\xrightarrow[x\to a]{}l$ donc il existe $\eta>0$ tel que $\forall x \in I, |x-a|\leq \eta\implies |f(x)-l|\leq\varepsilon$
* $h(x)\xrightarrow[x\to a]{}l$ donc il existe $\eta'>0$ tel que $\forall x \in I, |x-a|\leq \eta'\implies |h(x)-l|\leq \varepsilon$
* $f(x)\leq g(x)\leq h(x)$ au voisinage de $a$ donc il existe $\eta''>0$ tel que $\forall x \in I, |x-a|\leq \eta''\implies f(x)\leq g(x)\leq h(x)$
On pose $\alpha=\min(\eta,\eta',\eta'')$, alors :
$$
\forall x \in I, |x-a|\leq\alpha\implies l-\varepsilon\leq f(x)\leq g(x)\leq h(x)\leq l+\varepsilon
$$
D'où $g(x)\xrightarrow[x\to a]{}l$

#### Remarques


