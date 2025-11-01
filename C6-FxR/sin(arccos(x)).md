---
anki_linked: 1
raisonnements:
outils:
  - arctrigo
kh_n:
  - "4"
display_title: sin(arccos(x))
---
# $\sin(\arccos(x))$ pour $x \in [-1,1]$

> [!objectif]
> $$
> \forall x \in[-1,1],\sin(\arccos(x))=\sqrt{ 1-x^{2} }
> $$
### Démonstration

On sait que $\cos ^{2}(\arccos x)+\sin ^{2}(\arccos x)=1$
Or $\sin ^{2}(\arccos(x))=x^{2}$ pour $x \in[-1,1]$.
Donc $\sin ^{2}(\arccos(x))=1-x^{2}$.
De plus, $\arccos(x)\in \left[ 0, \pi \right]$, or $\sin$ est positif sur $\left[ 0, \pi \right]$, donc $\sin(\arccos x)\geq0$.
Donc : $\sin(\arccos x)=\sqrt{ 1-x^{2} }$

#### Remarques

C'est très similaire (pour un même résultat) à la [[cos(arcsin(x))|démonstration]] de $\cos(\arcsin x)=\sqrt{ 1-x^{2} }$;
