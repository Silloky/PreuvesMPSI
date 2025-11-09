---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - polynome
kh_n:
  - "5"
display_title: Équation du second degré complexe à coefficients complexes
---
# Équation du second degré complexe à coefficients complexes

> [!objectif]
> Soit $(a,b,c)\in \mathbb{R}^{3}$ et $a\neq 0$. On pose l'équation d'inconnue $z$ complexe : $(E):az^{2}+bz+c$.
> On pose $\Delta=b^{2}-4ac$;
> * Si $\Delta=0$ : il y a une seule racine $z_{0}=-\frac{b}{2a}$
> * Si $\Delta\neq 0$ : il y a deux racines distinctes, $z_{1}=\frac{-b-\delta}{2a}$ et $z_{2}=\frac{-b+\delta}{2a}$, où $\delta$ est une racine carrée de $\Delta$
### Démonstration

Soit $z\in \mathbb{C}$. On pose $\Delta=b^{2}-4ac$.
$$
\begin{align}
az^{2}+bz+c=0 &\Longleftrightarrow z^{2}+\frac{b}{a}z+\frac{c}{a}=0 \\
&\Longleftrightarrow z^{2}+2\times \frac{b}{2a}+\frac{b^{2}}{4a^{2}}-\frac{b^{2}}{4a^{2}}+\frac{c}{a}=0 \\
&\Longleftrightarrow \left( z+\frac{b}{2a} \right)^{2}-\frac{b^{2}}{4a^{2}}+\frac{c}{a}=0 \\
az^{2}+bz+c=0 &\Longleftrightarrow\left( z+\frac{b}{2a} \right) ^{2}=\frac{b^{2}-4ac}{4a^{2}}=\frac{\Delta}{4a^{2}}
\end{align}
$$
***Si $\Delta=0$*** :
$$
\begin{align}
az^{2}+bz+c=0 &\Longleftrightarrow\left( z+\frac{b}{2a} \right) ^{2}=\frac{\Delta}{4a^{2}} \\
&\Longleftrightarrow\left( z+\frac{b}{2a} \right)^{2}=0 \\
az^{2}+bz+c=0&\Longleftrightarrow z=-\frac{b}{2a}
\end{align}
$$
***Si $\Delta\neq 0$*** :
Alors il existe $\delta \in \mathbb{C}$ tel que $\delta^{2}=\Delta$ ($\delta$ est une racine carrée de $\Delta$).
Donc :
$$
\begin{align}
az^{2}+bz+c=0 &\Longleftrightarrow\left( z+\frac{b}{2a} \right) ^{2}=\frac{\Delta}{4a^{2}} \\
&\Longleftrightarrow \left( z+\frac{b}{2a} \right) ^{2}=\left( \frac{\delta}{2a} \right)^{2} \\
&\Longleftrightarrow z+\frac{b}{2a}=\frac{\delta}{2a} \quad\text{ou}\quad z+\frac{b}{2a}=-\frac{\delta}{2a} \\
az^{2}+bz+c=0&\Longleftrightarrow z=\frac{-b-\delta}{2a} \quad\text{ou}\quad z=\frac{-b-\delta}{2a}
\end{align}
$$

#### Remarques


