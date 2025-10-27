---
anki_linked: 0
raisonnements:
  - recurrence
outils:
  - sommes
---
# Somme des $n$ premiers cubes

> [!objectif]
>$$
> \forall n\in \mathbb{N},\sum_{k=0}^{n}k^{3}=\left( \sum_{k=0}^{n}k \right)^2=\left( \frac{n(n+1)}{2} \right)^2 
> $$
### Démonstration

Pour tout $n\in \mathbb{N}$, on pose $H_{n}:\sum_{k=0}^{n}k^{2}=\left( \sum_{k=0}^{n}k \right)^2$

*Initialisation* :
En $0$ : $\sum_{k=0}^{0}k^3=0$ et $\left( \sum_{k=0}^{0}k \right)^2=0$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée en $0$.

*Hérédité* :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$$
\begin{align}
\sum_{k=0}^{n+1}k^3&=\sum_{k=0}^{n}k^3+(n+1)^3 \\
&=\left( \sum_{k=0}^{n}k \right)^2+\frac{4n^3+12n^2+12n+4}{4} \tag*{par HR}\\
&=\left( \frac{(n+1)(n+2)}{2} \right)^2 \\
\sum_{k=0}^{n+1}k^3&=\left( \sum_{k=0}^{n+1}k \right)^2
\end{align}
$$
Donc $H_{n+1}$ est vraie et $H_{n}$ est héréditaire.

*Conclusion* :
$$
\forall n\in \mathbb{N},\sum_{k=0}^{n}k^{2}=\left( \sum_{k=0}^{n}k \right)^2
$$

#### Remarques


