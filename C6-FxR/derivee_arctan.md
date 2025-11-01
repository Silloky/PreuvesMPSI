---
anki_linked: 1
raisonnements:
outils:
  - bijection
kh_n:
  - "4"
display_title: Dérivée de arctan
---
# Dérivée de $\arctan$

> [!objectif]
> La fonction $\arctan:\mathbb{R}\to \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$ est dérivable sur $\mathbb{R}$ et sa dérivée vaut $\forall x \in \mathbb{R},\arctan'(x)=\frac{1}{1+x^{2}}$
### Démonstration

$\tan:\left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]\to \mathbb{R}$ est dérivable sur $\left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$ et $\forall x \in \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right],\tan'(x)=1+\tan ^{2}(x)\neq 0$
Donc d'après le [[theo_derivabilite_bijection_reciproque|théorème de la dérivabilité de la bijection réciproque]], $\arctan:\mathbb{R}\to \left[ -\frac{\pi}{2}, \frac{\pi}{2} \right]$ est dérivable sur $\mathbb{R}$ et :
$$
\forall x \in \mathbb{R},\arctan'(x)=\frac{1}{1+\tan ^{2}(\arctan(x))}=\frac{1}{1+x^{2}}
$$

#### Remarques


