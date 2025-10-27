---
anki_linked: 1
raisonnements:
  - recurrence
outils:
  - sommes
  - binom
kh_n:
  - "1"
---
# Formule du binôme de Newton

> [!objectif]
>$$
> \forall n\in \mathbb{N},\forall(a,b)\in \mathbb{R}^{2},(a+b)^n=\sum_{k=0}^{n}{n \choose k}a^kb^{n-k}
> $$
### Démonstration

Soit $(a,b)\in \mathbb{R}^{2}$
Pour tout $n\in \mathbb{N}$, on pose $H_{n}:(a+b)^n=\sum_{k=0}^{n}{n \choose k}a^kb^{n-k}$

*Initialisation* :
En $0$ : $(a+b)^0=1$ et $\sum_{k=0}^{0}{0 \choose k}a^kb^{0-k}={0 \choose 0}a^0b^0=1$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée en $0$.

*Hérédité* :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$$
\begin{align}
(a+b)^{n+1}&=(a+b)(a+b)^n \\
&=(a+b)\sum_{k=0}^{n}{n \choose k}a^kb^{n-k} \\
&=\sum_{k=0}^{n}{n \choose k}a^{k+1}b^{n-k}+\sum_{k=0}^{n}{n \choose k}a^kb^{n+1-k} \\
&=\sum_{k=1}^{n+1}{n \choose k-1}a^kb^{n+1-k}+\sum_{k=0}^{n}{n \choose k}a^kb^{n+1-k} \\
&=\sum_{k=1}^{n}{n \choose k-1}a^kb^{n+1-k}+{n \choose n}a^{k+1}b^0+{n\choose 0}a^0b^{n+1}+\sum_{k=1}^{n}{n \choose k}a^kb^{n+1-k} \\
&={n \choose n}a^{k+1}b^0+{n\choose 0}a^0b^{n+1}+\sum_{k=1}^{n} \left( {n \choose k-1}+{n \choose k} \right)a^kb^{n+1-k} \\
&={n+1 \choose n+1}a^{k+1}b^0+{n+1\choose 0}a^0b^{n+1}+\sum_{k=1}^{n} {n+1 \choose k}a^kb^{n+1-k} \\
&=\sum_{k=0}^{0} {n+1 \choose k}a^kb^{n+1-k}+\sum_{k=1}^{n} {n+1 \choose k}a^kb^{n+1-k}+\sum_{k=n+1}^{n+1} {n+1 \choose k}a^kb^{n+1-k} \\
(a+b)^{n+1}&=\sum_{k=0}^{n+1}{n+1 \choose k}a^kb^{(n+1)-k}
\end{align}
$$
Donc $H_{n+1}$ est vraie, donc $H_{n}$ est héréditaire.

*Conclusion* :
$$
\forall n\in \mathbb{N},\forall(a,b)\in \mathbb{R}^{2},(a+b)^n=\sum_{k=0}^{n}{n \choose k}a^kb^{n-k}
$$

#### Remarques


