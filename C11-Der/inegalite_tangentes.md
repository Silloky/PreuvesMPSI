---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - derivation
kh_n:
  - "11"
display_title: Inégalité des tangentes
---
# Inégalité des tangentes

> [!objectif]
> Soit $I$ un intervalle et $f:I\to \mathbb{R}$
> 
> "$f$ convexe sur $I$" $\iff$ "la courbe représentative de $f$ est au-dessus ses tangentes"
### Démonstration

***Sens $\implies$*** :
On suppose $f$ convexe sur $I$.
Soit $a\in I$ et $x \in I$. On suppose $x>a$ (le cas $a<x$ est similaire et le cas $x=a$ est évident).
D'après l'inégalité des pentes :
$$
\forall t\in]a,x[, \frac{f(t)-f(a)}{t-a}\leq \frac{f(x)-f(a)}{x-a}
$$
Donc par passage à la limite :
$$
f'(a)=\lim_{ t \to a^+ } \frac{f(t)-f(a)}{t-a}\leq \frac{f(x)-f(a)}{x-a} 
$$
Or $x-a>0$ donc $f'(a)(x-a)\leq f(x)-f(a)$, et enfin $f(x)=f'(a)(x-a)+f(a)$, ce qu'on reconnaît être l'expression de la tangente à la courbe représentative de $f$ au point $a$.

***Sens $\impliedby$*** :
On suppose que la courbe de $f$ est au-dessus de toutes ses tangentes.
Soit $(a,b)\in I^{2}$. On suppose $a<b$.
Par hypothèse, $f(b)\geq f'(a)(a-b)+f(a)$, donc $f'(a)\leq\frac{f(b)-f(a)}{b-a}$.
Et de même, $f(a)\geq f'(b)(a-b)+f(b)$, donc $\frac{f(b)-f(a)}{b-a}\leq f'(b)$.
Donc :
$$
f'(a)\leq \frac{f(b)-f(a)}{b-a}\leq f'(b)
$$
D'où $f'$ est croissante, donc $f$ est convexe.

#### Remarques


