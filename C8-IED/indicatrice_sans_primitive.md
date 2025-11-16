---
anki_linked: 0
raisonnements:
  - absurde
outils:
  - primitives
  - limites
kh_n:
  - "6"
display_title: Id_R+* n'admet pas de primitives sur R
---
# $\mathrm{Id}_{\mathbb{R}_{+}^*}$ n'admet pas de primitive sur $\mathbb{R}$

> [!objectif]
> On considère :
> $$
> \begin{align}
\mathrm{Id_{\mathbb{R}^*_{+}}}= f:\begin{cases}
\mathbb{R}\to \mathbb{R} \\
x\mapsto \begin{cases}
1 & \text{si } x>0 \\
0 & \text{si }x \neq 0
\end{cases}
\end{cases}
\end{align}
$$
### Démonstration

Par l'absurde, on suppose que $f$ admet une primitive sur $\mathbb{R}$ que l'on note $F$.

***Primitive sur $\mathbb{R}_{-}$*** :
$F$ y est dérivable, et, pour tout réel $x$, $F'(x)=f(x)=0$. Puisque $\mathbb{R}_{+}^*$ est un intervalle, $F$ est constante sur $\mathbb{R}_{-}$
Donc il existe $c\in \mathbb{R}$ tel que $\forall x \in\mathbb{R}_{-},F(x)=c$.

***Primitive sur $\mathbb{R}_{+}^*$*** :
$x\mapsto F(x)-x$ est dérivable sur $\mathbb{R}_{+}^*$ et sa dérivée y est nulle, donc elle est constante sur $\mathbb{R}_{+}^*$.
Donc il existe $c'\in \mathbb{R}$ tel que $\forall x \in \mathbb{R}_{+}^*,F(x)=x+c'$

***Apparition de l'absurde*** :
On a $\forall x >0,F(x)=x+c'$, donc $\lim_{ x \to 0^+ }F(x)=c'$.
Or $f$ est continue, donc $\lim_{ x \to 0^+ }F(x)=F(0)$, et $F(0)=c$, donc $c=c'$.
Alors :
* $\forall x>0, \frac{F(x)-F(0)}{x-0}=\frac{x+c'-c}{x}=1\xrightarrow[x\to 0^+]{}1$, donc $F'(0^+)=1$
* $\forall x <0, \frac{F(x)-F(0)}{x-0}=\frac{c-c}{x}=0\xrightarrow[x\to 0^-]{0}=0$, donc $F'(0^-)=0$
* $F(0)=c$
Donc $F$ n'est pas continue en $0$, donc elle n'est pas dérivable en $0$, ce qui est absurde.

Donc $f$ n'admet pas de primitives sur $I$.

#### Remarques


