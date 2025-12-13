---
anki_linked: 0
raisonnements:
outils:
  - derivation
  - limites
kh_n:
  - "10"
display_title: Théorème des accroissements finis
---
# Théorème des accroissements finis

> [!objectif]
> Soit $a<b$ des réels et $f:[a,b]\to \mathbb{R}$.
> On suppose :
> 1. $f$ continue sur $[a,b]$
> 2. $f$ dérivable sur $]a,b[$
>
> Alors il existe $c\in]a,b[$ tel que $f'(c)=\frac{f(b)-f(a)}{b-a}$
### Démonstration

On pose $g:x\mapsto f(x)- \frac{f(b)-f(a)}{a-b}\times f(x)$.
En particulier :
* $g(a)=f(a)-\frac{f(b)-f(a)}{b-a}=\frac{bf(a)-af(b)}{b-a}$
* $g(b)=f(b)-\frac{f(b)-f(a)}{b-a}\times f(b)=\frac{bf(a)-af(b)}{b-a}$
Or $g$ est continue sur $[a,b]$, dérivable sur $]a,b[$ et $g(a)=g(b)$.
Donc d'après le théorème de [[theo_rolle|Rolle]], il existe $c\in]a,b[$ tel que $g'(c)=0$.
Or pour tout $x \in]a,b[$ tel que $g'(x)=f'(x)-\frac{f(b)-f(a)}{b-a}$.
D'où $f'(c)=\frac{f(b)-f(a)}{b-a}$

#### Remarques

C'est à la fois une reformulation et une généralisation du théorème de Rolle.
Il existe un point sur l'intervalle $]a,b[$ auquel la tangente est parallèle à la corde $((a,f(a)),(b,f(b)))$.

