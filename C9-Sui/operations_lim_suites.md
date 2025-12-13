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
> 1. Somme de limites finies
> 2. Somme d'une limite fini et d'une limite infinie
> 3. Produit de deux limites finies
> 4. Produit d'une limite finie positive et d'une limite infinie positive
> 5. Produit d'une suite bornée et d'une limite nulle
> 6. Produit d'une limite par un réel
> 7. Produit de deux limites négatives infinies
> 8. Passage à l'inverse d'une limite finie non nulle
> 9. Passage à l'inverse d'une limite infinie négative
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

##### 4. Produit d'une limite finie positive et d'une limite infinie positive

On suppose $u_{n}\to l>0$ et $v_{n}\to +\infty$.
Soit $M>0$.
$\frac{1}{2}>0$ et $u_{n}\to l$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},|u_{n}-l|\leq \frac{1}{2}$, donc $u_{n}\geq l-\frac{1}{2}=\frac{l}{2}$.
De plus, $v_{n}\to +\infty$, donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, u_{n}\geq \frac{M}{\frac{l}{2}}$ (car $\frac{l}{2}>0$).
Donc, pour tout $n\geq\max(N_{1},N_{2}), u_{n}v_{n}\geq \frac{l}{2}\times \frac{M}{\frac{l}{2}}=M$.
Donc $u_{n}v_{n}\to +\infty$.

##### 5. Produit d'une suite bornée et d'une limite nulle

On suppose $u$ bornée et $v_{n}\to 0$.
$u$ est bornée, donc il existe $M\in \mathbb{R}_{+}^*$ tel que $\forall n\in \mathbb{N},|u_{n}|\leq M$.
Soit $\varepsilon>0$. Alors $\frac{\varepsilon}{M}>0$, et $v_{n}\to 0$, donc il existe $N\in \mathbb{N}$ tel que $\forall n\in \mathbb{N},|v_{n}|\leq \frac{\varepsilon}{M}$.
Ainsi $\forall n\geq N, |u_{n}\times v_{n}|=|u_{n}|\times|v_{n}|\leq M\times \frac{\varepsilon}{M}=\varepsilon$.
Donc $u_{n}v_{n}\to 0$

##### 6. Produit d'une limite par un réel

On suppose $u_{n}\to l$ et soit $\lambda \in \mathbb{R}$.
$\forall n\in \mathbb{N},\lambda u_{n}-\lambda l=\underbrace{ \lambda }_{ \text{bornée} }(\underbrace{ u_{n}-l }_{ \to 0 })\to 0$.
Donc $\lambda u_{n}\to\lambda l$

##### 7. Produit de deux limites négatives infinies

On suppose $u_{n}\to -\infty$ et $v_{n}\to -\infty$.
Soit $M\geq 0$.
D'après les hypothèses :
* $u_{n}\to -\infty$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall n\geq N_{1},u_n \leq -1<0$
* $v_{n}\to -\infty$ donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, v_{n}\leq -M<0$
Soit $n\geq N_{1}+N_{2}$.
* $n\geq N_{1}+N_{2}\geq N_{1}$ donc $u_{n}\leq -1$ donc $-u_{n}\geq 1\geq 0$
* $n\geq N_{1}+N_{2}\geq N_{2}$ donc $v_{n}\leq -M$ donc $-v_{n} \geq M\geq 0$
Donc :
$u_{n}v_{n}=(-u_{n})(-v_{n})\geq 1\times M=M$.
Donc $u_{n}v_{n}\to +\infty$.

##### 8. Passage à l'inverse d'une limite finie non nulle (APCR)

On suppose que $u_{n}\to l$ et que $u_{n}\neq 0\;\text{APCR}$.
$\frac{l}{2}>0$ et $u_{n}\to l$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N, |u_{n}-l|\leq \frac{l}{2}$, donc $u_{n}\geq l-\frac{l}{2}=\frac{l}{2}>0$ donc $u_{n}>0$, et ainsi $\left( \frac{1}{u_{n}} \right)_{n\in \mathbb{N}}$ est bien définie.
$$\forall n\geq N_{1},\left| \frac{1}{u_{n}} -\frac{1}{l}\right|=\left| \frac{l-u_{n}}{u_{n}l} \right|=\underbrace{ \frac{1}{u_{n}} }_{ \text{bornée} }\times \underbrace{ \frac{1}{n} }_{ \text{bornée} }\times \underbrace{ |u_{n}-l| }_{ \to 0 }\to 0$$
Donc $\frac{1}{u_{n}}\to \frac{1}{l}$.

##### 9. Passage à l'inverse d'une limite infinie négative

On suppose que $u_{n}\to -\infty$.
Soit $\varepsilon>0$. Il existe $M>0$ tel que $\frac{1}{M}\leq\varepsilon$.
Or $u_{n}\to-\infty$ donc il existe $N\in \mathbb{N}$ tel que $\forall n\geq N,u_{n}\leq -M <0$.
Soit $n\geq N$. On a : $\frac{1}{u_{n}}\geq \frac{1}{-M}$ donc $\left| \frac{1}{u_{n}} \right|=-\frac{1}{u_{n}}\leq \frac{1}{M}\leq \varepsilon$
Donc $\frac{1}{u_{n}}\to 0^-$.
#### Remarques


