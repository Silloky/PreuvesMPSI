---
anki_linked: 0
raisonnements:
outils:
  - sommes
  - binom
kh_n:
  - "1"
---
# Calculer $\sum_{k=0}^{n}k{n \choose k}$

> [!objectif]
>$$
> \forall n\in \mathbb{N},\quad\sum_{k=0}^{n}k{n \choose k}=n\times2^{n-1}
> $$
### Démonstration

Soit $n\in \mathbb{N}$. Par la formule du [[formule_du_capitaine|capitaine]] :
$$
\sum_{k=0}^{n}k{n \choose k}=\sum_{k=0}^nn{n-1\choose k-1}=n\sum_{k=0}^n{n-1 \choose k-1}=n\times2^{n-1}
$$

#### Remarques


