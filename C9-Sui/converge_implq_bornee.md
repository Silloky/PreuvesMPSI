---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - suites
kh_n:
  - "7"
display_title: Convergente => Bornée
---
# $u$ convergente $\implies$ $u$ bornée

> [!objectif]
> Si une suite $u$ est convergente, alors elle est bornée
### Démonstration

On suppose $u$ convergente.
Or $1>0$ et $u_{n}\to l$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N,|u_{n}-l|\leq 1$.
On pose $M=\max(|u_{0}|,|u_{1}|,\dots,|u_{N-1}|,1+|l|)$

Soit $n\in \mathbb{N}$.
Si $n\leq N-1$ : $|u_{n}|\leq M$
Si $n\geq N$ : 
$$
\begin{align}
|u_{n}|&=|u_{n}-l+l| \\
&\leq|u_{n}-l|+|l| \\
&\leq 1+|l| \\
|u_{n}|&\leq M
\end{align}
$$
Donc dans tous les cas $\forall n\in \mathbb{N}, |u_{n}|\leq M$, donc $u$ est bornée.

#### Remarques


