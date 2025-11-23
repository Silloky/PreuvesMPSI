---
anki_linked: 0
raisonnements:
outils:
  - suites
kh_n:
  - "7"
display_title: Théorème des gendarmes
---
# Théorème des gendarmes

> [!objectif]
> $$
\begin{cases}
u_{n}\to l \\
w_{n}\to l \\
u_{n}\leq v_{n} \leq w_{n} \; APCR
\end{cases} \implies v_{n} \to l
$$
### Démonstration

*On suppose les hypothèses vérifiées.*

Soit $\varepsilon>0$.
* $u_{n}\leq v_{n}\leq w_{n}\; APCR$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},u_{n}\leq v_{n}\leq w_{m}$
* $u_{n}\to l$ donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, |u_{n}-l|\leq\varepsilon$, donc $l-\varepsilon\leq u_{n}$
* $w_{n}\to l$ donc il existe $N_{3}\in \mathbb{N}$ tel que $\forall n\geq N_{3}, |w_{n}-l|\leq\varepsilon$, donc $w_{m}\leq l+\varepsilon$
Soit $n\geq \max(N_{1},N_{2},N_{3})$.
Alors $l-\varepsilon\leq u_{n}\leq v_{n}\leq w_{m}\leq l+\varepsilon$, donc $|v_{n}-l|\leq\varepsilon$.
Ainsi $v_{n}\to l$

#### Remarques


