---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - derivation
kh_n:
  - "11"
display_title: Convexe <=> Dérivée croissante
---
# Convexe $\iff$ Dérivée croissante

> [!objectif]
> Soit $f:I\to \mathbb{R}$. On suppose $f$ dérivable sur $I$.
> Alors "$f$ convexe sur $I$" $\iff$ "$f'$ croissante sur $I$"
### Démonstration

***Sens $\implies$*** :

On suppose $f$ convexe sur $I$.
Soit $(a,b)\in I^{2}$. On suppose $a\leq b$, et plus précisément, on suppose $a<b$ car le cas $a=b$ est évident.
D'après l'inégalité des pentes :
$$
\forall x \in ]a,b[, \frac{f(x)-f(a)}{x-a}\leq \frac{f(b)-f(a)}{b-a}\leq \frac{f(b)-f(x)}{b-x}
$$
$f$ est dérivable sur $I$, donc par passage à la limite :
$f'(a)=\lim_{ x \to a^+ } \frac{f(x)-f(a)}{x-a}\leq \frac{f(b)-f(a)}{b-a}$.
De même, $f'(b)=\lim_{ x \to b^- } \frac{f(x)-f(b)}{x-b}\geq \frac{f(b)-f(x)}{b-x}$.
Donc $f'(a)\leq f'(b)$.
D'où $f'$ est croissante.

***Sens $\impliedby$*** :
On suppose $f'$ croissante sur $I$.
Soit $(a,b)\in I^{2}$. On suppose $a<b$ (le cas $a>b$ est similaire, et le cas $a=b$ est évident).

On pose $g:\begin{cases}[0,1]\to \mathbb{R} \\ \lambda\mapsto \lambda f(a)+(1-\lambda)f(b)-f(\lambda a+(1-\lambda)b) \end{cases}$
Par composition et sommes de fonctions dérivables, $g$ est dérivable sur $[0,1]$ et :
$$
\forall \lambda \in[0,1], g'(\lambda)=f(a)-f(b)-(a-b)f'(\lambda a+(1-\lambda)b)
$$
Or $f$ est dérivable sur $[a,b]$, donc continue sur $[a,b]$ et dérivable sur $]a,b[$ donc il existe $c \in]a,b[$ tel que $f'(c)=\frac{f(b)-f(a)}{b-a}$
On a $c\in[a,b]$, donc il existe $\lambda_{0} \in[0,1]$ tel que $c=\lambda_{0} a+(1-\lambda_{0})b$.
Donc $g'(\lambda_{0})=f(a)-f(b)-(a-b)f'(c)=f(a)-f(b)-(a-b)\times \frac{f(a)-f(b)}{a-b}=0$, et $g'$ s'annule en $c$.

De plus, pour tout $\lambda \in[\lambda_{0},1]$, $\lambda_{0}a+(1-\lambda)b\leq \lambda a+(1-\lambda)b$, or $f'$ est croissante sur $[a,b]$ donc $f'(\lambda_{0}a+(1-\lambda_{0})b)\leq f'(\lambda a+(1-\lambda)b)$, donc $g'(\lambda)\leq 0$.
De même, pour tout $\lambda \in[0,\lambda_{0}]$, $g'$ est positif.

Enfin, $g(0)=g(1)=0$, donc on a le tableau de variation de $g$ :

$$
\begin{array}{c|ccc}
\lambda & 0 & \lambda_0 & 1 \\ \hline
g'(\lambda) & + &  0 & -\\ \hline
g(\lambda) & 0 & \nearrow\ g(\lambda_0)\ \searrow & 0
\end{array}
$$

Ainsi $g$ est positive sur $[0,1]$, d'où :
$$
\forall \lambda \in[0,1], f(\lambda a+(1-\lambda)b)\leq\lambda f(a)+(1-\lambda)f(b)
$$
Et donc, par définition, $f$ est convexe.

#### Remarques


