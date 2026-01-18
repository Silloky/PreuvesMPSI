---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Dérivée d'une composition de polynômes
---
# Dérivée d'une composition de polynômes

> [!objectif]
>$$
> \forall (P,Q)\in \mathbb{K}[X]^{2},(P\circ Q)'=Q'\times (P'\circ Q)
> $$
### Démonstration

Soit $n\in \mathbb{N}$ et $a_{0},\dots,a_{n}$ des réels non tous nuls. On note $\displaystyle P(X)=\sum_{k=0}^na_{k}X^k\in \mathbb{R}[X]$.
Soit $Q\in \mathbb{R}[X]$.
$$
\begin{align}
(P\circ Q)'&=\left( \sum_{k=0}^na_{k}Q^k \right)' \\
&=\sum_{k=0}^na_{k}(Q^k)' \\
&=\sum_{k=0}^n ka_{k}Q'Q^{k-1} \\
&=Q'\times \sum_{k=0}^nka_{k}Q^{k-1} \\
(P\circ Q)'&=Q'\times(P'\circ Q)
\end{align}
$$

#### Remarques


