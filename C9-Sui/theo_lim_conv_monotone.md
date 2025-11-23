---
anki_linked: 0
raisonnements:
outils:
  - suites
  - bornessup
kh_n:
  - "7"
display_title: Théorème de la limite/convergence monotone
---
# Théorème de la limite/convergence monotone

> [!objectif]
> Si $u$ est croissante et majorée alors $u$ converge.
### Démonstration

Soit $u$ une suite. On suppose $u$ croissante et majorée.
On pose $A=\{ u_{n}\mid n\in \mathbb{N} \}$. 
$A$ est non-vide (puisque $u_{0}\in A$) et et majoré (car $u$ est majorée). $A$ admet donc une borne supérieure que l'on note $c$.

Soit $\varepsilon>0$. 
$c-\varepsilon<c$ donc $c-\varepsilon$ n'est pas un majorant de $A$, et donc il existe $N\in \mathbb{N}$ tel que $c-\varepsilon<u_{N}$.
Donc, puisque $u$ est croissante, pour tout $n\geq N$, $c-\varepsilon<u_{N}\leq u_{n}\leq c<c+\varepsilon$, et donc $|u_{n}-c|\geq\varepsilon$.
Donc $u\to c$.

#### Remarques


