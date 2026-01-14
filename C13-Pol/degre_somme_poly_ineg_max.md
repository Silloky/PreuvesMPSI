---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Inégalité sur le degré de la somme de polynômes
---
# Inégalité sur le degré de la somme de polynômes

> [!objectif]
>$$
> \forall(P,Q)\in \mathbb{K}[X]^{2},\deg(P+Q)\leq \max(\deg(P),\deg(Q))
> $$
### Démonstration

Soit $(P,Q)\in \mathbb{K}[X]^{2}$.

**Si $P$ est nul** : 
Alors $P+Q=Q$, donc $\deg(P+Q)=\deg(Q)$, et $\max(\deg(P),\deg(Q))=\max(-\infty,\deg(Q))$, d'où $\deg(P+Q)\leq \max(\deg(P),\deg(Q))$.

**Si $Q$ est nul** : de même.

**Sinon** $P\neq 0$ et $Q\neq 0$.
On pose $n_{1}=\deg(P)$ et $n_{2}=\deg(Q)$. On pose $n=\max(n_{1},n_{2})$.
Alors $\forall k>n, [P+Q]_{k}=[P]_{k}+[Q]_{k}=0+0=0$
Donc $\deg(P+Q)\leq n$

#### Remarques


