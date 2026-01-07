---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
  - "12"
display_title: Produit de polynômes
---
# Produit de polynômes

> [!objectif]
> Le produit $P\times Q$ de deux polynômes $P=(a_{n})_{n\in\mathbb{N}}$ et $Q=(b_{n})_{n\in \mathbb{N}}$ est aussi un polynôme.
### Démonstration

Il faut démontrer que la suite $P\times Q=\left( \sum_{k=0}^na_{k}b_{n-k} \right)_{n\in \mathbb{N}}$ est nulle à partir d'une certain rang.
Or :
* $P=(a_{n})_{n\in \mathbb{N}}$ est un polynôme, donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},a_{n}=0$
* $Q=(b_{n})_{n\in \mathbb{N}}$ est un polynôme, donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, b_{n}=0$
Soit $n\geq N_{1}+N_{2}$.
Pour tout $k\geq N_{1},a_{n}=0$, donc :
$$
\sum_{k=0}^{n}a_{k}b_{n-k}=\sum_{k=0}^{N_{1}-1}a_{k}b_{n-k}
$$
Or pour tout $k\leq N_{1}-1$, $-k\geq 1-N_{1}$, donc $n-k\geq N_{1}+N_{2}+1-N_{1}=N_{2}+1\geq N_{2}$.
D'où, pour tout $k \in[\![0,N_{1}-1]\!]$, $b_{n-k}=0$.

Donc $P\times Q$ est nulle à partir du rang $N_{1}+N_{2}$

#### Remarques


