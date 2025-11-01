---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
  - absurde
outils:
kh_n:
  - "4"
---
# Fonction somme non-périodique de fonctions périodiques 

> [!objectif]
> Donner (et montrer) un exemple de fonction somme de 2 fonctions périodiques qui n'est pas périodique.

### Démonstration

On pose :
$$
\begin{cases}
f:x\mapsto \cos(x) \\
g:x\mapsto \cos(x\sqrt{ 2 })
\end{cases}
$$
Par définition, $f$ est $2\pi$ périodique et $g$ est est $\frac{2\pi}{\sqrt{ 2 }}=\pi \sqrt{ 2 }$ périodique.

Soit $x \in \mathbb{R}$ tel que $(f+g)(x)=2$. Donc :
$$
\underbrace{ \cos(x) }_{ \leq 1 }+\underbrace{ \cos(x\sqrt{ 2 }) }_{ \leq 1 }=1+1
$$
Donc $\cos(x)=1$ et $\cos(x\sqrt{ 2 })=1$.
Donc :
* il existe $k_{1}\in \mathbb{Z}$ tel que $x=2k_{1}\pi$
* il existe $k_{2}\in \mathbb{Z}$ tel que $x\sqrt{ 2 }=2k_{2}\pi$
On suppose par l'absurde que $x\ne0$, alors :
$$
\sqrt{ 2 }=\frac{2k_{2}\pi}{x}=\frac{2k_{2}\pi}{2k_{1}\pi}=\frac{k_{2}}{k_{1}}\in \mathbb{Q}
$$
Ce qui est absurde, donc $x=0$.

Ainsi $f+g$ ne prend la valeur $2$ qu'en $0$.
$f+g$ ne peut donc pas être périodique.

#### Remarques


