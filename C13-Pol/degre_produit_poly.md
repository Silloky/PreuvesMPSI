---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Degré d'un produit de polynômes
---
# Degré d'un produit de polynômes

> [!objectif]
>$$
> \forall(P,Q)\in \mathbb{K}[X]^{2},\deg(PQ)=\deg(P)+\deg(Q)
> $$
### Démonstration

Soit $(P,Q)\in \mathbb{K}[X]^{2}$.

**Si $P=0$** :
Alors $PQ=0$ donc $\deg(PQ)=-\infty$, et $\deg(P)+\deg(Q)=-\infty+\deg(Q)=-\infty$.
D'où $\deg(PQ)=\deg(P)+\deg(Q)$.

**Si $Q=0$** : de même.

**Si $P\neq 0$ et $Q\neq 0$** :
On pose $n_{1}=\deg(P)$ et $n_{2}=\deg(Q)$. Alors :
$$
\begin{align}
\forall n>n_{1}+n_{2}, [PQ]_{n}&=\sum_{k=0}^n[P]_{k}[Q]_{n-k} \\
&=\sum_{k=0}^{n_{1}}[P]_{k}[Q]_{n-k} & \text{car si $k\geq n_{1}$ alors $[P]_{k}=0$ } \\
[PQ]_{n}&=0 & \text{car $k\leq n$ donc $n-k\geq n-n_{1}>n_{2}$ d'où $[Q]_{k}=0$}
\end{align}
$$
Ainsi $\deg(PQ)\leq n_{1}+n_{2}$.
De plus :
$$
\begin{align}
[PQ]_{n_{1}+n_{2}}&=\sum_{k=0}^{n_{1}+n_{2}}[P]_{k}[Q]_{n_{1}+n_{2}-k} \\
&=\underbrace{ \sum_{k=0}^{n_{1}-1}[P]_{k}[Q]_{n_{1}+n_{2}-k} }_{ =\,0 }+\underbrace{ [P]_{n_{1}}[Q]_{n_{2}} }_{ \neq\,0 }+\underbrace{ \sum_{k=n_{1}+1}^{n_{1}+n_{2}}[P]_{k}[Q]_{n_{1}+n_{2}-k} }_{ =\, 0 } \\
[PQ]_{n_{1}+n_{2}}&\neq 0
\end{align}
$$
Le coefficient de rang $n_{1}+n_{2}$ est non nul ; on en déduit que $\deg(PQ)=n_{1}+n_{2}$.

Donc dans tous les cas, $\deg(PQ)=\deg(P)+\deg(Q)$.
#### Remarques


