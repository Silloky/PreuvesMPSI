---
anki_linked: 0
raisonnements:
outils:
kh_n:
display_title: Degré d'une composition de polynômes
---
# Degré d'une composition de polynômes

> [!objectif]
>$$
> \forall (P,Q)\in \mathbb{K}[X]^{2},\quad \deg(Q)\geq 1\implies \deg(P\circ Q)=\deg(P)\times \deg(Q)
> $$
### Démonstration

On suppose $\deg(Q)\geq 1$.

**Si $P=0$** : alors $P\circ Q=0$ donc $\deg(P\circ Q)=-\infty$ et $\deg(P)\times \deg(Q)=-\infty \times \underbrace{ \deg(Q) }_{ \geq\,1 }=-\infty$.
Donc $\deg(P\circ Q)=\deg(P)\times \deg(Q)$.

**Sinon** :
On note $n$ le degré de $P$ et $\lambda$ son coefficient dominant. Alors $\displaystyle P(X)=\lambda X^n+\sum_{k=0}^{n-1}[P]_{k}X^k$
Donc $\displaystyle P\circ Q=\lambda Q^n+\sum_{k=0}^{n-1}[P]_{k}Q^k$
Or $\deg(Q^k)=k\deg(Q)$, donc $\deg([P]_{k}Q^k)\in \{ k\deg(Q),-\infty \}$, d'où $\deg([P]_{k}Q^k)\leq k\deg(Q)$.
Donc en sommant, $\deg\left( \sum_{k=0}^{n-1}[P]_{k}Q^k \right)\leq(n-1)\deg(Q)$.
Or $\deg(Q)\geq 1> 0$ donc $\deg(\lambda Q^n)=n\deg(Q)>(n-1)\deg(Q)$

Donc $\deg(\lambda Q^n)\neq \deg \left( \sum_{k=0}^{n-1}[P]_{k}Q^k \right)$, d'où :
$$
\begin{align}
\deg(P\circ Q)&=\deg\left( \lambda Q^n+\sum_{k=0}^{n-1}[P]_{k}Q^k \right) \\
&=\max\left( \deg(\lambda Q^n),\deg\left( \sum_{k=0}^{n-1}[P]_{k}Q^k \right) \right) \\
&=\max(n\deg(Q),(n-1)\deg((Q))) \\
&=n\deg(Q) \\
\deg(P\circ Q)&=\deg(P)\deg(Q)
\end{align}
$$
D'où le résultat.
#### Remarques


