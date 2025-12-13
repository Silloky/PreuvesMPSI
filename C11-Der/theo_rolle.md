---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
outils:
  - derivation
kh_n:
  - "10"
display_title: Théorème de Rolle
---
# Théorème de Rolle

> [!objectif]
> Soit $a<b$ deux réels et $f:[a,b]\to \mathbb{R}$.
> On suppose que :
> 1. $f$ est continue sur $[a,b]$
> 2. $f$ est dérivable sur $]ab[$
> 3. $f(a)=f(b)$
>
>Alors la dérivée s'annule en un point de $]a,b[$ : $\exists c\in ]a,b[,f'(c)=0$
### Démonstration

Par hypothèse, $f$ est continue sur $[a,b]$ donc d'après le théorème des [[bornes_atteintes|bornes atteintes]], $f$ est bornée et atteint ses bornes : il existe $(c,d)\in[a,b]^{2}$ tels que : $\forall[a,b],f(c)\leq f(x)\leq f(d)$.

***Si $(c,d)\in \{ a,b \}$*** :
Alors $c=a$ ou $c=b$ donc $f(c)=f(a)$ ou $f(c)=f(b)$. 
Or $f(a)=f(b)$ donc $f(c)=f(a)$, et de même, $f(d)=f(a)$.
Donc pour tout $x \in[a,b],f(a)=f(c)\leq f(x)\leq f(d)=f(a)$, donc $f(x)=f(a)$.
Ainsi $f$ est constante sur $[a,b]$, et en particulier $f'\left( \frac{a+b}{2} \right)=0$

***Si $c\not\in \{ a,b \}\lor d\not\in \{ a,b \}$*** :
On suppose que $c\not\in \{ a,b \}$, car le cas $d\not\in \{ a,b \}$ est similaire.
On a $c \in[a,b]$ et $c\not\in \{ a,b \}$ donc $c\in]a,b[$.
$f$ admet un minimum global en $c$, donc un extrémum local en $c$. 
De plus, $f$ est dérivable sur $]a,b[$, or $c\in]a,b[$, donc $f$ est dérivable en $c$.
Ainsi d'après le théorème de l'[[theo_extremum_local|extrémum local]], $f'(c)=0$.

Donc dans tous les cas, $f'$ s'annule sur $]a,b[$. 


#### Remarques


