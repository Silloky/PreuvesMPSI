---
anki_linked: 0
raisonnements:
  - analyse_synthese
outils:
  - corps
kh_n:
display_title: C est un corps
---
# $(\mathbb{C},+,\times)$ est un corps

> [!objectif]
> $(\mathbb{C},+,\times)$ est un corps, i.e. un anneau commutatif dont tout élément non nul est inversible.
### Démonstration

***Montrons que $(\mathbb{C},+,\times)$ est un anneau commutatif*** :

Soit $(z,z')\in \mathbb{C}$. Donc il existe $(a,b,c,d)\in \mathbb{R}^4$ tel que $z=a+ib$ et $z'=c+id$.
Donc :
* $z\times z'=(a+ib)(c+id)=(ac-bd)+i(ad+bc)$
* $z'\times z=(c+id)(a+ib)=(ca-db)+i(cb+da)$
Or $\times$ et $+$ sont commutatives dans $\mathbb{R}$, donc $ac-bd=ca-db$ et $ad+bc=cb+da$
Donc les parties réelles et imaginaires de $z\times z'$ et $z' \times z$ sont égales, donc on peut [[identification_forme_algebrique|identifier]] et ainsi, $z\times z'=z'\times x$.
Donc $\times$ est commutative dans $\mathbb{C}$, et donc $(\mathbb{C},+,\times)$ est un anneau commutatif

***Montrons que tout élément non nul de $(\mathbb{C},+,\times)$ admet un unique inverse*** :

Soit $z \in \mathbb{C}^{2}$. On pose $a=\mathrm{Re}(z)$ et $b=\mathrm{Im}(z)$.

***Analyse*** :
Soit $z'$ un inverse de $z$.
Alors $zz'=1$ donc $(a+ib)z'=1$, donc $(a-ib)(a+ib)z'=a-ib$.
Donc $(a^{2}+b^{2})z'=a-ib$
Or $z\neq 0$ donc $(a,b)\neq(0,0)$, et donc $a^{2}+b^{2}\neq 0$
Et $a^{2}+b^{2}\in \mathbb{R}$, donc : $z'=\frac{a-ib}{a+ib}$

***Synthèse*** :
On pose $z'=\frac{a-ib}{a^{2}+b^{2}}$
Donc $zz'=\frac{(a+ib)(a-ib)}{a^{2}+b^{2}}=\frac{a^{2}+b^{2}}{a^{2}+b^{2}}=1$
Donc $z$ est bien un inverse de $z$.

***Bilan*** :
Ainsi $\forall(a,b)\in \mathbb{R},\frac{a-ib}{a+ib}$ est l'unique inverse de $a+ib$.

#### Remarques


