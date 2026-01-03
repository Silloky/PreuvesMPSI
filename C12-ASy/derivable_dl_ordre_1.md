---
anki_linked: 0
raisonnements:
outils:
  - dl
  - dérivation
kh_n:
  - "11"
display_title: Dérivable <=> DL d'ordre 1
---
# Dérivable $\iff$ DL d'ordre $1$

> [!objectif]
> Soit $a \in \mathbb{R}$ et $f:\mathbb{R}\to \mathbb{R}$
> Alors "$f$ dérivable en $a$" équivaut à "$f$ admet un $DL_{1}(a)$"
### Démonstration

***Sens $\implies$*** :
On suppose $f$ dérivable en $a$.
Donc d'après la "[[caract_epsilon_derivabilite|caractérisation epsilonesque de la dérivabilité]]", il existe $m\in \mathbb{R}$ et $\varepsilon:\mathbb{R}\to \mathbb{R}$ telle que $\varepsilon(x)\xrightarrow[x\to a]{} 0$ et :
$$
\forall x \in \mathbb{R}, f(x)=f(a)+m(x-a)+\varepsilon(x)(x-a)
$$
Puisque $\varepsilon(x)\xrightarrow[x\to a]{}0$, on peut directement écrire :
$f(x)\underset{ a }{ = }\left( f(a)+m(x-a) \right)+o(x-a)$
Ainsi $f$ admet un $DL_{1}(a)$ de partie régulière $P(t)=f(a)+mt$, qui est bien une fonction polynomiale du premier ordre.

***Sens $\impliedby$*** :
On suppose $f$ admet un $DL_{1}(a)$.
Donc par définition il existe un polynôme $P$ de degré $\deg(P)\leq 1$ tel que :
$$
f(x)\underset{ a }{ = }P(x-a)+o(x-a)
$$
$\deg(P)\leq 1$ donc il existe $(\alpha,\beta)\in \mathbb{R}^{2}$ tel que $\forall t \in \mathbb{R}, P(t)=\alpha+\beta h$
En remplaçant :
$$
f(x)\underset{ a }{ = }\alpha+\beta(x-a)+o(x-a)
$$
D'où en faisant tendre $x\to a$, par unicité de la limite $\alpha=f(a)$.

De plus, on pose $\varepsilon(x)\underset{ a }{ = }\frac{o(x-a)}{x-a}\xrightarrow[x\to a]{}0$.
Et on a :
$$
\forall x \in \mathbb{R}, f(x)=f(a)+\beta(x-a)+\varepsilon(x)(x-a)
$$
D'où, d'après la même "caractérisation", $f$ est dérivable en $a$ et sa dérivée vaut $\beta$.


#### Remarques


