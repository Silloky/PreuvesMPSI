---
anki_linked: 1
raisonnements:
  - absurde
outils:
  - sous-suites
  - suites
kh_n:
  - "8"
display_title: Convergence de (u_{2n}) et (u_{2n+1}) vers une limite différente
---
# Convergence de $(u_{2n})$ et $(u_{2n+1})$ vers une limite différente

> [!objectif]
> Soit $(u_{n})$ une suite réelle et $l\in \mathbb{R}$.
> Si $u_{2n}\to l$ et $u_{2n+1}\to l'$ avec $l\neq l'$, alors $(u_{n})$ est divergente.
### Démonstration

Par l'absurde, on suppose $(u_{n})$ convergente et on note $\alpha$ sa limite.
$(u_{2n})$ et $(u_{2n+1})$ sont des sous-suites de $(u_{n})$ car $n\mapsto 2n$ et $n \mapsto 2n+1$ sont des extractions.
Ainsi $u_{2n}\to\alpha$ et $u_{2n+1}\to\alpha$.
Donc $\alpha=l$ et $\alpha=l'$, donc $l=l'$, ce qui est absurde.
Donc $(u_{n})$ est convergente.

#### Remarques

Il faut que $(u_{13n})$ soit aussi convergente pour que $(u_{n})$ soit aussi convergente : [[u_2n_u_2n+1_u_13_n_convergentes|preuve]].
