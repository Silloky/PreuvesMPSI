---
anki_linked: 0
raisonnements:
  - analyse_synthese
outils:
  - equadiff
kh_n:
  - "6"
  - "7"
display_title: Solutions de y'+ay=0
---
# Solutions de $y'+ay=0$

> [!objectif]
> Les solutions de l'EDL $(E):y'+ay=0$ sur $I$ sont $\{ \lambda e^{-A(x)} \mid\lambda\in \mathbb{R} \}$ où $A$ est une primitive de $a$ sur $I$.
### Démonstration

***Analyse*** :
Soit $y$ une solution de $(E)$.

On pose $z:x\mapsto y(x)e^{A(x)}$ or $A$ est dérivable sur $I$ et $\exp$ est dérivable sur $\mathbb{R}$ donc $e^{A(x)}$ est dérivable sur $I$. De plus $y$ est dérivable sur $I$, donc, enfin, $z$ est dérivable sur $I$ et :
$\forall x \in \mathbb{R},z'(x)=e^{A(x)}(y'(x)+ay(x))$.
Or $y$ est solution, donc $\forall x \in \mathbb{R},  y'(x)+ay(x)=0$, et donc $z$ est constante sur $I$.
Ainsi il existe $\lambda \in \mathbb{R}$ tel que $\forall x \in I,z(x)=\lambda$.
Enfin, $\forall x \in I, \lambda=y(x)e^{A(x)}$ donc $y(x)=\lambda e^{-A(x)}$.

***Synthèse*** :
Soit $\lambda \in \mathbb{R}$. On pose $y:x\mapsto\lambda e^{-A(x)}$.
$y$ est dérivable sur $I$ et $\forall x \in I, y'(x)+a(x)y(x)=-a(x)y(x)+a(x)y(x)=0$.
Donc $y$ est bien solution

***Bilan*** :
L'ensemble des solutions de $(E)$ sur $I$ est : $\{ \lambda e^{-A(x)}\mid \lambda \in \mathbb{R} \}$

#### Remarques


