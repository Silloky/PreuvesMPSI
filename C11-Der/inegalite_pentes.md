---
anki_linked: 0
raisonnements:
outils:
  - dérivation
kh_n:
  - "11"
display_title: Inégalité des pentes
---
# Inégalité des pentes

> [!objectif]
> Soit $I$ un intervalle et $f:I\to \mathbb{R}$.
> 
> "$f$ convexe sur $I$" $\iff$ :
>$$
> \forall(a,b,c)\in I^3, a\leq b\leq c\implies \frac{f(b)-f(a)}{b-a}\leq \frac{f(c)-f(a)}{c-a}\leq \frac{f(c)-f(b)}{c-b}
> $$
### Démonstration

***Sens $\implies$***:

On suppose $f$ convexe sur $I$.
Soit $(a,b,c)\in I^{3}$. On suppose $a\leq b \leq c$.

On a $b\in[a,c]$ donc il existe $\lambda \in[0,1]$ tel que $b=\lambda a+(1-\lambda)c$.
Or $f$ est convexe sur $I$, et $b\in[a,c]\subset I$, donc $f(b)=f(\lambda a+(1-\lambda)c)\leq\lambda f(a)+(1-\lambda)f(c)$.

Ainsi $f(b)-f(a)\leq(\lambda f(a)+(1-\lambda)f(c))-f(a)=(1-\lambda)(f(c)-f(a))$
Et $b-a=(\lambda a+(1-\lambda)c)-a=(1-\lambda)(c-a)$.
Donc $\frac{f(b)-f(a)}{b-a}\leq \frac{f(c)-f(a)}{c-a}$.

De même, $f(b)-f(c)\leq\lambda f(a)+(1-\lambda)f(c)-f(c)=\lambda(f(a)-f(c))$, et $b-c=\lambda a+(1-\lambda)c-c=\lambda(a-c)$.
Donc $\frac{f(c)-f(a)}{c-a}\leq \frac{f(c)-f(b)}{c-b}$.

D'où :
$$
\frac{f(b)-f(a)}{b-a}\leq \frac{f(c)-f(a)}{c-a}\leq \frac{f(c)-f(b)}{c-b}
$$

#### Remarques


