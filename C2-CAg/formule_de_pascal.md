---
anki_linked: 1
raisonnements:
  - disjonction_de_cas
outils:
  - binom
  - factorielle
kh_n:
---
# Formule de Pascal

> [!objectif]
> Soit $(n,p)\in \mathbb{N}^{2}$
>$$
> {n+1 \choose p+1}={n \choose p+1}+{n \choose p}
> $$
### Démonstration

Soit $0\le p \leq n$ des entiers.

**Si $p=n$ :**
	Alors ${n \choose p+1}={n \choose n+1}=0$
	Donc ${n \choose p+1}+{n \choose p}={n \choose p}={n \choose n}=0={n+1 \choose n+1}={n+1 \choose p+1}$

**Sinon $0\leq p<n$ :**
	Donc $0\leq p+1\leq n$, donc :
$$
\begin{align}
{n \choose p+1}+{n \choose p}&=\frac{n!}{p!(n-p)!}+\frac{n!}{(p+1)!(n-(p+1))!} \\
&=\frac{(p+1)n!+(n-p)n!}{(p+1)!(n-p)!} \\
&=\frac{(n+1)!}{(p+1)!(n-p)!} \\
{n \choose p+1}+{n \choose p}&={n+1 \choose p+1}
\end{align}
$$


#### Remarques


