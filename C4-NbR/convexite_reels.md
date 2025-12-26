---
anki_linked: 0
raisonnements:
  - double_implication
outils:
kh_n:
  - "11"
display_title: Caractérisation de la convexité de R
---
# Caractérisation de la convexité de $\mathbb{R}$

> [!objectif]
> Soit $a<b$ deux réels.
>$$
> \forall x \in \mathbb{R},x \in[a,b]\iff \exists\lambda \in[0,1],x=\lambda a+(1-\lambda)b
> $$
### Démonstration

Soit $x \in \mathbb{R}$.

**Sens $\implies$** :
On suppose $x \in[a,b]$.
On pose $\lambda= \frac{b-x}{b-a}$, donc $x=\lambda a+(1-\lambda)b$
Or $x\geq a$ donc $-x\leq -a$ d'où $b-x\leq b-a$. De plus $x\leq b$, donc $0\leq b-x$
Donc $b-a>0$ et $0\leq \frac{b-x}{b-a}\leq 1$ donc $\lambda \in[0,1]$.

***Sens $\impliedby$*** :
On suppose qu'il existe $\lambda \in[0,1]$ tel que $x=\lambda a+(1-\lambda)b$.
Or :
* $a\leq b$ et $\lambda\geq 0$ donc $\lambda a\leq\lambda b$
* $a\leq b$ et $1-\lambda\geq 0$ donc $(1-\lambda)a\leq(1-\lambda)b$
Donc $\lambda a+(1-\lambda)a\leq\lambda a+(1-\lambda)b\leq\lambda b+(1-\lambda)b$, d'où $a\leq x\leq b$.
Ainsi $x \in[a,b]$

#### Remarques


