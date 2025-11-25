---
anki_linked: 1
raisonnements:
  - double_implication
outils:
  - suites
kh_n:
display_title: Caractérisation séquentielle du caractère non majorée
---
# Caractérisation séquentielle du caractère *non majorée*

> [!objectif]
> Soit $A\in\mathcal{P}(\mathbb{R})$
>$$
> A \text{ n'est pas majorée}\iff \text{il existe une suite $(u_{n})$ d'éléments de $A$ qui tend vers $+\infty$}
> $$
### Démonstration

***Sens $\implies$*** :
On suppose que $A$ n'est pas majorée.
Pour tout $n\in \mathbb{N}$, $A$ n'est pas majorée donc il existe un élément de $A$ qu'on note $u_{n}$ tel que $u_{n}>n$.
On a là "construit" une suite d'éléments de $A$ telle que $\forall n\in \mathbb{N},u_{n}>n$ donc par [[theo_comparaison|comparaison]] $u_{n}\to +\infty$.

***Sens $\impliedby$*** :
On suppose qu'il existe une suite $(u_{n})$ d'éléments de $A$ (i.e. $u\in A^\mathbb{N}$) qui tend vers $+\infty$.
Soit $M\in \mathbb{R}$. 
$u_{n}\to +\infty$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N, u_{n}\geq M+1$.
En particulier, $u_{N}\in A$ et $u_{N}>M$, donc $A$ n'est pas majorée (puisque $M$ est quelconque).


#### Remarques


