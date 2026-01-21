---
anki_linked: 0
raisonnements:
outils:
  - matrices
  - sommes
kh_n:
display_title: Associativité du produit matriciel
---
# Associativité du produit matriciel

> [!objectif]
>$$
> \forall(n,p,q,r)\in(\mathbb{N}^*)^{4}, \forall(A,B,C)\in \mathcal{M}_{n,p}(\mathbb{K})\times \mathcal{M}_{p,q}(\mathbb{K})\times \mathcal{M}_{q,r}(\mathbb{K}),A(BC)=(AB)C
> $$
### Démonstration

Soit $(n,p,q,r)\in(\mathbb{N}^*)^4$ et $(A,B,C)\in \mathcal{M}_{n,p}(\mathbb{K})\times \mathcal{M}_{p,q}(\mathbb{K})\times \mathcal{M}_{q,r}(\mathbb{K})$.

$A$ est de taille $(n,p)$ et $B$ de taille $(p,q)$ donc $AB$ existe et est de taille $(n,q)$ ; or $C$ est de taille $(q,r)$ donc $(AB)C$ existe et est de taille $(n,r)$.
Or $BC$ existe et est de taille $(p,r)$, donc $A(BC)$ existe et est de taille $(n,r)$.
D'où $A(BC)$ et $(AB)C$ sont de même taille $(n,r)$.

Soit $(i,j)\in [\![1,n]\!]\times [\![1,r]\!]$.
$$
\begin{align}
[A(BC)]_{ij}&=\sum_{k=1}^p[A]_{ik}[BC]_{kj} \\
&=\sum_{k=1}^p[A]_{ik}\left( \sum_{k'=1}^q[B]_{kk'}[C]_{k'j} \right) \\
&=\sum_{k=1}^p\sum_{k'=1}^q[A]_{ik}[B]_{kk'}[C]_{k'j} \\
&=\sum_{k'=1}^q\left( \sum_{k=1}^p[A]_{ik}[B]_{kk'} \right) [C]_{k'j} \\
&=\sum_{k'=1}^q[AB]_{ik'}[C]_{k'j} \\
[A(BC)]_{ij}&=[(AB)C]_{ij}
\end{align}
$$

#### Remarques


