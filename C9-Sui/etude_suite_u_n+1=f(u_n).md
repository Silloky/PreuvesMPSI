---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
  - recurrence
outils:
  - suites
kh_n:
  - "8"
display_title: Etude d'une suite de la forme u_{n+1}=f(u_n)
---
# Etude de $(u_{n}):$ $u_{0}\geq -1$ et $u_{n+1}=\sqrt{ u_{n}+1 }$

> [!objectif]
> Soit une suite $(u_{n})$ définie par :
>$$
> \begin{cases}
u_{0}\in[-1,+\infty[ \\
\forall n\in \mathbb{N},u_{n+1}=\sqrt{ u_{n}+1 }
\end{cases}
> $$
### Démonstration

C'est une suite de la forme $u_{n+1}=f(u_{n})$, où ici $f:x\mapsto \sqrt{ x+1 }$, donc $\mathcal{D}=[-1,+\infty[$.
On détermine le point fixe qu'on note $\alpha$ : $\alpha=\sqrt{ \alpha+1 }$, donc $\alpha=\frac{1+\sqrt{ 5 }}{2}$.

##### Si $u_{0}\in[-1,\alpha]$ :

Pour tout $n\in \mathbb{N}$, on pose $H_{n}$ : "$u_{n}$ est défini et $u_{n}\in[-1,\alpha]$".

***Initialisation*** :
En $0$ : $u_{0}$ est bien défini et par hypothèse $u_{0}\in[-1,\alpha]$
Donc $H_{0}$ est vérifié.
***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$f$ est strictement croissante et continue donc d'après la théorème de la bijection monotone :
$$
f([-1,\alpha])=[f(-1),f(\alpha)]=[0,\alpha]\subset[-1,\alpha]\subset[-1,+\infty[
$$
Donc $u_{n+1}$ est bien défini et $u_{n+1}\in[-1,\alpha]$
Donc $H_{n+1}$ est vérifié
***Bilan*** : $(u_{n})$ est définie et à valeurs dans $[-1,\alpha]$

De plus, $\forall  x \in[-1,\alpha], f(x)\geq x$, donc $\forall n\in \mathbb{N},u_{n+1}-u_{n}=f(u_{n})-u_{n}\geq 0$.
Ainsi $(u_{n})$ est croissante, en plus d'être majorée par $\alpha$.
On en déduit que $(u_{n})$ est convergente, et on note $l$ sa limite.
Or $\forall n\in \mathbb{N},-1\leq u_{n}\leq\alpha$ donc par passage à la limite $-1\leq l\leq \alpha$.

En particulier, si $f$ est continue en $a$, alors par définition, $f(x)\xrightarrow[x\to a]{}f(a)$.
Et $f$ est continue sur $[-1,\alpha]$, donc elle est continue en $l\in[-1,\alpha]$.
Or $u_{n}\to l$, donc $u_{n+1}=f(u_{n})\to f(l)$, et $u_{n+1}\to l$
Donc par unicité de la limite $f(l)=l$ et puisque l'équation du point fixe n'admettait qu'une unique solution, on peut en déduire que $l=\alpha$. 

Ainsi $u_{n}\to\alpha$.

##### Si $u_{0}\in[\alpha,+\infty[$ :

Pour tout $n\in \mathbb{N}$, on pose $H_{n}:$ "$u_{n}$ est défini et $u_{n}\in[\alpha,+\infty[$".

***Initialisation*** :
En $0$ : $u_{0}$ est bien défini et par hypothèse $u_{0}\in[\alpha,+\infty[$
Donc $H_{0}$ est vérifié.
***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$.
$f$ est strictement croissante et continue donc d'après le théorème de la bijection monotone :
$$
f([\alpha,+\infty[)=[f(\alpha),\lim_{ x \to +\infty } f(x)]=[\alpha,+\infty[\subset[-1,+\infty[
$$
Donc $u_{n+1}$ est bien défini et $u_{n+1}\in[\alpha,+\infty[$
Donc $H_{n+1}$ est vérifié.
***Bilan*** : $(u_{n})$ est définie et à valeurs dans $[\alpha,+\infty[$.

De plus, $\forall x \in[\alpha,+\infty], f(x)\leq x$ donc $\forall n\in \mathbb{N},u_{n+1}-u_{n}=f(u_{n})-u_{n}\leq 0$.
Ainsi $(u_{n})$ est décroissante, en plus d'être minorée par $\alpha$.
On en déduit que $(u_{n})$ est convergente, et on note sa limite $l$.
Or $\forall n\in \mathbb{N}, \alpha\leq u_{n}$ donc par passage à la limite $\alpha\leq l$

$f$ est continue sur $[\alpha,+\infty[$, donc elle est continue en $l\in[\alpha,+\infty[$.
Or $u_{n}\to l$, donc $u_{n+1}=f(u_{n})\to f(l)$, mais aussi $u_{n+1}\to l$.
Donc par unicité de la limite, $f(l)=l$ et puisque l'équation du point fixe n'admettait qu'une unique solution, on en déduit que $l=\alpha$.

Donc $u_{n}\to \alpha$


#### Remarques


