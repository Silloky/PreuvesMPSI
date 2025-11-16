---
anki_linked: 0
raisonnements:
outils:
  - derivation
  - limites
kh_n:
  - "6"
display_title: Fonction dérivable dont la dérivée n'est pas continue
---
# Fonction dérivable dont la dérivée n'est pas continue

> [!objectif]
> Soit : 
> $$
> f:
> \begin{cases} \\
\mathbb{R}\to \mathbb{R} \\
x\mapsto \begin{cases}
> x^{2}\sin\left( \frac{1}{x} \right)&\text{si }x\neq 0 \\
> 0 & \text{si }x=0
> \end{cases}
\end{cases}
> $$
> Montrer que $f$ est dérivable et que sa dérivée n'est pas continue.

### Démonstration

***Dérivabilité sur $\mathbb{R}_{+}^*$ et $\mathbb{R}_{-}^*$***
$x\mapsto \frac{1}{x}$ est dérivable sur $\mathbb{R}_{+}^*$ et à valeurs dans $\mathbb{R}$. De plus, $\sin$ est dérivable sur $\mathbb{R}$ donc par composée $x\mapsto \sin\left( \frac{1}{x} \right)$ est dérivable sur $\mathbb{R}_{+}^*$.
Enfin, par produit, $f$ est dérivable sur $\mathbb{R}_{+}^*$, et de même, $f$ est dérivable sur $\mathbb{R}_{-}^*$.

***Epointage de $0$*** :
Pour tout $x\neq 0$ : $\frac{f(x)-f(0)}{x-0}=x\sin\left( \frac{1}{x} \right)$.
$\sin\left( \frac{1}{x} \right)$ est bornée, donc $\frac{f(x)-f(0)}{x-0}\xrightarrow[x\to 0]{}=0$.
Donc $f$ est dérivable en $0$ et $f'(0)=0$

***Expression de $f'$*** :
Donc $f$ est dérivable sur $\mathbb{R}$ et :
$$
f':\begin{cases}
\mathbb{R}\to \mathbb{R} \\
x\mapsto \begin{cases}
2x\sin\left( \frac{1}{x} \right)-\cos\left( \frac{1}{x} \right) & \text{si } x\neq 0 \\
0 & \text{si } x=0
\end{cases}
\end{cases}
$$
***Non-continuité de $f'$*** :
Or $x\mapsto\cos\left( \frac{1}{x} \right)$ n'a pas de limite à droite en $0$, donc $f'$ n'est pas continue.


#### Remarques


