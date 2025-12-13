---
anki_linked: 0
raisonnements:
outils:
  - derivation
  - limites
kh_n:
  - "10"
display_title: Théorème de l'extrémum local
---
# Théorème de l'extrémum local

> [!objectif]
> Soit $a<b$ deux réels, $f:[a,b]\to \mathbb{R}$ et $c\in[a,b]$.
> On suppose que :
> 1. $f$ admet un extrémum local en $c$
> 2. $f$ est dérivable en $c$
> 3. $c\in]a,b[$
> 
> Alors $f'(c)=0$
### Démonstration

On a:
* $c\in]a,b[$ donc il existe $\eta_{1}>0$ tel que $[c-\eta_{1},c+\eta_{1}]\subset[a,b]$.
* $f$ admet un extrémum local en $c$ ; on suppose que c'est un maximum local (le cas minimum est similaire), donc il existe $\eta_{2}>0$ tel que $\forall x \in[a,b]\cap[c-\eta_{2},c+\eta_{2}],f(x)\leq f(c)$
On pose $\eta=\min(\eta_{1},\eta_{2})>0$.

Pour tout $x \in[c-\eta,c], \frac{\overbrace{ f(x)-f(c) }^{ \leq 0 }}{\underbrace{ x-c }_{ <0 }}\geq 0$
Or $f$ est dérivable en $c$ donc $\frac{f(x)-f(c)}{x-c}\xrightarrow[x\to c^-]{}f'(c)$.
Par passage à la limite, on en déduit que $f'(c)\geq 0$.
De même, avec $x \in[c,c+\eta]$, on obtient que $f'(c)\leq 0$.

Ainsi $f'(c)=0$

#### Remarques


