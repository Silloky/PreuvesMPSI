---
anki_linked: 1
raisonnements:
outils:
  - sous-suites
  - suites
  - limites
kh_n:
  - "8"
display_title: Convergence de (u_{2n}), (u_{2n+1}) et (u_{13n})
---
# Convergence de $(u_{2n})$, $(u_{2n+1})$ et $(u_{13n})$

> [!objectif]
> Soit $(u_{n})$ une suite réelle et $(l,l',l'')\in \mathbb{R}^{3}$.
> On suppose que $(u_{2n})\to l$, $u_{2n+1}\to l'$ et $u_{13n}\to l''$.
> Alors $(u_{n})\to l=l'=l''$
### Démonstration

$(u_{26n})=(u_{13(2n)})=(u_{2(13n)})$.
Or $(u_{13(2n)})$ est une sous-suite de $(u_{13n})$, donc $(u_{26n})\to l''$
Mais $(u_{2(13n)})$ est une sous-suite de $(u_{2n})$ donc $(u_{26n})\to l$.
Par unicité de la limite, $l=l''$.

$(u_{26n+13})=(u_{13(2n+1)})=(u_{2(13n+6)+1})$
Or $(u_{13(2n+1)})$ est une sous-suite de $(u_{13n})$, donc $(u_{26n+13})\to l''$.
Mais $(u_{2(13n+6)+1})$ est une sous-suite de $(u_{2n+1})$, donc $(u_{26n+13})\to l'$.
Par unicité de la limite, $l'=l''$.

Donc $l=l'$, ainsi $(u_{2n})$ et $(u_{2n+1})$ convergent vers une même limite.
Donc ([[u_2n_u_2n+1_convrg_meme_lim|preuve]]) $(u_{n})\to l$

#### Remarques


