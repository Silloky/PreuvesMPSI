---
anki_linked: 1
raisonnements:
outils:
  - limites
  - dérivation
  - bijection
kh_n:
  - "4"
display_title: Théorème de la dérivabilité de la bijection réciproque
---
# Théorème de la dérivabilité de la bijection réciproque

> [!objectif]
> Soit  $f:I\to J$  une bijection.
> Si $f$ est dérivable sur $I$ et si $f'$ ne s'annule pas sur $I$, alors $f^{-1}$ est dérivable sur $J$ et :
> $$
> (f^{-1})'=\frac{1}{f'\circ f^{-1}}
> $$
### Démonstration

Soit  $f:I\to J$  une bijection (monotone). On suppose $f$ dérivable sur $I$ et que $f'$ ne s'annule pas sur $I$
Soit $x_{0} \in I$ ; on pose $y_{0}=f(x_{0})$.

Soit $y \in J$ tel que $y\neq y_{0}$. On pose $x=f^{-1}(y)$. Alors on a :$$
\frac{f^{-1}(y)-f^{-1}(y_{0})}{y-y_{0}}=\frac{x-x_{0}}{f(x)-f(x_{0})}=\frac{1}{\frac{f(x)-f(x_{0})}{x-x_{0}}}
$$Or quand $y\to y_{0}$, comme $f^{-1}$ est continue (d'après le théorème de la bijection monotone), $x\to x_{0}$.
Donc : $\frac{f(x)-f(x_{0})}{x-x_{0}}\to f'(x_{0})$ lorsque $y\to y_{0}$
Enfin : $$\lim_{ y \to y_{0} } \frac{f^{-1}(y)-f^{-1}(y_{0})}{y-y_{0}}=\frac{1}{f'(x_{0})}$$
Or $f'$ ne s'annule pas sur $I$ (par hypothèse), donc $\frac{1}{f'(x_{0})}$ est bien définie, donc cette limite est définie.
Donc $f^{-1}$ est dérivable en $y_{0}$ et :
$$
(f^{-1})'(y_{0})=\frac{1}{f'(x_{0})}=\frac{1}{f'(f^{-1}(y_{0}))}=\frac{1}{(f'\circ f^{-1})(y_{0})}
$$
Pour conclure, puisque $y_{0}\in J$ dépend de $x_{0}$ qui est quelconque, on peut dire que $f^{-1}$ est dérivable sur $J$ et que : $$(f^{-1})'=\frac{1}{f'\circ f^{-1}}$$

#### Remarques


