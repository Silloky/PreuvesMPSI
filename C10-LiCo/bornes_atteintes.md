---
anki_linked: 0
raisonnements:
  - absurde
outils:
kh_n:
  - "9"
display_title: Théorème des bornes atteintes
---
# Théorème des bornes atteintes

> [!objectif]
> Soit $(a,b)\in \mathbb{R}^{2}$ et $f$ une fonction continue sur $[a,b]$.
> Alors :
> 1. $f$ est bornée sur $[a,b]$
> 2. $f$ atteint ses bornes : $\exists (\alpha,\beta)\in[a,b]\in \mathbb{R}^{2},\forall x \in[a,b], f(\alpha)\leq f(x)\leq f(\beta)$
### Démonstration

##### 1. $f$ est bornée sur $[a,b]$

Par l'absurde, on suppose que $f$ n'est pas majorée.
Autrement dit, $(P):\forall M\in \mathbb{R},\exists x \in[a,b],f(x)> M$

Pour tout $n\geq 1$, $P$ appliqué à $M=n$, donc il existe un réel noté $x_{n}\in[a,b]$ tel que $f(u_{n})> n$.
$(u_{n})$ est bornée, donc d'après [[bolzano_weierstrass|Bolzano-Weierstrass]], il existe une extraction $\varphi$ telle que $(x_{\varphi(n)})$ converge ; on note $l$ sa limite.
Pour tout $n\in \mathbb{N}$, $a\leq u_{\varphi(n)}\leq b$ donc par [[theo_passage_lim_suites|passage à la limite]] $a\leq l\leq b$.

$u_{\varphi(n)}\to l$ et $f$ est continue sur $[a,b]$. Donc puisque $l\in[a,b]$, $f(u_{\varphi(n)})\to f(l)$.
Or d'après notre construction de $(u_{n})$, $\forall n\in \mathbb{N},f(u_{\varphi(n)})>\varphi(n)\geq n$ donc $f(u_{\varphi(n)})\to +\infty$.
Ce qui est absurde, donc $f$ est majorée.

De même, $f$ est minorée, donc $f$ est bornée sur $[a,b]$.
##### 2. $f$ atteint ses bornes

On note $M=\sup{f([a,b])}$.
Pour tout $n\geq 1$, $M- \frac{1}{n}<M$ donc $M-\frac{1}{n}$ n'est pas un majorant de $f([a,b])$, donc il existe $u_{n}\in [a,b]$ tel que $M-\frac{1}{n}<f(u_{n})$.
$(u_{n})$ est bornée donc d'après [[bolzano_weierstrass|Bolzano-Weierstrass]], il existe une extraction $\varphi$ telle que $(u_{\varphi(n)})$ converge ; on note $l$ sa limite.
$u_{\varphi(n)}\to l\in[a,b]$ et $f$ est continue sur $[a,b]$ donc $f(u_{\varphi(n)})\to f(l)$.
Or, pour tout $n\geq 1$ :
$$
M-\frac{1}{n}\leq M-\frac{1}{\varphi(n)}<f(u_{\varphi(n)})\leq M
$$
Donc $f(u_{\varphi(n)})\to M$, ainsi par unicité $M=f(l)$.


#### Remarques


