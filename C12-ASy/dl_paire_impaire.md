---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "11"
display_title: Parité et DL
---
# Parité et développement limité

> [!objectif]
> Soit $f$ définie au voisinage de $0$.
> On suppose que $f$ admet un $DL_{1}(0)$ :
>$$
> f(x)\underset{ 0 }{ = }a_{0}+a_{1}x+a_{2}x^{2}+\dots+a_{n}x^n+o(x^n)
> $$
> Si :
> * $f$ est paire, les coefficients de rang impair sont nuls : $a_{1}=a_{3}=\dots=0$
> * $f$ est impaire, les coefficients de rang pair sont nuls : $a_{0}=a_{2}=\dots=0$

### Démonstration

On peut écrire :
$f(-x)\underset{ 0 }{ = }a_{0}-a_{1}x+a_{3}x^{2}+\dots+(-1)^n a_{n}x^n$.

***Si $f$ est paire*** :
On a alors, pour tout $x$, $f(-x)=f(x)$.
On note $k$ le plus grand entier impair inférieur à $n$.
Par unicité des DL :
$$
\begin{cases}
-a_{1}=a_{1} \\
-a_{3}=a_{3} \\
\dots \\
-a_{k}=a_{k}
\end{cases}\implies \begin{cases}
a_{1}=0 \\
a_{3}=0 \\
\dots \\
a_{k}=0
\end{cases}
$$
Ainsi tous les coefficients de rang impair sont nuls, et :
$$
f(x)\underset{ 0 }{ = }a_{0}+a_{2}x^2+a^4x^4+\dots+o(x^n)
$$
***Si $f$ est impaire*** :
On a, pour tout $x$, $f(-x)=-f(x)$.
Or : $-f(x)\underset{ 0 }{ = }-a_{0}-a_{1}x-a_{2}x^{2}-\dots -o(x^n)$
On note $k$ le plus grand entier pair inférieur à $n$.
Par unicité des DL :
$$
\begin{cases}
a_{0}=-a_{0} \\
a_{2}=-a_{2} \\
\dots \\
a_{k}=-a_{k}
\end{cases}\implies \begin{cases}
a_{0}=0 \\
a_{2}=0 \\
\dots \\
a_{k}=0
\end{cases}
$$
Donc tous les coefficients de rang pair sont nuls, et :
$$
f(x)\underset{ 0 }{ = }a_{1}x+a_{3}x^{3}+\dots+o(x^n)
$$

#### Remarques


