---
anki_linked: 1
raisonnements:
outils:
  - module
kh_n:
display_title: Propriétés du module
---
# Propriétés du module

> [!objectif]
> Soit $(z,z')\in \mathbb{C}$
> 1. $|zz'|=|z|\times |z'|$
> 2. $|\mathrm{Re}(z)|\leq |z|$
### Démonstration

##### 1. Module d'un produit

Soit $(z,z')\in \mathbb{C}$ deux complexes.

***Sans passer à une autre forme*** :
$$
\begin{align}
|zz|^{2}&=zz'\times \overline{zz'} \\
&=zz'\times \bar{z}\bar{z'} \\
&=zz'\times z'\bar{z'} \\
|zz|^{2}&=|z|^{2}\times |z'|^{2}
\end{align}
$$
Et puisque $\forall z\in \mathbb{C},|z|\in \mathbb{R}_{+}$ : $|zz'|=|z|\times |z'|$

***En passant par la forme algébrique*** :
Alors il existe $(a,b,a',b')\in \mathbb{R}^4$ tel que $z=a+ib$ et $z'=a'+ib'$.
Donc 
$$
\begin{align}
|zz'|^{2}&=|(a+ib)(a'+ib')|^{2} \\
&=|aa'-bb'+i(a'b+ab')|^{2} \\
&=(aa'-bb')^{2}+(a'b+ab')^{2} \\
&=(aa')^{2}-2aa'bb'+(bb')^{2}+(a'b)^{2}+2a'bab'+(ab')^{2} \\
|zz'|^{2}&=(aa')^{2}+(ab')^{2}+(a'b)^{2}+(bb')^{2}
\end{align}
$$
Or : $(|z|\times |z'|)^{2}=|z|^{2}\times |z'|^{2}=(a^{2}+b^{2})(a'^{2}+b'^{2})=(aa')^{2}+(ab')^{2}+(a'b)^{2}+(bb')^{2}$
Donc $|zz'|^{2}=(|z|\times |z'|)^{2}$, donc puisque $\forall z\in \mathbb{C},|z|\in \mathbb{R}_{+}$ :
$$
|zz'|=|z|\times |z'|
$$
##### 2. $|\mathrm{Re}(z)|\leq |z|$

Soit $z\in \mathbb{C}$. Donc il existe $(a,b)\in \mathbb{R}^{2}$ tel que $z=a+ib$.
Donc $|\mathrm{Re}(z)|=|a|$
Or $|z|=\sqrt{ a^{2}+b^{2} }\geq \sqrt{ a^{2} }=|a|$.
Donc $|\mathrm{Re}(z)|\leq |z|$

#### Remarques


