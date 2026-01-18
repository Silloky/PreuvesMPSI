---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Degré de la dérivée d'un polynôme
---
# Degré de la dérivée d'un polynôme

> [!objectif]
> Soit $\displaystyle P(X)=\sum_{k=0}^na_{k}X^k\in \mathbb{K}[X]$. Alors $P'(X)=P(X)'=\sum_{k=1}^nka_{k}X^{k-1}$ et :
>$$
> \deg(P')=\begin{cases}
\deg(P)-1 & \text{si } P\not\in \mathbb{K}_{0}[X] \\
-\infty & \text{si }P\in \mathbb{K}_{0}[X]
\end{cases}
> $$
### Démonstration

**Si $P$ est constante** : alors $P'=0$ donc $\deg(P')=-\infty$.
**Sinon** :
On note $n=\deg(P)\geq 1$ et $a_{0},\dots,a_{n}$ ses coefficients (non tous nuls, avec $a_{n}\neq 0$).
Donc :
$$
P'(X)=\sum_{k=1}^nka_{k}X^{k-1}=\sum_{k=0}^{n-1}(k+1)a_{k+1}X^k
$$
Or $((n-1)+1)a_{(n-1)+1}=na_{n}\neq 0$
Donc $\deg(P')=n-1=\deg(P)-1$.

#### Remarques


