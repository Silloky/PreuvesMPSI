---
anki_linked: 0
raisonnements:
  - double_implication
  - disjonction_de_cas
outils:
  - limites
kh_n:
  - "9"
display_title: Limite en un réel et limite à gauche et droite
---
# Limite en un réel et limite à gauche et droite

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ une fonction et $a\in I$.
> On suppose $a\in \dot{I}$  ($a$ est à l'intérieur de $I$).
>$$
> f(x)\xrightarrow[x\to a]{}f(a)\iff \begin{cases}f(x)\xrightarrow[x\to a^-]{} f(a) \\ f(x)\xrightarrow[x\to a^+]{}f(a)
> \end{cases}
> $$
### Démonstration

***Sens $\implies$*** :
$I\cap]a,+\infty[\subset I$ et $I\cap]-\infty,a[$ donc c'est évident en utilisant les quantifications :
$$
(\forall \varepsilon>0,\exists \eta>0,\forall x \in I,|x-a|\leq \eta\implies |f(x)-f(a)|\leq\varepsilon)
$$
Equivaut à $(\forall \varepsilon>0,\exists \eta>0,\forall x \in I\cap]-\infty,a[,|x-a|\leq \eta\implies |f(x)-f(a)|\leq\varepsilon)$ et : $(\forall \varepsilon>0,\exists \eta>0,\forall x \in I\cap]a,+\infty[|x-a|\leq \eta\implies |f(x)-f(a)|\leq\varepsilon)$

D'où $f(x)\xrightarrow[x\to a^-]{}f(a)$ et $f(x)\xrightarrow[x\to a^+]{}f(a)$.

***Sens $\impliedby$*** :
$f(x)\xrightarrow[x\to a^-]{}f(a)$ donc il existe $\eta>0$ tel que $\forall x\in I\cap]-\infty,a[,|x-a|\leq \eta\implies |f(x)-f(a)|\leq\varepsilon$
Et $f(x)\xrightarrow[x\to a^+]{}f(a)$ donc il existe $\eta'>0$ tel que $\forall x \in I\cap]a,+\infty[,|x-a|\leq \eta\implies |f(x)-f(a)|\leq \varepsilon$.
Soit $x \in I$, on suppose $|x-a|\leq\min(\eta,\eta')$.
* Si $x<a$ : $|x-a|\leq \eta$ donc $|f(x)-f(a)|\leq\varepsilon$
* Si $x=a$ : $|f(x)-f(a)|=0\leq\varepsilon$
* Si $x> a$ : $|x-a|\leq \eta'$ donc $|f(x)-f(a)|\leq\varepsilon$
Donc dans tous les cas $|f(x)-f(a)|\leq \varepsilon$.
Ainsi $f(x)\xrightarrow[x\to a]{}f(a)$.

#### Remarques


