---
anki_linked: 0
raisonnements:
  - double_implication
outils:
  - derivation
kh_n:
  - "11"
display_title: Convexe <=> Dérivée seconde positive
---
# Convexe $\iff$ Dérivée seconde positive

> [!objectif]
> Soit $f:I\to \mathbb{R}$ deux fois dérivable sur $I$.
> Alors "$f$ convexe sur $I$" $\iff$ "$f''$ positive sur $I$"
### Démonstration

***Sens $\implies$*** :
On suppose $f$ convexe sur $I$.
$f$ est dérivable, donc $f'$ existe, et $f$ est convexe sur $I$, donc $f'$ est croissante.
Or $f$ est deux fois dérivable, donc $f'$ est dérivable et $f''$ existe.
Enfin, $f'$ est croissante, donc $f''$ est positive.

***Sens $\impliedby$*** :
On suppose $f''$ positive sur $I$.
Donc $f'$ est croissante sur $I$, donc $f$ est convexe.

#### Remarques

Cette preuve en mobilise deux autres :
* [[convexe_derivee_croissante|Convexe <=> Dérivée Croissante]]
* [[croissante_derivee_positive|Croissante <=> Dérivée positive]]


