---
anki_linked: 0
raisonnements:
  - recurrence
outils:
  - derivation
  - sommes
kh_n:
  - "10"
display_title: Formule de Leibniz
---
# Formule de Leibniz

> [!objectif]
> Soit $u:I\to \mathbb{R}$ et $v:I\to \mathbb{R}$.
> Pour tout $n\in \mathbb{N}$, si $u$ et $v$ sont $n$-fois dérivables sur $I$ alors :
>$$
> (uv)^{(n)}=\sum_{k=0}^{n}{n \choose k}u^{(k)}v^{(n-k)}
> $$
### Démonstration

Pour tout $n\in \mathbb{N}$, on pose $H_{n}$ :

> Si $u$ et $v$ sont $n$-fois dérivables sur $I$ alors $uv$ est $n$-fois dérivable sur $I$ et $$(uv)^{(n)}=\sum_{k=0}^n{n \choose k}u^{(k)}v^{(n-k)}$$

***Initialisation*** :
En $0$ : $(uv)^{(0)}=\sum_{k=0}^0{0 \choose k}u^{(k)}v^{(n-k)}={0 \choose 0}u^{(0)}v^{(0)}=uv$
Donc $H_{0}$ est vraie et $H_{n}$ est initialisée.

***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
On suppose que $u$ et $v$ sont $(n+1)$-fois dérivables.
En particulier, $u$ et $v$ sont $n$-fois dérivables, donc d'après $H_{n}$, $uv$ est $n$-fois dérivable et :
$$
(uv)^{(n)}=\sum_{k=0}^n{n \choose k}u^{(n)}v^{(n-k)}
$$
Soit $k\in[\![0,n]\!]$.
* $k\leq n<n+1$ donc $u^{(k)}$ est dérivable
* $k\geq 0>-1$ donc $n-k<n+1$ donc $v^{(n-k)}$ est dérivable.
Ainsi par somme de fonctions dérivables, $(uv)^{(n)}$ est dérivable, et donc $uv$ est $(n+1)$-fois dérivable et :
$$
\begin{align}
(uv)^{(n+1)}&=\left( (uv)^{(n)} \right)' \\
&=\left( \sum_{k=0}^n {n \choose k}u^{(n)}v^{(n-k)} \right)' \\
&=\sum_{k=0}^n{n \choose k}\left( u^{(k+1)}v^{(n-k)}+u^{(k)}v^{(n+1-k)} \right) \\
&= \sum_{k=0}^n {n \choose k}u^{(k+1)}v^{(n-k)}+\sum_{k=0}^n{n \choose k}u^{(k)}v^{(n+1-k)} \\
&=\sum_{k=1}^{n+1}{n \choose k-1}u^{(k)}v^{(n+1-k)}+\sum_{k=0}^{n}{n \choose k}u^{(k)}v^{(n+1-k)} \\
&={n\choose 0}u^{(0)}v^{(n+1)}+ \sum_{k=1}^{n}\left( {n\choose k-1}+{n \choose k} \right)u^{(k)}v^{(n+1-k)}+{n+1 \choose n+1}u^{(n+1)}v^{(0)} \\
&=\sum_{k=0}^0{n+1 \choose k}u^{(k)}v^{(n+1-k)}+\sum_{k=1}^{n}{n+1\choose k}u^{(k)}v^{(n+1-k)}+\sum_{k=n+1}^{n+1}{n+1\choose k}u^{(k)}v^{(n+1-k)} \\
(uv)^{(n+1)}&=\sum_{k=0}^{n+1}{n+1 \choose k}u^{(k)}v^{(n+1-k)}
\end{align}
$$
Donc $H_{n+1}$ est vraie et $H_{n}$ est héréditaire.


#### Remarques

Le développement de la somme est quasiment identique à celui du [[binome_de_newton|binôme de Newton]].
