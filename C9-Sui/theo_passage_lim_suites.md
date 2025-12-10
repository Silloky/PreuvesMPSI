---
anki_linked: 1
raisonnements:
  - absurde
outils:
  - suites
kh_n:
  - "7"
display_title: Théorème du passage à la limite (suites)
---
# Théorème du passage à la limite (suites)

> [!objectif]
> Si une suite $(u_{n})$ tend vers $l$ et que $u_{n}\leq M\;APCR$, alors $l\leq M$
### Démonstration

Par l'absurde, on suppose que $l>M$.
On pose $\varepsilon=\frac{l-M}{2}>0$.
D'après les hypothèses :
* il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq\varepsilon$ donc $u_{n}\geq l-\varepsilon$
* il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},u_{n}\leq M$
On pose $N=\max(N_{1},N_{2})$ et alors :
$$
u_{N}\leq \underbrace{ M<l-\varepsilon }_{ \varepsilon=\frac{l-M}{2}<l-M }\leq u_{N}
$$
Donc $u_{N}<u_{N}$ ce qui est absurde.
Donc $l\leq M$

#### Remarques


