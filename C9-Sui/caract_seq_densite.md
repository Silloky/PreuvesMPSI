---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - suites
  - densite
kh_n:
display_title: Caractérisation séquentielle de la densité
---
# Caractérisation séquentielle de la densité

> [!objectif]
> Soit $A\in\mathcal{P}(\mathbb{R})$
>$A$ est dense dans $\mathbb{R}$ $\iff$ Pour tout réel $x$, il existe une suite d'éléments de $A$ qui tend vers $x$.
### Démonstration

***Sens $\implies$*** :
On suppose $A$ dense dans $\mathbb{R}$.
Soit $x \in \mathbb{R}$. 
$A$ est dense dans $\mathbb{R}$, donc pour tout $n\geq 1$, il existe un élément de $A$ qu'on note $u_{n}$ dans $\left[ x- \frac{1}{n}, x+\frac{1}{n} \right]$.
$(u_{n})$ est une suite d'éléments de $A$ de $\forall n\geq 1, x-\frac{1}{n} \leq u_{n}\leq x+\frac{1}{n}$, donc par encadrement, $u_{n}\to x$

***Sens $\impliedby$*** :
On suppose que pour tout réel $x$, il existe une suite d'éléments de $A$ qui tend vers $x$.
Soit $x \in \mathbb{R}$ et $\varepsilon>0$.
Il existe une suite $u_{n}$ d'éléments de $A$ telle que $u_{n}\to x$, donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N, |u_{n}-x|\leq \varepsilon$.
En particulier, $u_{N}\in \left[ x-\varepsilon,x+\varepsilon \right]$, et $u_{N}\in A$, donc par définition $A$ est dense dans $\mathbb{R}$.


#### Remarques


