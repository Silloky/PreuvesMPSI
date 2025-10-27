---
anki_linked: 1
raisonnements:
outils:
  - binom
  - factorielle
kh_n:
---
# Formule du capitaine

> [!objectif]
> Soit $(n,p)\in \mathbb{N}$
>$$
> p{n \choose p}=n{n-1 \choose p-1}
> $$

### Démonstration

Soit $0\leq p\leq n$ des entiers.
$$
\begin{align}
p{n \choose p}&=p\times \frac{n!}{p!(n-p)!} \\
&=\frac{n!}{(p-1)!(n-p)!} \\
&=n\times \frac{(n-1)!}{(p-1)!(n-p)!} \\
p{n \choose p}&=n{n-1 \choose p-1}
\end{align}
$$

#### Remarques


