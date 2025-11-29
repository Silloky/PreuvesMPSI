---
anki_linked: 1
raisonnements:
  - disjonction_de_cas
outils:
  - suites
  - limites
  - sous-suites
kh_n:
  - "8"
display_title: Convergence de (u_{2n}) et (u_{2n+1}) vers une même limite
---
# Convergence de $(u_{2n})$ et $(u_{2n+1})$ vers une même limite

> [!objectif]
> Soit $(u_{n})$ une suite réelle et $l\in \mathbb{R}$.
> Si $u_{2n}\to l$ et $u_{2n+1}\to l$, alors $(u_{n})\to l$
### Démonstration

Pour tout $n\in \mathbb{N}$, on pose : $v_{n}=u_{2n}$ et $w_{n}=u_{2n+1}$.
On suppose que $v_{n}\to l$ et $w_{n}\to l$.
 
Soit $\varepsilon> 0$.
* $v_{n}\to l$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|v_{n}-l|\leq \varepsilon$
* $w_{n}\to l$ donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},|w_{n}-l|\leq \varepsilon$.

Soit $n\geq \max(2N_{1},2N_{2}+1)$.

***Si $n$ est pair*** :
$|u_{n}-l|=|u_{2\times \frac{n}{2}}-l|\leq \varepsilon$
Or $n\geq 2N_{1}$, donc $\frac{n}{2}\geq N_1$ donc $|u_{n}-l|\leq\varepsilon$
***Si $n$ est impair*** :
$|u_{n}-l|=|u_{2\left( \frac{n-1}{2} \right)+1}-l|\leq\varepsilon$
Or $n\geq 2N_{2}+1$ donc $\frac{n-1}{2}\geq N_{2}$ donc $|u_{n}-l|\leq\varepsilon$

Donc dans tous les cas, $|u_{n}-l|\leq\varepsilon$.
Donc $u_{n}\to l$.

#### Remarques

Il faut dans ce cas que $v_{n}$ et $w_{n}$ convergent *vers la même limite*. Sinon ([[u_2n_u_2n+1_convrg_lim_differ|preuve]]) $u_{n}$ est divergente.
On peut remplacer cette condition par le fait $u_{13n}$ converge aussi : voir [[u_2n_u_2n+1_u_13_n_convergentes|cette preuve]].
