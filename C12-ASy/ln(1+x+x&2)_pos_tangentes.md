---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "12"
display_title: Position de x->ln(1+x+x^2)
---
# Position de $x\mapsto \ln(1+x+x^{2})$ par rapport à ses tangentes $0$ et en $1$

> [!objectif]
> Soit $f:x\mapsto \ln(1+x+x^{2})$.
> Alors :
> * sa tangente en $0$ a pour équation $y=x$ et est en-dessous de $f$
> * sa tangente en $1$ a pour équation $y=x+1-\ln(3)$
### Démonstration

##### 1. En $0$
On détermine le $DL_{2}(0)$ de $f$ :
$$
\ln(1+(x+x^{2}))=(x+x^{2})- \frac{(x+x^{2})^{2}}{2}+o(x^{2})=x+\frac{x^{2}}{2}+o(x^{2})
$$
D'où $f(x)=x+o(x)$, donc la tangente à $f$ en $0$ a pour équation $y_{0}=x$.
De plus $f(x)-y_{0}=\frac{x^{2}}{2}+o(x^{2})\sim \frac{x_{2}}{2}\geq 0$.
Donc $f$ est au-dessus de sa tangente en $0$.

##### 2. En $1$
On pose $g:h\mapsto f(h+1)$.
On détermine le $DL_{2}(0)$ de $g$ :
$$
\begin{align}
g(h)&=\ln(1+(h+1)+(h+1)^{2}) \\
&=\ln(3+3h+h^{2}) \\
&=\ln\left( 3\left( 1+h+\frac{1}{3}h^{2} \right) \right) \\
&=\ln(3)+\ln\left( 1+\left( h+\frac{1}{3}h^{2} \right) \right) \\
&=\ln(3)+\left( h+\frac{1}{3}h^{2} \right)-\frac{1}{2}\left( h+\frac{1}{3}h^{2} \right)^{2}+o(h^{2}) \\
&=\ln(3)+h+\frac{1}{3}h^{2}-\frac{1}{2}h^{2}+o(h^{2}) \\
g(h)&=\ln(3)+h-\frac{1}{6} h^{2}+o(h^{2}) \\
\end{align}
$$
D'où le $DL_{2}(1)$ de $f$ :
$$
f(x)=\ln(3)+(h-1)-\frac{1}{6}(h-1)^{2}+o((h-1)^{2})
$$
Donc $DL_{1}(1)$ de $f$ : $f(x)=h+\ln(3)-1+o((h-1))$. D'où la tangente d'équation $y=x+\ln(3)-1$ en $1$.
Et :
$$
f(x)-(x+\ln(3)-1)=-\frac{1}{6}(h-1)^{2}+o((h-1)^{2})\sim -\frac{1}{6}(h-1)^{2}\leq 0
$$
Donc $f$ est au-dessous de sa tangente en $1$.


#### Remarques


