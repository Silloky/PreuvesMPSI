---
anki_linked: 0
raisonnements:
outils:
  - dérivation
kh_n:
  - "10"
display_title: Inégalité des accroissements finis
---
# Inégalité des accroissements finis

> [!objectif]
> Soit $a<b$ des réels et $f:[a,b]\to \mathbb{R}$
> On suppose :
> 1. $f$ est continue sur $[a,b]$
> 2. $f$ est dérivable sur $]a,b[$
> 3. $f'$ est bornée : $\exists(m,M)\in \mathbb{R}^{2},\forall x \in]a,b[,m\leq f'(c)\leq M$
>
Alors $m\leq \frac{f(b)-f(a)}{b-a}\leq M$
### Démonstration

D'après le théorème des [[theo_accroissements_finis|accroissements finis]], il existe $c\in]a,b[$ tel que $f'(c)=\frac{f(b)-f(a)}{b-a}$.
Or $c\in]a,b[$ donc par hypothèse, $m\leq f'(c)\leq M$.
D'où :
$$
m\leq \frac{f(b)-f(a)}{b-a}\leq M
$$

#### Remarques


