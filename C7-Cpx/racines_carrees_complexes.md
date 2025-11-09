---
anki_linked: 1
raisonnements:
  - analyse_synthese
outils:
kh_n:
display_title: Existence et duplicité des racines carrées complexes
---
# Existence et duplicité des racines carrées complexes

> [!objectif]
> Soit $a\in \mathbb{C}^*$. Il existe exactement deux complexes dont le carré vaut $a$, et ils sont opposés.
### Démonstration

Soit $a\in \mathbb{C}$.

***Synthèse*** :
Il existe $r>0$ et $t\in \mathbb{R}$ tels que $a=re^{it}$.
Alors $\sqrt{ r }e^{i t/2}$ et $-\sqrt{ r }e^{it/2}$ conviennent.

***Analyse*** :
Soit $z\in \mathbb{C}$. On suppose que $z^{2}=a$.
On pose $z_{0}=\sqrt{ r }e^{it/2}$.
$$
\begin{align}
z^{2}=z_{0}^{2} \quad&\text{donc}\quad z^{2}-z_{0}^{2}=0 \\
&\text{donc}\quad (z-z_{0})(z+z_{0})=0 \\
&\text{donc}\quad z-z_{0}=0 \quad\text{ou}\quad z+z_{0}=0 \\
&\text{donc}\quad z=z_{0} \quad\text{ou}\quad z=-z_{0}
\end{align}
$$

#### Remarques


