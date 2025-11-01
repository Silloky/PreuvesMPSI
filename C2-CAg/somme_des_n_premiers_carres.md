---
anki_linked: 1
raisonnements:
  - recurrence
outils:
  - sommes
kh_n:
  - "1"
---
# Somme des $n$ premiers carrés

> [!objectif]
>$$
> \forall n\in \mathbb{N},\sum_{k=0}^{n}k^{2}=\frac{n(n+1)(2n+1)}{6}
> $$
### Démonstration
##### 1. Par récurrence

Pour tout $n\in \mathbb{N}$, on pose $H_{n}:\sum_{k=0}^{n}k^{2}=\frac{n(n+1)(2n+1)}{6}$

***Initialisation*** :
En $0$ : $\sum_{k=0}^{0}k^2=0$ et $\frac{0(0+1)(2\times0+1)}{6}=0$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée en $0$.

***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$$
\begin{align}
\sum_{k=0}^{n+1}k^2&=\sum_{k=0}^{n}k^2+(n+1)^2 \\
&=\frac{n(n+1)(2n+1)}{6}+\frac{6(n^{2}+2n+1)}{6} \tag*{par hypothèse de récurrence}\\
&=\frac{2n^3+9n^2+13n+6}{6} \\
\sum_{k=0}^{n+1}k^2&=\frac{(n+1)((n+1)+1)(2(n+1)+1)}{6}
\end{align}
$$
Donc $H_{n+1}$ est vraie et $H_{n}$ est héréditaire.

***Conclusion*** :
$$
\forall n\in \mathbb{N},\sum_{k=0}^{n}k^{2}=\frac{n(n+1)(2n+1)}{6}
$$
##### 2. Par téléscopage (M-TD2-5)

Soit $n\in \mathbb{N}$. On pose $S=\sum_{k=0}^n((k+1)^{3}-k^{3})$.

D'une part, par téléscopage, $S=(n+1)^{3}-0^{3}=(n+1)^{3}$.

De plus, $\forall k\in \mathbb{N},(k+1)^{3}-k^{3}=3k^{2}+3k+1$, donc :
$$
\begin{align}
S&=\sum_{k=0}^n(3k^{2}+3k+1) \\
&=3\sum_{k=0}^{n}k^{2}+3\sum_{k=0}^{n}k+\sum_{k=0}^{n}1 \\
S&=3\sum_{k=0}^{n}k^{2}+\frac{3n(n+1)}{2}+n+1
\end{align}
$$
Donc :
$$
\begin{align}
3\sum_{k=0}^nk^{2}&=(n+1)^3-\frac{3n(n+1)}{2}-(n+1) \\
&=(n+1)\left[ (n+1)^{2}-\frac{3n}{2}-1 \right]  \\
&=(n+1)\left( \frac{2n^{2}+n}{2} \right)  \\
3\sum_{k=0}^nk^{2}&=\frac{n(n+1)(2n+1)}{2}
\end{align}
$$
Enfin : $$\sum_{k=0}^{n}k^{2}=\frac{n(n+1)(2n+1)}{6}$$
#### Remarques


