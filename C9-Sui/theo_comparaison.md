---
anki_linked: 0
raisonnements:
outils:
  - suites
kh_n:
  - "7"
display_title: Théorème de comparaison
---
# Théorème de comparaison (du gendarme)

> [!objectif]
> $$
\begin{cases}
u_{n}\leq v_{n}\; APCR \\
u_{n}\to +\infty
\end{cases} \implies v_{n}\to +\infty
$$
### Démonstration

*On suppose les hypothèses vérifiées.*
Soit $M\in \mathbb{R}$.
* $u_{n}\leq v_{n}\;APCR$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},u_{n}\leq v_{n}$
* $u_{n}\to +\infty$ donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},M\leq u_{n}$
Soit $n\geq \max(N_{1},N_{2})$. Alors $M\leq u_{n}\leq v_{n}$, donc $v_{n}\geq M$.
Ainsi $v_{n}\to +\infty$

#### Remarques


