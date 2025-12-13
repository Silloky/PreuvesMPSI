---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - dérivation
kh_n:
  - "10"
display_title: Caractérisation epsilonesque de la densité
---
# Caractérisation epsilonesque de la densité

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ et $a\in I$.
> "$f$ est dérivable en $a$" équivaut à "il existe un réel $m$ et une fonction $\varepsilon$ définie sur $I$ telle que $\varepsilon(x)\xrightarrow[x\to a]{}0$ et $\forall x \in I,f(x)=f(a)+m(x-a)+\varepsilon(x)(x-a)$"
### Démonstration

***Sens $\impliedby$*** :
On suppose qu'il existe un réel $m$ et une fonction $\varepsilon:I\to \mathbb{R}$ qui conviennent.
Alors, pour tout $x \in I\setminus{a}$, on a : $\frac{f(x)-f(a)}{x-a}=m+\varepsilon(x)\xrightarrow[x\to a^{\neq}]{}m$
Donc $f$ est dérivable en $a$ et sa dérivée vaut $m$.

***Sens $\implies$*** :
On suppose que $f$ est dérivable en $a$. 
On pose $m=f'(a)$ et :
$$
\forall x \in I,\varepsilon(x)=\begin{cases}
\frac{f(x)-f(a)}{x-a}-m & \text{si }x\neq a \\
0 & \text{si }x=a
\end{cases}
$$
Soit $x \in I$.
Si $x\neq a$ alors $\frac{f(x)-f(a)}{x-a}-m=\varepsilon(x)$, donc $f(x)=f(a)+m(x-a)+\varepsilon(x)(x-a)$.
Si $x=a$ alors $f(x)=f(a)=f(a)+m\underbrace{ (x-a) }_{ =0 }+\underbrace{ \varepsilon(x)(x-a) }_{ =0 }$.
Donc dans tous les cas, $f(x)=f(a)+m(x-a)+\varepsilon(x)(x-a)$ et :
$$
\forall x \in I,\varepsilon(x)=\frac{f(x)-f(a)}{x-a}-m
$$
Or $\frac{f(x)-f(a)}{x-a}\xrightarrow[x\to a^\neq]{}f'(a)=m$.
Donc $\varepsilon(x)\xrightarrow[x\to_{0}]{}0$.

#### Remarques


