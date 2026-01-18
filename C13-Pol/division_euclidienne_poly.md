---
anki_linked: 0
raisonnements:
outils:
  - polynome
  - arithmetique
kh_n:
display_title: Division euclidienne polynomiale
---
# Division euclidienne polynomiale

> [!objectif]
>$$
> \forall (A,B)\in \mathbb{K}[X]\times \mathbb{K}[X]^*,\exists!(Q,R)\in \mathbb{K}[X]^{2}, \begin{cases}
A=BQ+R \\
\deg(R)<\deg(B)
\end{cases}
> $$
### Démonstration

Soit $B\in \mathbb{K}[X]^*$.
##### 1. Existence

Notons $d\in \mathbb{N}$ le degré de $B$.
Pour tout $n\geq d-1$, on pose $H_{n}$ : "pour tout $A\in \mathbb{K}_{n}[X]$, il existe un couple $(Q,R)$ tel que $A=BQ+R$ et $\deg(R)<\deg(B)$".

**Initialisation** (en $d-1$) : Soit $A\in \mathbb{K}_{d-1}[X]$. Le couple $(B,Q)=(0,A)$ convient, d'où $H_{d-1}$.

**Hérédité** :
Soit $n\geq d-1$. On suppose $H_{n}$.
Soit $A\in \mathbb{K}_{n+1}[X]$.

Si $A\in \mathbb{K}_{n}[X]$, alors d'après $H_{n}$ il existe un couple qui convient.
On suppose donc que $\deg(A)=n+1$, et donc il existe $\lambda \in \mathbb{K}^*$ et $A_{1}\in \mathbb{K}_{n}[X]$ tels que $A(X)=\lambda X^{n+1}+A_{1}(X)$.

Or $B$ est de degré $d$, donc il existe $\beta \in \mathbb{K}^*$ et $B_{1}\in \mathbb{K}_{d-1}[X]$ tels que $B(X)=\beta X^{d}+B_{1}(X)$.
Alors :
$$
\left( \frac{\lambda}{\beta}X^{n+1-d} \right)B(X)=\left( \frac{\lambda}{\beta}X^{n+1-d} \right)(\beta X^d+B_{1}(X))=\lambda X^{n+1}+\frac{\lambda}{\beta}X^{n+1-d}B_{1}(X)
$$
Donc :
$$
A(X)-\left( \frac{\lambda}{\beta}X^{n+1-d} \right)B(X)=\cancel{ \lambda X^{n+1} }+A_{1}(X)\cancel{ -\lambda X^{n+1} }-\frac{\lambda}{\beta}X^{n+1-d}B_{1}(X)\in \mathbb{K}_{n}[X]
$$
Ainsi d'après $H_{n}$, il existe $(Q_{1},R_{1})\in \mathbb{K}[X]^2$ tel que $A_{1}(X)-\frac{\lambda}{\beta}X^{n+1-d}B_{1}(X)=BQ_{1}(X)+R_{1}(X)$ et $\deg(R_{1})<\deg(B)$.
Donc $A(X)-\left( \frac{\lambda}{\beta}X^{n+1-d} \right)B(X)=B(X)Q_{1}(X)+R_{1}(X)$.
D'où $A(X)=\left( \frac{\lambda}{\beta}X^{n+1-d}+Q_{1}(X) \right)B(X)+R_{1}(X)$ avec $\deg(R_{1})<\deg(B)$.
Donc $H_{n+1}$.

**Bilan** : la division euclidienne d'un polynôme non nul existe.
##### 2. Unicité

Soit $A\in \mathbb{K}[X]$ et $(Q_{1},R_{1})$ et $(Q_{2},R_{2})$ deux couples qui conviennent :
$$
A=\begin{cases}
BQ_{1}+R_{1} \\
BQ_{2}+R_{2}
\end{cases}
$$
Donc $B(Q_{1}-Q_{2})=R_{2}-R_{1}$, d'où $\deg(B)+\deg(Q_{1}-Q_{2})=\deg(R_{2}-R_{1})$.
Or $\deg(R_{2}-R_{1})<\deg(B)$, donc $\deg(Q_{1}-Q_{2})<0$.
Ainsi $\deg(Q_{1}-Q_{2})=-\infty$ et $Q_{1}-Q_{2}=0$.

Donc $Q_{1}=Q_{2}$, d'où $R_{1}=R_{2}$.
Ainsi $(Q_{1},R_{1})=(Q_{2},R_{2})$, ce qui montre l'unicité de la division euclidienne.


#### Remarques


