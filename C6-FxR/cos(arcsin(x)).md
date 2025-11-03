---
anki_linked: 1
raisonnements:
outils:
  - trigo
kh_n:
  - "4"
display_title: cos(arcsin(x))
---
# $\cos(\arcsin(x))$ pour $x \in [-1,1]$

> [!objectif]
> $$
> \forall x \in[-1,1],\cos(\arcsin(x))=\sqrt{ 1-x^{2} }
> $$
### Démonstration

On sait que $\cos ^{2}(\arcsin x)+\sin ^{2}(\arcsin x)=1$
Or $\sin ^{2}(\arcsin(x))=x^{2}$ pour $x \in[-1,1]$.
Donc $\cos ^{2}(\arcsin(x))=1-x^{2}$.
De plus, $\arcsin(x)\in \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$, or $\cos$ est positif sur $\left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$, donc $\cos(\arcsin x)\geq0$.
Donc : $\cos(\arcsin x)=\sqrt{ 1-x^{2} }$

#### Remarques

C'est très similaire (pour un même résultat) à la [[sin(arccos(x))|démonstration]] de $\sin(\arccos x)=\sqrt{ 1-x^{2} }$;
