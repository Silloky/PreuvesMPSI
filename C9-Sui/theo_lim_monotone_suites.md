---
anki_linked: 1
raisonnements:
outils:
  - suites
  - limites
kh_n:
display_title: Théorème de la limite monotone (suites)
---
# Théorème de la limite monotone (suites)

> [!objectif]
>1. Toute suite croissante et majorée converge
>2. Toute suite croissante et non majorée diverge vers $+ \infty$
>3. Toute suite décroissante et minorée converge
>4. Toute suite décroissante et non minorée diverge vers $- \infty$

### Démonstration

##### 1. Toute suite croissante et majorée converge

Soit $(u_{n})$ une suite. On suppose $u$ croissante et majorée.
On pose $A=\{ u_{n}\mid n\in \mathbb{N} \}$. $A$ est non-vide (puisque $u_{0}\in A$) et majorée, donc $A$ admet une borne supérieure que l'on note $c$.
Soit $\varepsilon>0$. $c-\varepsilon<\varepsilon$ donc $c-\varepsilon$ n'est pas un majorant de $A$, donc il existe $N \in \mathbb{N}$ te lque $c-\varepsilon<u_{N}$.
Donc $\forall n\geq N, c-\varepsilon<\underbrace{ u_{N}\leq u_{n} }_{ \text{car }u \,\nearrow }\leq c< c+\varepsilon$
Donc $|u_{n}-c|\leq\varepsilon$, donc $u_{n}\to c$.

##### 2. Toute suite croissante et non majorée diverge vers $+\infty$

Soit $(u_{n})$ une suite. On suppose $u$ croissante et non-majorée.
Soit $M\in \mathbb{R}$.
$u$ est non-majorée donc il existe $N\in \mathbb{N}$ tel que $u_{N}>M$.
Donc $\forall n>N,\underbrace{ u_{n}\geq u_{N} }_{ \text{car } u\,\nearrow }>M$
Donc $u_{n}\to +\infty$.

#### Remarques


