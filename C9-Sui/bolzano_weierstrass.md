---
anki_linked: 1
raisonnements:
  - construction
  - disjonction_de_cas
outils:
  - suites
  - sous-suites
kh_n:
display_title: Théorème de Bolzano-Weierstrass
---
# Théorème de Bolzano-Weierstrass

> [!objectif]
> Toute suite bornée admet une sous-suite convergente.
### Démonstration

Soit $(u_{n})$ une suite. On suppose $u$ bornée, donc il existe $(a,b)\in \mathbb{R}^{2}$ tel que $\forall n\geq N,a\leq u_{n}\leq b$.

On va construire deux suites $(a_{n})$ et $(b_{n})$, et une extraction $\varphi$ telles que :
* $(a_{n})$ soit décroissante
* $(b_{n})$ soit croissante
* $\forall n\in \mathbb{N},a_{n}\leq u_{\varphi(n)}\leq b_{n}$
* $\forall n\in \mathbb{N},b_{n}-a_{n}=\frac{1}{2^n}(b-a)$
* Pour tout $n\in \mathbb{N}$, il y a une infinité de termes de la suite dans $[a_{n},b_{n}]$

On pose $a_{0}=a,b_{0}=b$ et $\varphi(0)=0$.
Soit $n\in \mathbb{N}$. On suppose construits $a_{0},\dots,a_{n}$ , $b_{0},\dots,b_{n}$ et $\varphi(0),\dots,\varphi(n)$.
Par hypothèse, il existe une infinité de terme de la suite dans $[a_{n},b_{n}]$.

***Si*** : il y a une infinité de termes dans $\left[ a_{n}, \frac{a_{n}+b_{n}}{2} \right]$, on pose :
$$
\begin{cases}
a_{n+1}=a_{n} \\
b_{n+1}=\frac{a_{n}+b_{n}}{2}
\end{cases}
$$
***Sinon*** : il y a une infinité de termes dans $\left[ \frac{a_{n}+b_{n}}{2},b_{n} \right]$ et on pose :
$$
\begin{cases}
a_{n+1}=\frac{a_{n}+b_{n}}{2} \\
b_{n+1}=b_{n}
\end{cases}
$$
Dans les 2 cas on obtient que $a_{n}\leq a_{n+1}$, $b_{n}\geq b_{n+1}$ et $b_{n+1}-a_{n+1}=\frac{1}{2}(b_{n}-a_{n})=\frac{1}{2^{n+1}}(b-a)$ (par une rapide récurrence).
Et aussi, il y a une infinité de termes dans $[a_{n+1},b_{n+1}]$, donc il existe une indice qu'on note $\varphi(n+1)$ tel que $\varphi(n+1)>\varphi(n)$ et $a_{n+1}\leq u_{\varphi(n+1)}\leq b_{n+1}$.

Les suites $(a_{n})$ et $(b_{n})$ ainsi construites sont adjacentes (car l'une est croissante, l'autre décroissante, et que $b_{n}-a_{n}\to 0$).
Donc elles convergent vers une même limite qu'on note $l$.
Ainsi, pour tout $n\in \mathbb{N}, a_{n}\leq u_{\varphi(n)}\leq b_{n}$, donc par [[theo_encadrement_suites|encadrement]], $u_{\varphi(n)}\to l\in[a,b]$


#### Remarques


