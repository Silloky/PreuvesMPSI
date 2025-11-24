---
anki_linked: 0
raisonnements:
outils:
  - suites
  - limites
kh_n:
  - "7"
display_title: Opérations sur les limites de suites
---
# Opérations sur les limites de suites

> [!objectif]
> Soit
>$$
> x
> $$
### Démonstration

##### 1. Somme de limites finies

On suppose que $u_{n}\to l$ et $v_{n}\to l'$.
Soit $\varepsilon>0$.
Or $\frac{\varepsilon}{2}>0$ et $u_{n}\to l$, donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq \frac{\varepsilon}{2}$.
De même, il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},|v_{n}-l|\leq \frac{\varepsilon}{2}$.
On pose $N=\max(N_{1},N_{2})$.
Soit $n\geq N$
$$
\begin{align}
|u_{n}+v_{n}-(l+l')|&=|(u_{n}-l)+(v_{n}-l')| \\
&\leq |u_{n}-l|+|v_{n}-l| \\
&=\frac{\varepsilon}{2} + \frac{\varepsilon}{2} \\
&=\varepsilon
\end{align}
$$
Donc $u_{n}+v_{n}\to l+l'$.

##### 2. Somme d'une limite finie et d'une limite infinie

On suppose $u_{n}\to l$ et $v_{n}\to +\infty$.
Soit $M\in \mathbb{R}$.
D'après les hypothèses :
* il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq 1>0$ donc $u_{n}\geq l-1$
* il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2},v_{n}\geq M-l+1$
On pose $N=\max(N_{1},N_{2})$.
Pour tout $n\geq N,u_{n}+v_{n}\geq l-1+M-l+1=M$.
Donc $u_{n}+v_{n}\to +\infty$

##### 3. Produit de deux limites finies

On suppose $u_{n}\to l$ et $v_{n}\to l'$.
Pour tout $n\in \mathbb{N}$ :
$$
\begin{align}
|u_{n}v_{n}-ll'|&=|u_{n}(v_{n}-l')+(u_{n}-l)l'| \\
&\leq|u_{n}(v_{n}-l')|+|(u_{n}-l)l'| \\
&=\underbrace{ \underbrace{ |u_{n}| }_{ \text{bornée} }\underbrace{ |v_{n}-l'| }_{ \to 0 } }_{ \to 0 }+\underbrace{ \underbrace{ |u_{n}-l| }_{ \to 0 }|l'| }_{ \to 0 } \\
|u_{n}v_{n}-ll'|&\to 0
\end{align}
$$
Donc $u_{n}\times v_{n}\to l\times l'$.

##### 4. Produit d'une limite finie et d'une limite infinie

On suppose $u_{n}\to l>0$ et $v_{n}\to +\infty$.
Soit $M>0$.
$\frac{1}{2}>0$ et $u_{n}\to l$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq \frac{1}{2}$, donc $u_{n}\geq l-\frac{1}{2}=\frac{l}{2}$.
De plus, $v_{n}\to +\infty$, donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, u_{n}\geq \frac{M}{\frac{l}{2}}$ (car $\frac{l}{2}>0$).
Donc, pour tout $n\geq\max(N_{1},N_{2}), u_{n}v_{n}\geq \frac{l}{2}\times \frac{M}{\frac{l}{2}}=M$.
Donc $u_{n}v_{n}\to +\infty$.



#### Remarques


