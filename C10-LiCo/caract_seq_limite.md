---
anki_linked: 0
raisonnements:
  - double_implication
  - contraposée
  - construction
outils:
  - limites
  - suites
kh_n:
  - "9"
display_title: Caractérisation séquentielle de la limite
---
# Caractérisation séquentielle de la limite

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$, $a\in \bar{I}$ et $L\in \bar{R}$ 
>$$
> f(x)\xrightarrow[x\to a]{}L\iff (\forall u\in I^\mathbb{N},u_{n}\to a\implies f(u_{n})\to L)
> $$
### Démonstration

Soit $a\in \mathbb{R}$ et $L\in \mathbb{R}$.

***Sens $\implies$*** :
On suppose $f(x)\xrightarrow[x\to a]{}L$.
Soit $u\in I^\mathbb{N}$. On suppose $u_{n}\to a$.
Soit $\varepsilon>0$.
$f(x)\xrightarrow[x\to a]{}L$ donc il existe $\eta>0$ tel que $\forall n\in \mathbb{N}, |u_{n}-a|\leq \eta\implies |f(u_{n})-L|\leq\varepsilon$.
Or $u_{n}\to a$ et $\eta>0$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N,|u_{n}-a|\leq\varepsilon$.
Soit $n\geq N$. $|u_{n}-a|\leq\varepsilon$, donc $|f(u_{n}-L)\leq\varepsilon|$.
Donc $f(u_{n})\to L$

***Sens $\impliedby$*** :
Par contraposée, montrons que $(f(x)\not\xrightarrow[x\to a]{}L)\implies(\exists u\in I^\mathbb{N},u_{n}\to a\land f(u_{n})\not\to L)$.
On suppose que $f(x)\not\xrightarrow[x\to a]{}L$. Donc il existe $\varepsilon>0$ tel que : $\forall \eta>0,\exists x \in I,|x-a|\leq \eta \land |f(x)-L|>\varepsilon$.

Pour tout $n\geq 1$, $\frac{1}{n}>0$, donc d'après la proposition précédente, il existe $x_{n}\in I$ tel que :
* $|x_{n}-a|\leq \frac{1}{n}$ donc $a-\frac{1}{n}\leq x_{n}\leq a+\frac{1}{n}$, donc par encadrement $x_{n}\to a$
* $|f(x_{n})-L|>\varepsilon$ donc $f(x_{n})\not\to L$

On a donc bien construit une suite $(x_{n})$ telle que $x_{n}\to a$ et $f(x_{n})\not\to L$.

D'où l'implication.

#### Remarques


