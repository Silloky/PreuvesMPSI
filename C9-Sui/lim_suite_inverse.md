---
anki_linked: 0
raisonnements:
outils:
  - suites
  - limites
kh_n:
display_title: Limite de 1/n
---
# Limite de $\frac{1}{n}$

> [!objectif]
> $$\frac{1}{n}\to 0$$
### Démonstration

Soit $\varepsilon>0$. On pose $N=\left\lfloor  \frac{1}{\varepsilon}  \right\rfloor+1$.
Soit $n\geq N$, donc :
$$
\begin{align}
n&\geq \left\lfloor  \frac{1}{\varepsilon}  \right\rfloor +1 \\
n&>\left\lfloor  \frac{1}{\varepsilon}  \right\rfloor  \\
n&> \frac{1}{\varepsilon} \\
\frac{1}{n}&<\varepsilon \\
\left| \frac{1}{n}-0 \right| &< \varepsilon
\end{align}
$$
Donc il existe bien $N\in \mathbb{N}$ tel que $\forall n\geq N, \frac{1}{n}<\varepsilon$.
Donc $\frac{1}{n}\to 0$

#### Remarques


