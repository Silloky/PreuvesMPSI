---
anki_linked: 1
raisonnements:
outils:
  - suites
  - limites
  - sous-suites
kh_n:
display_title: Convergence de sous-suites
---
# Convergence de sous-suites

> [!objectif]
> Si une suite converge alors toutes ses sous-suites convergent vers la même limite.
### Démonstration

Soit $(u_{n})$ une suite convergente et $(v_{n})$ une sous-suite de $(u_{n})$. 
Donc, on note $l$ la limite de $(u_{n})$, et il existe une extraction $\varphi$ telle que $\forall n \in \mathbb{N},v_{n}=u_{\varphi(n)}$.
Soit $\varepsilon>0$.
$u_{n}\to l$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N,|u_{n}-l|<\varepsilon$.
Soit $n\geq N$.
Or $\varphi(n)\geq n\geq N$ donc $|u_{\varphi(n)}-l|\leq\varepsilon$ et donc $|v_{n}-l|\leq\varepsilon$.
Ainsi $v_{n}\to l$

#### Remarques


