---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - groupe
  - bornessup
kh_n:
display_title: Sous-groupes additifs de R
---
# Sous-groupes additifs de $\mathbb{R}$

> [!objectif]
> Les sous-groupes de $(\mathbb{R},+)$ sont soit de la forme $\alpha \mathbb{Z}$ avec $\alpha \in \mathbb{R}_{+}$ soit denses dans $\mathbb{R}$.

### Démonstration

Soit $H$ un sous-groupe de $(\mathbb{R},+)$.

Si $H=\{ 0 \}$, alors $H=0\mathbb{Z}$, et si $H=\mathbb{R}$, alors $H$ est dense dans $\mathbb{R}$.
Donc on peut supposer que $H\neq \{ 0 \}$ et $H\neq \mathbb{R}$.
On pose $H_{+}^*=H\cap \mathbb{R}_{+}^*$.

$H\neq \{ 0 \}$, donc il existe $x \in H$ tel que $x\neq 0$.
Si $x>0$, alors $x \in H_{+}^*$
Si $x<0$, alors $-x \in H_{+}^*$
Donc dans tous les cas, $H_{+}^*$ est non-vide.
De plus, $\mathbb{R}_{+}^*$ est minoré par $0$, donc $H_{+}^*$ aussi.
Ainsi $H_{+}^*$ admet une borne inférieure qu'on note $\alpha\geq 0$.

***Si $\alpha>0$*** :
Par l'absurde, on suppose que $\alpha \not\in H_{+}^*$.
$\alpha>0$, donc $\alpha<2\alpha$. Donc $2\alpha$ n'est pas la borne inférieure, donc il existe $x \in H_{+}^*$ tel que $x<2\alpha$.
Or $\alpha$ est la borne inférieure, donc $\alpha<x$, donc $x$ n'est pas un minorant de $H_{+}^*$.
Donc il existe $y \in H_{+}^*$ tel que $y<x$, et de même, $\alpha<y$.
Ainsi, on a $\alpha<y<x<2\alpha$.
$x$ et $y$ sont dans $H$, donc puisque $(H,+)$ est un sous-groupe, $x-y\in H$.
Or $x>y$, donc $x-y>0$, d'où $x-y \in \mathbb{R}_{+}^*$.
Donc $x-y\in H_{+}^*$.
De plus, $x-y<2\alpha-y<2\alpha-\alpha=\alpha$.
Ce qui est absurde, d'où $\alpha \in H_{+}^*$, donc $\langle \alpha \rangle=\alpha \mathbb{Z}\subset H$ (sens $\subset$)

(Sens $\supset$) Soit $x \in H$. 
$\alpha\neq 0$ donc on peut écrire que $\mathbb{R}=\bigcup_{k\in \mathbb{Z}}[k\alpha,(k+1)\alpha[$.
En particulier, pour $x \in H\subset \mathbb{R}$ : il existe $k \in \mathbb{Z}$ tel que $k\alpha\leq x<(k+1)\alpha$, donc $0\leq x-k\alpha\leq\alpha$ 
$x$ et $\alpha$ sont dans $H$ et $\alpha \mathbb{Z}\subset H$, donc puisque $k\in \mathbb{Z}$, $x-k\alpha \in H$.
Or $x-k\alpha\lt\alpha$, donc $x-k\alpha \not\in H_{+}^*$ d'où $x-k\alpha \in H\setminus H_{+}^*=\{ 0 \}$ 
Donc $x-k\alpha=0$, donc $x=k\alpha \in\alpha \mathbb{Z}$

Donc $H=\alpha \mathbb{Z}$

***Si $\alpha=0$*** :
Soit $(a,b)\in \mathbb{R}^{2}$. On suppose que $a<b$, donc $b-a>0=\alpha$. Or $\alpha$ est la borne inférieure, donc il existe $x \in H_{+}^*$ tel que $x<b-a$.
Puisque $x\neq 0$, on peut écrire $\mathbb{R}=\bigcup_{k\in \mathbb{Z}}[kx,(k+1)x[$, d'où pour $a$ : il existe $k \in \mathbb{Z}$ tel que $kx\leq a<(k+1)x=kx+x$.
Or $kx\leq a$ et $x<b-a$, donc $a<(k+1)x<b$.
De plus $k+1 \in \mathbb{Z}$, donc $(k+1)x \in \langle x \rangle\subset H$
D'où $(k+1)x \in H\cap]a,b[$, donc $H\cap]a,b[\neq \emptyset$.
Donc $H$ est dense dans $\mathbb{R}$.


#### Remarques


