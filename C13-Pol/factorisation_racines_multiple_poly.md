---
anki_linked: 0
raisonnements:
outils:
  - produits
  - polynome
kh_n:
display_title: Factorisations multiples par des racines
---
# Factorisations multiples par des racines

> [!objectif]
>$$
> \forall P\in \mathbb{K}[X], (\exists n\in \mathbb{N}^*,\forall \alpha \in(\alpha_{i})_{i\in[\![1,n]\!]},P(\alpha)=0)\implies \exists Q\in \mathbb{K}[X],P(X)=\left[ \prod_{i=1}^n(X-\alpha_{i}) \right]Q(X) 
> $$
### Démonstration

Soit $P\in \mathbb{K}[X]$. Soit $n\geq 1$ et on note $\alpha_{1},\dots,\alpha_{n}$ des racines distinctes.

Pour tout $k \in[\![0,n]\!]$, on pose $\displaystyle H_{k}: \exists Q_{k}\in \mathbb{K}[X],P(X)=\left[ \prod_{i=1}^k(X-\alpha_{i}) \right]Q_{k}(X)$
**Initialisation** : $Q_{0}(X)=P(X)$ convient, d'où $H_{0}$.

**Hérédité** : 
Soit $k \in[\![0,n-1]\!]$. 
On suppose $H_{k}$, donc il existe $Q_{k}\in \mathbb{K}[X]$ tel que $P(X)=\left[ \prod_{i=1}^k(X-\alpha_{i}) \right]Q_{k}(X)$
Alors :
$$
\underbrace{ P(\alpha_{k+1}) }_{ =\, 0 }=\underbrace{ \left[ \prod_{i=1}^k (\alpha_{k+1}-\alpha_{i})\right] }_{ \neq\, 0\text{ car distincts} }Q_{k}(\alpha_{k+1}) 
$$
On en déduit que $Q_{k}(\alpha_{k+1})=0$, donc $\alpha_{k+1}$ est une racine de $Q_{k}$.
Ainsi il existe $Q_{k+1}\in \mathbb{K}[X]$ tel que $Q_{k}(X)=(X-\alpha_{k+1})Q_{k+1}(X)$.
Donc :
$$
P(X)=\left[ \prod_{i=1}^k(X-\alpha_{i}) \right](X-\alpha_{k+1})Q_{k+1}(X)=\left[ \prod_{i=1}^{k+1}(X-\alpha_{i}) \right] Q_{k+1}(X) 
$$
D'où $H_{k+1}$.

#### Remarques


