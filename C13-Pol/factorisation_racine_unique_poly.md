---
anki_linked: 0
raisonnements:
outils:
  - polynome
kh_n:
display_title: Factorisation simple par une racine
---
# Factorisation simple par une racine

> [!objectif]
>$$
> \forall P\in \mathbb{K}[X],\forall \alpha \in K,P(\alpha)=0\iff \exists Q\in \mathbb{K}[X],P(X)=(X-\alpha)Q(X)
> $$
### Démonstration

Soit $P\in \mathbb{K}[X]$ et $\alpha \in \mathbb{K}$.

**Sens $\impliedby$** : évident

**Sens $\implies$** :
On suppose $P(\alpha)=0$

##### 1. En passant par les coefficients

Notons $P(X)=\sum_{k=0}^na_{k}X^k$. Alors :
$$
\begin{align}
P(X)&=P(X)-P(\alpha) \\
&=\sum_{k=0}^na_{k}X^k-\sum a_{k}\alpha^k \\
&=\sum_{k=0}^na_{k}(X^k-\alpha^k) \\
&=\sum_{k=0}^na_{k}(X-\alpha)\sum_{i=0}^{k-1}\alpha^{k-1-i}X^i \\
P(X)&=(X-\alpha)\underbrace{ \sum_{i=0}^{n-1}\left( \sum_{k=i+1}^{n}a_{k}\alpha^{k-1-i} \right)X^i }_{ \in\,\mathbb{K}[X] }
\end{align}
$$
##### 2. En passant par une [[division_euclidienne_poly|division euclidienne]]

On effectue la division euclidienne de $P(X)$ par $X-\alpha$.
Il existe $(Q,R)\in \mathbb{K}[X]^{2}$ tel que :
$$
\begin{cases}
P(X)=(X-\alpha)Q(X)+R(X) \\
\deg(R)<\deg(X-\alpha)=1
\end{cases}
$$
Donc $\deg(R)\leq 0$, d'où $R$ est constante. Or $P(\alpha)=(\alpha-\alpha)Q(\alpha)+R(\alpha)=0$ donc $R(\alpha)=0$, et ainsi $R(X)=0$.
D'où $P(X)=(X-\alpha)Q(X)$.

##### 3. En passant par la formule de [[taylor_poly|Taylor]]

D'après la formule de Taylor : $\displaystyle P(X)=\sum_{k\in \mathbb{N}} \frac{P^{(k)}(\alpha)}{k!}(X-\alpha)^k$.
Or $P(\alpha)=0$ donc $\frac{P^{(0)}(\alpha)}{0!}=0$ d'où :
$$
P(X)=\sum_{k\in \mathbb{N}^*} \frac{P^{(k)}(\alpha)}{k!}(X-\alpha)^{k}=(X-\alpha)\underbrace{ \sum_{k\in \mathbb{N}^*} \frac{P^{(k)}(\alpha)}{k!}(X-\alpha)^{k-1} }_{ \in }
$$

#### Remarques


