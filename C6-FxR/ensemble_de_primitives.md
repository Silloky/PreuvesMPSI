---
anki_linked: 1
raisonnements:
  - double_inclusion
outils:
  - primitives
kh_n:
  - "4"
display_title: Ensemble de primitives à partir d'une seule
---
# Ensemble de primitives à partir d'une seule

> [!objectif]
> Soit $f:I\to \mathbb{R}$. On suppose que $f$ admet une primitive $F$ sur $I$.
> Alors l'ensemble des primitives de $f$ sur $I$ est :
>$$
> \{x\mapsto F(x)+c\mid c\in \mathbb{R}\}
> $$
### Démonstration

***Sens $\subset$*** :

Soit $G$ une primitive $f$ sur $I$.
Donc $(G-F)'=G'-F'=f-f=0$, donc $G-F$ est une constante, i.e. $\exists c\in\mathbb{R}, \forall x\in I, G(x)=F(x)+c$.
Autrement dit, $G\in\{x\mapsto F(x)+c\mid c\in\mathbb{R}\}$

***Sens $\supset$*** :

Soit $G\in\{x\mapsto F(x)+c\mid c\in\mathbb{R}\}$.
$G$ est dérivable car $F$ est dérivable (puisque $F$ est une primitive de $f$), et $c$ aussi.
Donc $G'(x)=F'(x)+(c)'=f(x)+0=f(x)$
Donc $G$ est une primitive de $f$ sur $I$

#### Remarques


