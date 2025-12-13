---
anki_linked: 0
raisonnements:
outils:
  - limites
kh_n:
  - "8"
display_title: Opérations sur les limites de fonctions
---
# Opérations sur les limites de fonctions

> [!objectif]
> Soit $f:I\to \mathbb{R}$, $g:I\to \mathbb{R}$, $a\in \bar{I}$. On suppose $a\in \mathbb{R}$.
> On suppose que $f(x)\xrightarrow[x\to a]{}l\in \mathbb{R}$ et $g(x)\xrightarrow[x\to a]{}l'\in \mathbb{R}$.
> 1. $f(x)+g(x)\xrightarrow[x\to a]{}l+l'$
> 2. $f(x)\times g(x)\xrightarrow[x\to a]{}l\times l'$
> 3. Si $f$ est bornée au voisinage de $a$ et $g(x)\xrightarrow[x\to a]{}0$, alors $f(x)\times g(x)\xrightarrow[x\to a]{}0$
### Démonstration

##### 1. $f+g$

Soit $\varepsilon>0$.
$f(x)\xrightarrow[x\to a]{}l$, donc il existe $\eta>0$ tel que $\forall x \in I,|x-a|\leq \eta\implies |f(x)-l|\leq \varepsilon$.
De même, $g(x)\xrightarrow[x\to a]{}l'$ donc il existe $\eta'>0$ tel que $\forall x \in I, |x-a|\leq\eta'\implies |f(x)-l'|\leq \varepsilon$.
Donc pour tout $x \in I$, $|x-a|\leq\min(\eta,\eta')\implies|f(x)+l+g(x)-l'|\leq \varepsilon$.
Donc il existe bien un $\eta''>0$ tel que $\forall x \in I, |x-a|\leq \eta''\implies |(f(x)+g(x)-(l+l'))|\leq \varepsilon$.
Ainsi $f(x)+g(x)\xrightarrow[x\to a]{}l+l'$
##### 2. $f\times g$

Pour tout $x \in I$:
$$\begin{align}
|f(x)g(x)-ll'|&=|f(x)(g(x)-l')+l'(f(x)-l)| \\
&\leq |f(x)||g(x)-l'|+|l'||f(x)-l|
\end{align}
$$
Or $f(x)\xrightarrow[x\to a]{}l$ et $g(x)\xrightarrow[x\to a]{}l'$, donc $|f(x)-l|\xrightarrow[x\to a]{}0$ et $|g(x)-l'|\xrightarrow[x\to a]{}0$.
Donc $|f(x)g(x)-ll'|\xrightarrow[x\to a]{}0$, donc $\forall \varepsilon>0, |f(x)g(x)-ll'-0|\leq\varepsilon$, donc $f(x)g(x)\xrightarrow[x\to a]{}ll'$.
##### 3. $f$ bornée et $g\to 0$

Soit $\varepsilon>0$.
$f$ est bornée au voisinage de $a$, donc il existe $\eta>0$ et $M>0$ tel que $\forall x \in I\cap[0-\eta,0+\eta], f(x)\leq M$.
$\frac{\varepsilon}{M}$ donc il existe $\eta'>0$ tel que $\forall x \in I, |x-a|\leq \eta'\implies |g(x)|\leq \frac{\varepsilon}{M}$.
Donc pour tout $x \in I$ : $|x-a|\leq \min(\eta,\eta'), |f(x)g(x)|\leq M\times \frac{\varepsilon}{M}=\varepsilon$.
Donc $f(x)g(x)\xrightarrow[x\to a]{}\varepsilon$.

#### Remarques

Pour la [[composition_limites|composition de limites]], voir le document à part.