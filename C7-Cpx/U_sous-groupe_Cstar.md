---
anki_linked: 0
raisonnements:
outils:
  - groupe
kh_n:
  - "5"
display_title: U sous-groupe de (C*,+)
---
# $\mathbb{U}$ sous-groupe de $(\mathbb{C}^*,\times)$

> [!objectif]
> Le cercle unitaire $\mathbb{U}=\{ z\in \mathbb{C}\mid |z|=1 \}$ est un sous-groupe du groupe $(\mathbb{C}^*,\times)$
### Démonstration

***Inclusion des ensembles*** :
Pour tout $z\in \mathbb{U}$, $|z|=1\neq 0$ donc $z\neq 0$.
Donc $z\in \mathbb{C}^*$, donc $\mathbb{U}\subset \mathbb{C}^*$

***Element neutre*** :
$|1_{\mathbb{C}^*}|=|1|=1$ donc $1_{\mathbb{C}^*}\in \mathbb{U}$

***Stabilité*** :
Soit $(z,z')\in \mathbb{U}^{2}$.
$|zz'|=|z||z'|=1\times 1=1$ donc $zz'\in \mathbb{U}$

***Stabilité par passage à l'inverse***
Soit $z\in \mathbb{U}\subset \mathbb{C}^*$, donc $z$ est inversible et on note $z^{-1}$ son inverse. 
$\left| \frac{1}{z} \right|=\frac{|1|}{|z|}=\frac{1}{1}=1$, donc $\frac{1}{z}=z^{-1}\in \mathbb{U}$

Donc $\mathbb{U}$ est un sous-groupe de $(\mathbb{C}^*,\times)$.

#### Remarques

On pourrait rassembler la stabilité et la stabilité par passage à l'inverse, ce serait tout à fait faisable et correct, mais moins joli pour une preuve aussi courte.
