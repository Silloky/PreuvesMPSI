---
anki_linked: 1
raisonnements:
  - recurrence
outils:
  - sommes
kh_n:
  - "1"
---
# Somme des $n$ premiers entiers

> [!objectif]
>$$
> \forall n\in \mathbb{N},\sum_{k=0}^{n}k=\frac{n(n+1)}{2}
> $$
### Démonstration
##### 1. Par récurrence

Pour tout $n\in \mathbb{N}$, on pose $H_{n}:\sum_{k=0}^{n}k=\frac{n(n+1)}{2}$

*Initialisation* :
En $0$ : $\sum_{k=0}^{0}k=0$ et $\frac{0(0+1)}{2}=0$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée en $0$.

*Hérédité* :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$$
\begin{align}
\sum_{k=0}^{n+1}k&=\sum_{k=0}^{n}k+(n+1) \\
&=\frac{n(n+1)}{2}+\frac{2n+2}{2} \tag*{par hypothèse de récurrence}\\
&=\frac{n^{2}+3n+2}{2} \\
\sum_{k=0}^{n+1}k&=\frac{(n+1)((n+1)+1)}{2}
\end{align}
$$
Donc $H_{n+1}$ est vraie et $H_{n}$ est héréditaire.

*Conclusion* :
$$
\forall n\in \mathbb{N},\sum_{k=0}^{n}k=\frac{n(n+1)}{2}
$$
##### 2. Par téléscopage (M-TD2-5)

On pose $S=\sum_{k=0}^n((k+1)^{2}-k^{2})$.

D'une part, par téléscopage, $S=(n+1)^{2}-0^{2}=(n+1)^{2}=n^{2}+2n+1$.

De plus, $(k+1)^{2}-k^{2}=2k+1$, donc $S=\sum_{k=0}^n(2k+1)=n+1+2\sum_{k=0}^nk$.
Donc :
$$\sum_{k=0}^nk=\frac{S-n-1}{2}=\frac{n^{2}+2n+1-n-1}{2}=\frac{n^{2}+n}{2}=\frac{n(n+1)}{2}$$
#### Remarques


