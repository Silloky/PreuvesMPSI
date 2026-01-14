---
anki_linked: 0
raisonnements:
outils:
  - sommes
  - polynome
kh_n:
display_title: Associativité du produit polynomial
---
# Associativité du produit polynomial

> [!objectif]
>$$
> \forall(P,Q,R)\in \mathbb{K}[X]^{3},(PQ)R=P(QR)
> $$
### Démonstration

Soit $(P,Q,R)\in \mathbb{K}[X]^{3}$.
Soit $n\in \mathbb{N}$.
$$
\begin{align}
[P(QR)]_{n}&=\sum_{k=0}^n[P]_{n-k}[QR]_{k} \\
&=\sum_{k=0}^n[P]_{n-k}\left( \sum_{k'=0}^k[Q]_{k-k'}[R]_{k'} \right)  \\
&=\sum_{k=0}^n\sum_{k'=0}^k[P]_{n-k}[Q]_{k-k'}[R]_{k'} \\
&=\sum_{k'=0}^n\left( \sum_{k=k'}^n[P]_{n-k}[Q]_{k-k'} \right)[R]_{k'} \\
&=\sum_{k'=0}^n\left( \sum_{k=0}^{n-k'}[P]_{(n-k')-k}[Q]_{k} \right) [R]_{k'} \\
&=\sum_{k'=0}^n[PQ]_{n-k'}[R]_{k'} \\
[P(QR)]_{n}&=[(PQ)R]_{n}
\end{align}
$$
D'où le résultat.

#### Remarques

Ceci contribue à montrer que $(\mathbb{K}[X],+,\times)$ est un anneau.
Voir la [[commutativite_produit_pol|commutativité]] dans le document à part.