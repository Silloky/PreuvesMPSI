---
anki_linked: 0
raisonnements:
outils:
  - primitives
  - integration
kh_n:
  - "6"
  - "7"
display_title: Intégration par parties
---
# Intégration par parties

> [!objectif]
> Soit $u$ et $v$ deux fonctions de classe $\mathcal{C}^1$ sur $[a,b]$
>$$
> \int_{a}^bu'v=[uv]_{a}^b-\int_{a}^buv'
> $$
### Démonstration

Soit $u$ et $v$ deux fonctions de classe $\mathcal{C}^1$ sur $[a,b]$.
Donc $uv$ est dérivable et $(uv)'=u'v+uv'$, et donc $uv$ est une primitive de $u'v+uv'$.
Autrement dit :
$$
\begin{align}
\int_{a}^b(u'v+uv')=[uv]_{a}^b&\implies \int_{a}^bu'v+\int_{a}^buv'=[uv]_{a}^b \\&\implies \int_{a}^bu'v=[uv]_{a}^b-\int_{a}^buv'
\end{align}
$$

#### Remarques


