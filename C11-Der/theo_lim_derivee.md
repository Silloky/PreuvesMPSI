---
anki_linked: 0
raisonnements:
outils:
  - derivation
  - limites
kh_n:
  - "11"
display_title: Théorème de la limite de dérivée
---
# Théorème de la limite de dérivée

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ et $a \in I$.
> Si :
> 1. $f$ est continue sur $I$
> 2. $f$ est dérivable sur $I\setminus \{ a \}$
> 3. $f'(x)\xrightarrow[x\to a]{}l \in\overline{\mathbb{R}}$
>
>Alors :
>$$
> \tau_{a}(x)=\frac{f(x)-f(a)}{x-a}\xrightarrow[x\to a]{}l
> $$
> En particulier :
> * Si $l\in \mathbb{R}$ alors $f$ est dérivable en $a$ et $f'(a)=l$
> * Si $l=\pm \infty$ alors $f$ n'est pas dérivable en $a$

### Démonstration

Soit $x \in I\setminus \{ a \}$. On suppose $x>a$ (le cas $x<a$ est similaire).

Alors $a$ et $x$ sont dans $I$ et $I$ est un intervalle donc $[a,x]\subset I$.
Or $f$ est continue sur $I$ et dérivable sur $I\setminus \{ a \}$, donc en particulier, $f$ est continue sur $[a,x]$ et dérivable sur $]a,x[$.
Donc d'après le [[theo_accroissements_finis|TAF]], il existe un réel $c(x)\in]a,x[$ tel que $\frac{f(x)-f(a)}{x-a}=f'(c(x))$.

Ainsi, pour tout $x \in I\setminus \{ a \}$, $0\leq|c(x)-a|\leq |x-a|$. Or $|x-a|\xrightarrow[x\to a^\neq]{}0$, donc par encadrement, $|c(x)-a|\xrightarrow[x\to a^\neq]{}0$, donc $c(x)\xrightarrow[x\to a^\neq]{}a^\neq$.
Et par hypothèse $f'(x)\xrightarrow[x\to a^\neq]{}l$, donc par composition, $f'(c(x))\xrightarrow[x\to a^\neq]{}l$.

D'où $\frac{f(x)-f(a)}{x-a}\xrightarrow[x\to a^\neq]{}l$

Cette expression correspond à celle de $\tau_{a}$, d'où les conséquences immédiates du théorème sur la dérivabilité de $f$ en $a$.
#### Remarques
