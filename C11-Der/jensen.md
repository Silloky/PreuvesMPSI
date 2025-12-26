---
anki_linked: 0
raisonnements:
outils:
  - dérivation
kh_n:
  - "11"
display_title: Inégalité de Jensen
---
# Inégalité de Jensen

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ une fonction convexe sur $I$.
> Pour tous :
> * $n\in \mathbb{N}^*$
> * $(x_{1},\dots x_{n})\in I^n$
> * $(\lambda_{1},\dots,\lambda_{n})\in(\mathbb{R}_{+})^n$
> 
> On a :
>$$
> \lambda_{1}+\dots+\lambda_{n}=1\implies f(\lambda_{1}x_{1}+\dots+\lambda_{n}x_{n})\leq\lambda_{1}f(x_{1})+\dots+\lambda_{n}f(x_{n})
> $$
> Ou avec des sommes :
> $$
> \sum_{k=1}^n\lambda_{k}=1\implies f\left( \sum_{k=1}^n\lambda_{n}x_{n} \right) \leq \sum_{k=1}^n\lambda_{k}f(x_{k})
> $$

### Démonstration

Pour tout $n\in \mathbb{N}^*$, on pose $H_{n}$ : "$\forall(x_{1},\dots,x_{n})\in I^n, \forall(\lambda_{1},\dots,\lambda_{n})\in(\mathbb{R}_{+})^n, \sum_{k=1}^n\lambda_{k}=1 \implies f\left( \sum_{k=1}^n \lambda_{k}x_{k}\right)\leq \sum_{k=1}^n\lambda_{k}f(x_{k})$"

***Initialisation*** en $1$ :
Soit $x_{1}\in I$ et $\lambda_{1}\in \mathbb{R}_{+}$. On suppose $\sum_{k=1}^1\lambda_{k}= \lambda_{1}=1$. 
Alors $f(\lambda_{1}x_{1})\leq f(x_{1})=\lambda_{1}f(x_{1})$.
D'où $H_{1}$.

***Hérédité*** :

Soit $n\in \mathbb{N}^*$. On suppose $H_{n}$.
Soient $(x_{1},\dots,x_{n+1})\in I^{n+1}$ et $(\lambda_{1},\dots,\lambda_{n+1})\in(\mathbb{R}_{+})^{n+1}$.
On suppose que $\sum_{k=1}^{n+1}\lambda_{k}=1$.

**Si** $\lambda_{n+1}=1$, alors $\lambda_{1}=\dots=\lambda_{n}=0$, et donc :
$f\left( \sum_{k=1}^{n+1} \lambda_{k}x_{k}\right)= \lambda_{k+1}f(x_{n+1})\leq f(x_{n+1})+\sum_{k=1}^{n}\lambda_{k}x_{k}=\sum_{k=1}^{n+1}\lambda_{k}x_{k}$

**Sinon** $\lambda_{n+1}<1$ donc $1-\lambda_{n+1}<0$ et $\sum_{k=1}^n\lambda_{k}=1-\lambda_{n+1}$.
D'où $\sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}=1$
Donc d'après $H_{n}$ :
$$
f\left( \sum_{k=1}^n \left( \frac{\lambda_{1}}{1-\lambda_{n+1}} \right)x_{k}  \right)\leq \sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}f(x_{k})= \frac{1}{1-\lambda_{n+1}} \sum_{k=1}^n \lambda_{k}f(x_{k}) 
$$
Donc en multipliant par $1-\lambda_{n+1}$ : $$(1-\lambda_{n+1})f\left(\sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}x_{k}\right)\leq \sum_{k=1}^n \lambda_{k}f(x_{k})$$
On pose $x_{-}=\min(x_{1},\dots,x_{n})\in I$ et $x_{+}=\max(x_{1},\dots,x_{n})\in I$.
On a alors : $$\sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}} x_{-}\leq \sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}x_{n}\leq \sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}x_{+}$$
Donc $x_{-}\leq \sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}x_{n}\leq x_{+}$.
Or puisque $x_{-}\in I$ et $x_{+}\in I$, on peut dire que $I$ est un intervalle, donc $\sum_{k=1}^n \frac{\lambda_{k}}{1-\lambda_{n+1}}x_{n} \in I$

Et $f$ est convexe, $x_{n+1}\in I$ et $\lambda_{n+1}\in I$, donc :
$$
f\left( \lambda_{n+1}x_{n+1}+\frac{1-\lambda_{n+1}}{1-\lambda_{n+1}}\sum_{k=1}^n \lambda_{k}x_{k}\right)\leq\lambda_{n+1}f(x_{n+1})+(1-\lambda_{n+1})f\left( \frac{1}{1-\lambda_{n+1}} \sum_{k=1}^n\lambda_{k}x_{k} \right)  
$$
Donc avec l'inégalité précédente :
$$
f\left( \sum_{k=1}^{n+1}\lambda_{k}x_{k} \right)\leq\lambda_{n+1}f(x_{n+1})+\sum_{k=1}^n\lambda_{k}f(x_{k})=\sum_{k=1}^{n+1}\lambda_{k}f(x_{k}) 
$$
D'où $H_{n+1}$


#### Remarques


