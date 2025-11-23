---
anki_linked: 0
raisonnements:
outils:
  - integration
kh_n:
  - "6"
  - "7"
display_title: Changement de variable (intégrales)
---
# Changement de variable

> [!objectif]
> Soit $\phi$ de classe $\mathcal{C}^1$ sur $[a,b]$ et à valeurs dans $I$ et $f$ continue sur $I$.
>$$
> \int_{a}^b f(\phi(t))\phi'(t)\mathrm{d}t=\int_{\phi(a)}^{\phi(b)}f(x)\mathrm{d}x
> $$
### Démonstration

Soit $\phi$ de classe $\mathcal{C}^1$ sur $[a,b]$ et à valeurs dans $I$ et $f$ continue sur $I$.
Notons $F$ une primitive de $f$ sur $I$.
On a : $(F\circ\phi)'=(F'\circ\phi)\times \phi'=(f\circ \phi)\times \phi'$
Donc :
$$
\begin{align}
\int_{a}^b f(\phi(t))\phi'(t)\mathrm{d}t&=\left[ F(\phi(t)) \right]_{a}^b \\
&=F(\phi(b))-F(\phi(a)) \\
\int_{a}^b f(\phi(t))\phi'(t)\mathrm{d}t&=\int_{\phi(a)}^{\phi(b)}f(t)\mathrm{d}t
\end{align}
$$
#### Remarques


