---
anki_linked: 0
raisonnements:
  - recurrence
outils:
  - limites
kh_n:
  - "4"
display_title: Croissance comparée p^n/n!
---
# Croissance comparée $\frac{p^n}{n!}$

> [!objectif]
> Soit $p>1$ et $n \in \mathbb{N}$$$
> \lim_{ n \to +\infty } \frac{p^n}{n!}=0
> $$

### Démonstration

##### 1. Algébriquement

Il existe un rang $N\in \mathbb{N}$ tel que pour tout entier $k\geq N$, $k\geq 2p$, d'où $\frac{p}{k}\leq \frac{1}{2}$.
Donc pour tout $n \in \mathbb{N}$ :
$$
\frac{p^n}{n!}= \prod_{k=1}^n \frac{p}{k}=\left( \prod_{k=1}^{N-1} \frac{p}{k} \right)\left( \prod_{k=N}^n \frac{p}{k}\right)\leq \left( \prod_{k=1}^{N-1} \frac{p}{k} \right) \times \frac{1}{2^{n-N}}\xrightarrow[n\to +\infty]{}0 
$$
Or le produit est positif, donc par encadrement, $\frac{p^n}{n!}\xrightarrow[]{}0$.

##### 2. Par récurrence

Soit $p>1$.
Pour tout $n\in \mathbb{N}$, on pose $u_{n}=\frac{p^n}{n!}>0$.
Pour tout $n\in \mathbb{N}, \frac{u_{n+1}}{u_{n}}=\frac{p}{n+1}$
Il existe un $M\in \mathbb{N}$ tel que $\forall n\geq M, \frac{p}{n+1}\leq \frac{1}{2}$

Pour tout $k\in \mathbb{N}^*$, on pose $H_{k}:u_{M+k}\leq \frac{1}{2^k}u_{M}$
***Initialisation*** :
En $1$ : $\frac{u_{M+1}}{u_{M}}\leq \frac{1}{2^1}$
Donc $H_{0}$ est vraie et $H_{k}$ est initialisée en $1$.

***Hérédité*** :
Soit $k\in \mathbb{N}$. On suppose $H_{k}$.
Or $M+k \geq M$ donc $\frac{u_{M+k+1}}{u_{M+k}}\leq \frac{1}{2}$ donc $u_{M+k+1}\leq \frac{1}{2}u_{M+k}$ 
Or par hypothèse de récurrence, $u_{M+k}\leq \frac{1}{2^k}u_{M}$ donc $\frac{1}{2}u_{M+k}\leq \frac{1}{2^{k+1}}u_{M}$ donc $u_{M+k+1}\leq  \frac{1}{2^{k+1}}u_{M}$
Donc $H_{k+1}$ est vraie et $H_{k}$ est héréditaire.

***Conclusion*** : $\forall k\in \mathbb{N}^*, u_{M+k}\leq \frac{1}{2^k}u_{M}$


Donc $\forall n\geq M, 0\leq u_{n} \leq \left( \frac{1}{2} \right)^{n-M}u_{M}\xrightarrow[n\to +\infty]{}0$
Donc d'après le théorème des  gendarmes, $\frac{p^n}{n!} \xrightarrow[x\to +\infty]{}0$

#### Remarques


