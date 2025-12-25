---
anki_linked: 0
raisonnements:
  - construction
outils:
  - limites
kh_n:
  - "9"
display_title: Théorème des Valeurs Intermédiaires (Annulation)
---
# Théorème des Valeurs Intermédiaires (Annulation)

> [!objectif]
> Soit $a<b$ deux réels et $f:[a,b]\to \mathbb{R}$ continue sur $[a,b]$.
> Si $f(a)\leq 0$ et $f(b)\geq 0$, alors $f$ s'annule sur $[a,b]$
### Démonstration

On va construire deux suites $(a_{n})$ et $(b_{n})$ telles que $(a_{n})$ soit croissante, $(b_{n})$ décroissante, et, pour tout $n\in \mathbb{N}, b_{n}-a_{n}=-\frac{1}{2^n}(b-a)$ et $f(a_{n})\leq 0$ et $f(b_{n})\geq 0$.

On pose $a_{0}=a$ et $b_{0}=b$.
Soit $n\in \mathbb{N}$. On suppose $a_{0},\dots a_{n}$ et $b_{0},\dots,b_{n}$ construits qui conviennent.

Si $f\left( \frac{a_{n}+b_{n}}{2} \right)\leq 0$, on pose $a_{n+1}=\frac{a_{n}+b_{n}}{2}$ et $b_{n+1}=b_{n}$.
Sinon on pose $a_{n+1}=a_{n}$ et $b_{n+1}=\frac{a_{n}+b_{n}}{2}$.
Dans tous les cas, $a_{n}\leq a_{n+1}$ et $b_{n+1}\leq b_{n}$
Et : $b_{n+1}-a_{n+1}=\frac{1}{2}(b_{n}-a_{n})=\frac{1}{2^{n+1}}(b-a)$.

Donc $(a_{n})$ est croissante, $(b_{n})$ décroissante et $b_{n}-a_{n}\to 0$, ainsi $(a_{n})$ et $(b_{n})$ sont adjacentes et il existe $c\in[a,b]$ tel que $a_{n}\to c$ et $b_{n}\to c$.
$a_{n}\to c$ et $f$ est continue en $c\in[a,b]$ donc $f(a_{n})\to f(c)$.
Or $\forall n\in \mathbb{N},f(a_{n})\leq 0$, donc $f(c)\leq 0$ ; de même, $f(b_{n})\geq 0$, donc $f(c)\geq 0$.
Ainsi $f(c)=0$.

Donc $f$ s'annule en $c$.


#### Remarques


