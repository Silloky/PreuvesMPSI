---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Dérivée du produit polynomial
---
# Dérivée du produit polynomial

> [!objectif]
>$$
> \forall(P,Q)\in \mathbb{K}[X]^{2},(PQ)'=P'Q+PQ'
> $$
### Démonstration

Soit $(n,n')\in \mathbb{N}^{2}$ et $a_0,\dots,a_{n}$ et $b_{0},\dots,b_{n}$ des réels.
On note :
$$
P(X)=\sum_{k=0}^na_{k}X^k\qquad Q(X)=\sum_{i=0}^{n'}b_{i}X^{i}
$$
Pour tout $k\in \mathbb{N}^*$ :
$$
\begin{align}
(X^{k}Q(X))'&=\left( \sum_{i=0}^{n'}b_{i}X^{i+k} \right)' \\
&=\sum_{i=0}^{n'}(i+k)b_{i}X^{i+k-1} \\
&=\sum_{i=0}^{n'}ib_{i}X^{i+k-1}+\sum_{i=0}^{n'}kb_{i}X^{i+k-1} \\
&=X^{k}\sum_{i=0}^{n'}ib_{i}X^{i-1}+kX^{k-1}\sum_{i=0}^{n'}b_{i}X^{i} \\
(X^{k}Q(X))'&=X^{k}Q'(X)+kX^{k-1}Q(X)
\end{align}
$$
D'où :
$$
\begin{align}
(PQ)'&=\left( \sum_{k=0}^{n}a_{k}X^kQ(X) \right)' \\
&=\sum_{k=0}^{n}a_{k}(X^kQ(X))' \\
&=\sum_{k=0}^{n}\left( a_{k}X^kQ'(X)+a_{k}kX^{k-1}Q(X)  \right) \\
&=\left( \sum_{k=0}^n a_{k}X^{k}\right)Q'(X)+\left( \sum_{k=0}^{n}a_{k}kX^{k-1} \right)Q(X) \\
(PQ)'&=PQ'+P'Q
\end{align}
$$

#### Remarques


