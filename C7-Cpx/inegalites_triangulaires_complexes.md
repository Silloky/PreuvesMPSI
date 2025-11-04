---
anki_linked: 0
raisonnements:
  - double_implication
  - disjonction_de_cas
outils:
  - module
kh_n:
display_title: Inégalités triangulaires complexes
---
# Inégalités triangulaires complexes

> [!objectif]
> Soit $(z,z')\in \mathbb{C}^{2}$
>1. Classique : $|z+z'|\leq |z|+|z'|$
>2. Inversée : $||z|-|z'||\leq |z-z'|$
>3. Cas d'égalité : $|z+z'|=|z|+|z'|\Longleftrightarrow (\exists\lambda \in \mathbb{R}_{+},z=kz')\lor z'=0$
### Démonstration

##### 1. Classique
Soit $(z,z')\in \mathbb{C}^{2}$.
D'une part :
$$
\begin{align}
(|z+z'|)^{2}&=(z+z')\overline{z+z'} \\
&=(z+z')(\bar{z}+\bar{z'}) \\
&=zz+z \bar{z'}+z' \bar{z}+z' \bar{z'} \\
&=|z|^{2}+z \bar{z'}+\overline{z \bar{z'}}+|z'|^{2} \\
(|z+z'|)^{2}&=|z|^{2}+2\mathrm{Re}(z \bar{z'})+|z'|^{2}
\end{align}
$$
D'autre part :
$$
\begin{align}
(|z|+|z'|)^{2}&=|z|^{2}+2|z||z'|+|z'|^{2} \\
&=|z|^{2}+2|z||z'|+|z'|^{2} \\
(|z|+|z'|)^{2}&=|z|^{2}+2|zz'|+|z'|^{2}
\end{align}
$$
Or $\mathrm{Re}(zz')\leq |zz'|$
Donc $(|z|+|z'|)^{2}\leq(|z|+|z'|)^{2}$.
Or par définition du module, $|z+z'|\geq 0$ et $|z|+|z'|\geq 0$
Donc $|z+z'|\leq |z|+|z'|$
##### 2. Inversée

Soit $(z,z')\in \mathbb{C}^{2}$
$|z|=|z-z'+z'|\leq |z-z'|+|z'|$ donc $|z|-|z'|\leq |z-z'|$.
Et de même, $|z'|-|z|\leq |z'-z|=|z-z'|$.
Ainsi, $||z|-|z'||\leq |z-z'|$
##### 3. Cas d'égalité
Soit $(z,z')\in \mathbb{C}^{2}$.

***Sens $\Longrightarrow$*** :
On suppose $(\exists\lambda \in \mathbb{R}_{+},z=kz')\lor z'=0$.

1. On suppose qu'il existe $\lambda \in \mathbb{R}_{+}$ tel que $z=kz'$. Alors :
$$
\begin{align}
|z+z'|&=|\lambda z'+z'| \\
&=|(\lambda+1)z'| &  \\
&=\lambda |z'|+|z'| \\
&=|\lambda z'|+|z'| \\
|z+z'|&=|z|+|z'|
\end{align}
$$
2. On suppose que $z'=0$. Alors $|z+z'|=|z|=|z|+|0|=|z|+|z'|$

***Sens $\Longleftarrow$*** :
On suppose que $|z+z'|=|z|+|z'|$. Alors :
$$
\begin{align}
(|z|+|z'|)^{2}&=(z+z')\overline{z+z'} \\
&=|z|^{2}+2\mathrm{Re}(zz')+|z'|^{2} \\
(|z|+|z'|)^{2}&=|z|^{2}+2|z \bar{z'}|+|z'|^{2}
\end{align}
$$
Donc $\mathrm{Re}(zz')=|zz'|$, donc $z \bar{z'}\in \mathbb{R}_{+}$.
On pose $\alpha=z \bar{z'}$
On suppose $z'\neq 0$, donc $|z'|^{2}\neq 0$
On pose alors $\lambda=\frac{\alpha}{|z'|^{2}}\geq 0$.
$\alpha=z \bar{z'}$, donc $zz' \bar{z'}=\alpha z'$, donc $z|z'|^{2}=\alpha z'$, donc $z=\frac{\alpha}{|z'|^{2}}z'=\lambda z'$
Donc il existe bien $\lambda \in \mathbb{R}_{+}$ tel que $z=\lambda z'$

#### Remarques


