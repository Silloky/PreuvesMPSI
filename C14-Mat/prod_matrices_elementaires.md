---
anki_linked: 0
raisonnements:
outils:
  - matrices
kh_n:
display_title: Produit de matrices élémentaires
---
# Produit de matrices élémentaires

> [!objectif]
>$$
> \forall(i_{1},j_{1},i_{2},j_{2})\in [\![1,n]\!]^{4},E_{i_{1}j_{1}}\times E_{i_{2}j_{2}}=\delta_{j_{1}i_{2}}E_{i_{1}j_{2}}
>  $$
### Démonstration

Soit $(i_{1},j_{1},i_{2},j_{2})\in [\![1,n]\!]^4$.
Soit $(i,j)\in[\![1,n]\!]^{2}$.
$$
\begin{align}
[E_{i_{1}j_{1}}\times E_{i_{2}j_{2}}]_{ij}&=\sum_{k=1}^n[E_{i_{1}j_{1}}]_{ik}[E_{i_{2}j_{2}}]_{kj} \\
&=\sum_{k=1}^n (\delta_{i_{1}i}\delta_{j_{1}k})(\delta_{i_{2}k}\delta_{j_{2}j}) \\
&=\delta_{i_{1}i}\delta_{i_{2}j_{1}}\delta_{j_{2}j} \\
&=\delta_{i_{2}j_{1}}[E_{i_{1}j_{2}}]_{ij} \\
[E_{i_{1}j_{1}}\times E_{i_{2}j_{2}}]_{ij}&=[\delta_{i_{2}j_{1}}E_{i_{1}j_{2}}]_{ij}
\end{align}
$$

#### Remarques


