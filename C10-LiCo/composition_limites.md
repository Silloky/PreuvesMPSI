---
anki_linked: 0
raisonnements:
outils:
  - limites
  - voisinages
kh_n:
  - "9"
display_title: Composition de limites
---
# Composition de limites

> [!objectif]
> Soit $f:I\to \mathbb{R}$, $g:J\to \mathbb{R}$ avec $f(I)\subset J$, $a\in \bar{I}$, $b\in \bar{\mathbb{R}}$ et $L\in \bar{\mathbb{R}}$
> On suppose que $f(x)\xrightarrow[x\to a]{}b\in \bar{J}$ et $g(x)\xrightarrow[x\to b]{}L$
> Alors : $(f\circ g)(x)\xrightarrow[x\to a]{}L$
### Démonstration

Soit $W\in \mathcal{V}(L)$.
On a :
* $g(y)\xrightarrow[y\to b]{}L$, donc il existe $V\in \mathcal{V(b)}$ tel que $\forall y\in J,y\in V\implies g(y) \in W$
* $f(x)\xrightarrow[x\to a]{}b$ donc il existe $U\in \mathcal{V}(a)$ tel que $\forall x\in I, x \in U\implies f(x)\in V$
Ainsi, pour tout $x \in I$, $x \in U\implies f(x)\in V\implies g(f(x))\in W$.
D'où  $(f\circ g)(x)\xrightarrow[x\to a]{}L$

#### Remarques


