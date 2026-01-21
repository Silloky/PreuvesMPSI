---
anki_linked: 0
raisonnements:
outils:
  - matrices
  - sommes
kh_n:
display_title: Distributivité du produit matriciel
---
# Distributivité du produit matriciel

> [!objectif]
>$$
>\begin{gather}
\forall(n,p,q)\in (\mathbb{N}^*)^{3},\forall A\in \mathcal{M}_{n,p}(\mathbb{K}), \forall(B,C)\in \mathcal{M}_{p,q}(\mathbb{K})^2, \\  \\\begin{cases}
A(B+C)=AB+AC \\
(B+C)A=BA+CA
\end{cases}
\end{gather}
> $$
### Démonstration

Soit $(n,p,q)\in(\mathbb{N}^*)^{3}$ et $A\in \mathcal{M}_{n,p}(\mathbb{K})$, $(B,C)\in \mathcal{M}_{p,q}(\mathbb{K})^{2}$.

$B$ et $C$ sont de taille $(p,q)$ donc $B+C$ est de taille $(p,q)$.
Or $A$ est de taille $(n,p)$, donc $A(B+C)$ existe et est de taille $(p,q)$.
D'autre part $AB$ et $AC$ sont de taille $(n,q)$, donc leur somme l'est aussi.
Donc $A(B+C)$ et $AB+AC$ sont de même taille $(n,q)$.

Soit $(i,j)\in [\![1,n]\!]\times [\![1,q]\!]$
$$
\begin{align}
[A(B+C)]_{ij}&=\sum_{k=1}^p[A]_{ik}[B+C]_{kj} \\
&=\sum_{k=1}^p[A_{ik}]([B]_{kj}+[C]_{kj}) \\
&=\sum_{k=1}^p[A]_{ik}[B]_{kj}+\sum_{k=1}^p[A]_{ik}[C]_{kj} \\
&=[AB]_{ij}+[AC]_{ij} \\
[A(B+C)]_{ij}&=[AB+AC]_{ij}
\end{align}
$$

**Et de même pour l'autre sens du développement.**

#### Remarques


