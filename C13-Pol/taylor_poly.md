---
anki_linked: 0
raisonnements:
outils:
  - polynome
  - sommes
kh_n:
display_title: Formule de Taylor polynomiale
---
# Formule de Taylor polynomiale

> [!objectif]
>$$
> \forall P\in \mathbb{K}[X],\forall a \in \mathbb{K},P(X)=\sum_{k\in \mathbb{N}} \frac{P^{(k)}(a)}{k!}(X-a)^k
> $$
### Démonstration

**On se place d'abord dans le cas où $a=0$.**
Soit $Q\in \mathbb{K}[X]$. Il existe $n\in \mathbb{N}$ et des scalaires $a_{0},\dots,a_{n}$ tels que $Q(X)=\sum_{k=0}^na_{k}X^k$.
Soit $i \in \mathbb{N}$.
$$
\begin{align}
Q^{(i)}(X)&=\left( \sum_{k=0}^na_{k}X^k \right)^{(i)}\\
&=\sum_{k=0}^na_{k}\left( X^k \right)^{(i)}\\
&=\sum_{k=i}^na_{k} \frac{k!}{(k-i)!}X^{k-1} \\
Q^{(i)}(X)&=a_{i}i!X ^0+a_{i+1}(i+1)!X+\dots+a_{n} \frac{n!}{(n-i)!}X^{n-i}
\end{align}
$$
D'où $Q^{(i)}(0)=a_{i}i!$ et ainsi $a_{i}= \frac{Q^{(i)}(0)}{i!}$.
Ainsi $Q(X)=\sum_{k=0}^n \frac{Q^{(k)}(0)}{k!}X^{k}=\sum_{k\in \mathbb{N}} \frac{Q^{(k)}(0)}{k!}X^{k}$

**Maintenant pour un $a$ quelconque.**
Soit $P\in \mathbb{K}[X]$ et $a\in \mathbb{K}$.
On pose $Q(X)=P(X+a)$, d'où $Q'(X)=P'(X+a)\times 1$ et $Q''(X)=P''(X+a)\times 1 \times 1$.
Par récurrence évidente $\forall k \in \mathbb{N},Q^{(k)}(X)=P^{(k)}(X+a)$.
En particulier, $Q^{(k)}(0)=P^{(k)}(a)$.
On applique la formule précédente pour $Q$ en $0$ :
$$
Q(X)=\sum_{k\in \mathbb{N}} \frac{Q^{(k)}(0)}{k!}X^{k}=\sum_{k\in \mathbb{N}} \frac{P^{(k)}(a)}{k!}X^{k}
$$
Or $P(X)=Q(X-a)$, d'où :
$$
P(X)=\sum_{k\in \mathbb{N}} \frac{P^{(k)}(a)}{k!}(X-a)^k
$$

#### Remarques


