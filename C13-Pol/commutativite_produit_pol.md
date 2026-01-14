---
anki_linked: 0
raisonnements:
outils:
  - sommes
  - polynome
kh_n:
display_title: Commutativité du produit polynomial
---
# Commutativité du produit polynomial

> [!objectif]
>$$
> \forall(P,Q)\in \mathbb{K}[X]^{2},PQ=QP
> $$
### Démonstration

**En une ligne** : par retour à la somme d'éléments de $(\mathbb{K},+)$ qui est un groupe commutatif, on montre que le produit polynomial est commutatif.

Soit $(P,Q)\in \mathbb{K}[X]^{2}$.
Soit $n\in \mathbb{N}$.
$$
\begin{align}
[PQ]_{n}&=\sum_{k=0}^n[P]_{n-k}[Q]_{k} \\
&=\sum_{k=0}^n[Q]_{k}[P]_{n-k} \\
&=\sum_{k=0}^n[Q]_{n-k}[P]_{k} \\
[PQ]_{n}&=[QP]_{n}
\end{align}
$$
D'où le résultat.
#### Remarques


