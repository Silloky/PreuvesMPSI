---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "11"
display_title: Unicité des DL
---
# Unicité des développements limités

> [!objectif]
> Soit $a \in \mathbb{R}$, $f$ définie sur un voisinage de $a$ (sauf éventuellement en $a$) et $n \in \mathbb{N}$.
> Si $f$ admet un $DL_{n}(a)$ alors il est unique.
### Démonstration

On suppose que $f$ admet deux $DL_{n}(a)$.
Alors il existe $P$ et $Q$ deux fonctions polynomiales de degré inférieur ou égal à $n$ tels que :
* $f(x)\underset{ a }{ = }P(x-a)+o((x-a)^n)$
* $f(x)\underset{ a }{ = }Q(x-a)+o((x-a)^n)$
Donc $P(x-a)-Q(x-a)\underset{ a }{ = }o((x-a)^n)$, d'où :
$$
\frac{P(x-a)-Q(x-a)}{(x-a)^n}\xrightarrow[x\to a]{}0
$$
$P-Q$ est un polynôme, on note $a_{0},\dots,a_{n}$ ses coefficients.
Par l'absurde, on suppose que $P\neq Q$, donc $P-Q\neq 0$.
Ainsi $P-Q$ n'est pas un polynôme identiquement nul, donc il existe $k \in [\![0,n]\!]$ l'indice du premier terme non nul.
Donc :
$$
\forall x \in \mathbb{R}, P(x-a)-Q(x-a)=a_{k}(x-a)^k+\dots+a_{n}(x-a)^n
$$
Avec $a_{k}\neq 0$, donc $P(x-a)-Q(x-a) \underset{ a }{ \sim }a_{k}(x-a)^k$, d'où :
$$
\frac{P(x-a)-Q(x-a)}{(x-a)^n} \underset{ a }{ \sim } \frac{a_{k}}{(x-a)^{n-k}}\not\xrightarrow[x\to a]{}0
$$
Ce qui est absurde, donc $P=Q$.
D'où l'unicité du $DL_{n}(a)$ de $f$.

#### Remarques


