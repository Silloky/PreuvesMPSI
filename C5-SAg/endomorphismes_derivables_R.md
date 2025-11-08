---
anki_linked: 0
raisonnements:
  - analyse_synthese
outils:
  - morphisme
kh_n:
  - "4"
display_title: Endomorphismes dérivables de R
---
# Endomorphismes dérivables de $\mathbb{R}$

> [!objectif]
> Les endomorphismes dérivables de $\mathbb{R}$ sont les fonctions linéaires à coefficient réel.
### Démonstration

***Analyse*** :

Soit $f$ un endomorphisme de $\mathbb{R}$ dérivable sur $\mathbb{R}$.

Soit $y\in \mathbb{R}$.
On pose : 
$$
\begin{cases}
f_{1}:x\mapsto f(x+y) \\
f_{2}:x\mapsto f(x)+f(y) \\
h:x\mapsto x+y
\end{cases}
$$
$h$ est dérivable sur $\mathbb{R}$, à valeurs dans $\mathbb{R}$ et $f$ est dérivable sur $\mathbb{R}$, donc $f_{1}=f\circ h$ est dérivable sur $\mathbb{R}$ et :
$$
\begin{align}
\forall x\in \mathbb{R}, f_{1}'(x)&=(f\circ h)'(x) \\
&=f'(h(x))\times h'(x) \\
f_{1}'(x)&=f'(x+y)\times 1
\end{align}
$$
De même, $f_{2}$ est dérivable sur $\mathbb{R}$ et $\forall x \in \mathbb{R},f_{2}'(x)=f'(x)+0$ (puisque $y$ est une constante).

Par hypothèse (d'endomorphisme), $f_{1}=f_{2}$, donc $f_{1}'=f_{2}'$. En particulier, $f'(y)=f'(0)$.
On pose $a=f'(0)$, ainsi $\forall x \in \mathbb{R},f'(x)=a$ (car $f'(y)$ ne dépend pas de $y$).

On pose $g:x\mapsto f(x)-ax$.
$g$ est dérivable sur $\mathbb{R}$ et $\forall x \in \mathbb{R}, g'(x)=f'(x)-a=a-a=0$.

Donc $g$ est constante sur $\mathbb{R}$ donc il existe $b\in \mathbb{R}$ tel que : $\forall x \in \mathbb{R},g(x)=b$, donc que $f(x)=ax+b$.

Or $f(0)=f(0+0)=f(0)+f(0)$, donc $f(0)=0$, et puisque $f(0)=0a+b=b$, on en déduit que $b=0$.

Donc $\forall x \in \mathbb{R},f(x)=ax$

***Synthèse*** :

Soit $f\in \{x\mapsto ax\mid a \in \mathbb{R}\}$.
Donc il existe $a\in \mathbb{R}$ tel que $\forall x \in \mathbb{R},f(x)=ax$.

Or pour tout $x \in \mathbb{R}$, on a bien $ax \in \mathbb{R}$, donc $f:\mathbb{R}\to \mathbb{R}$.
De plus : soit $(x,y)\in \mathbb{R}^2$.
$f(x+y)=a(x+y)=ax+ay=f(x)+f(x)$
Donc $f$ est bien un endomorphisme de $\mathbb{R}$.

Enfin, $f$ est dérivable car il existe bien $a$ tel que pour tout $x \in \mathbb{R}$, $f'(x)=a$ existe.

Donc $f$ est un endomorphisme dérivable de $\mathbb{R}$.

***Bilan*** :

Les endomorphismes dérivables de $\mathbb{R}$ sont les fonctions linéaires à coefficient réel.

#### Remarques


