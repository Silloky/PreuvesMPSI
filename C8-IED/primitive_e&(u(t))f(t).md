---
anki_linked: 0
raisonnements:
outils:
  - primitives
  - complexes
kh_n:
  - "6"
display_title: Primitive de e^(at)cos(bt) et sin(bt)
---
# Primitive de $x\mapsto e^{\alpha t}\cos(\omega t)$ et $x \mapsto e^{\alpha t}\sin(\omega t)$

> [!objectif]
> 1. Trouver une primitive de $x\mapsto e^{\alpha t}\cos(\omega t)$
> 2. Trouver une primitive de $x\mapsto e^{\alpha t}\sin(\omega t)$
### Démonstration

##### 1. Pour $\cos$

On a : $e^{\alpha t}\cos(\omega t)=\mathrm{Re}(e^{\alpha t}(\cos(\omega t)+i\sin(\omega t)))=\mathrm{Re}(e^{(\alpha+\omega i)t})$
Or la primitive de la partie réelle vaut la partie réelle de la primitive.
De plus, $\frac{1}{\alpha+\omega i}e^{(\alpha+\omega i)t}=\frac{\alpha-\omega i}{\alpha^{2}+\omega^{2}}e^{(\alpha+\omega i)t}$ est une primitive de $e^{(\alpha+\omega i)t}$.
Ainsi, avec du calcul, on obtient : la primitive $\frac{1}{13}e^{2t}(2\cos(3t)+3\sin(3t))$

##### 2. Pour $\sin$
De même, mais avec la partie imaginaire, pas réelle.
#### Remarques


