---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
kh_n:
  - "4"
---
# Monotonie de la composée de fonctions monotones

> [!objectif]
> La composée de 2 fonctions monotones est monotone.
### Démonstration

Soit $f:I\to J$ et $g:J\to \mathbb{R}$ deux fonctions monotones sur leur ensemble de départ.

***Si $f$ est croissante et $g$ décroissante*** :
Soit $(x,y)\in I^{2}$. On suppose que $x<y$.
$f$ est croissante, donc $f(x)\leq f(y)$
$g$ est décroissante, donc $g(f(y))\leq g(f(x))$
Donc $(g\circ f)(y)\leq(g\circ f)(x)$
Donc $g\circ f$ est décroissante sur $I$

***Idem pour les 3 autres cas***

#### Remarques

Preuve élégante qui réduit le nombre de cas à étudier à 2 en introduisant une fonction qui généralise la même monotonie/monotonie opposée : [ChatGPT](https://chatgpt.com/share/6905f0f9-eab0-8001-8127-e0f7a862dda1)
