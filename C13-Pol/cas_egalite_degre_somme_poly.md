---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Cas d'égalité sur le degré d'une somme de polynômes
---
# Cas d'égalité sur le degré d'une somme de polynômes

> [!objectif]
>$$
> \forall(P,Q)\in \mathbb{K}[X]^{2}, \deg(P)\neq \deg(Q)\implies \deg(P+Q)=\max(\deg(P),\deg(Q))
> $$
### Démonstration

On suppose que $\deg(P)<\deg(Q)$ (le cas $\deg(P)>\deg(Q)$ est similaire).
On note $n=\deg(Q)\in \mathbb{N}$ car $\deg(Q)\in \mathbb{N}\cup \{ -\infty \}$ et $\deg(Q)>\deg(P)\geq-\infty$.
Or :
* $\deg(P+Q)\leq \max(\deg(P),\deg(Q))=\deg(Q)=n$
* $[P+Q]_{n}=\underbrace{ [P]_{n} }_{ =\,0 }+\underbrace{ [Q]_{n} }_{ \neq\,0 }\neq 0$
Ainsi $\deg(P+Q)=n=\max(\deg(P),\deg(Q))$.

#### Remarques


