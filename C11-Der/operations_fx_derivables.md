---
anki_linked: 0
raisonnements:
outils:
  - limites
  - derivation
kh_n:
  - "10"
display_title: Opérations sur les fonctions dérivables
---
# Opérations sur les fonctions dérivables

> [!objectif]
> Soit $I$ un intervalle, $f:I\to \mathbb{R}$ et $g:I\to \mathbb{R}$ et $a \in I$ tels que $f$ et $g$ soient dérivables en $a$.
> 1. $f+g$ est dérivable en $a$ et $(f+g)'=f'+g'$
> 2. $f\times g$ est dérivable en $a$ et $(f\times g)=f'g+fg'$
> 3. Si $g$ ne s'annule pas sur $I$, $\frac{f}{g}$ est dérivable sur $I$ et $\left( \frac{f}{g} \right)'=\frac{f'g-fg'}{g^2}$
> 4. Si $g$ ne s'annule pas sur $I$, $\frac{1}{g}$ est dérivable sur $I$ et $\left( \frac{1}{g} \right)'=-\frac{g'}{g^2}$
> 5. Si $g: J\to \mathbb{R}$, $f(I)\subset J$ et $g$ dérivable en $f(a)$, alors $g\circ f$ est dérivable en $a$ et $(g\circ f)'=(g'\circ f)\times f'$

### Démonstration

##### 1. Somme

Pour tout $x \in I\setminus \{ a \}$ :$$
\frac{(f+g)(a)-(f+g)(x)}{x-a}=\underbrace{ \frac{f(x)-f(a)}{x-a} }_{ \xrightarrow[x\to a^\neq]{} f'(a)}+\underbrace{ \frac{g(x)-g(a)}{x-a} }_{ \xrightarrow[x\to a^\neq]{}g'(a) }\xrightarrow[x\to a^\neq]{}f'(a)+g'(a)
$$Donc $f+g$ est dérivable en $a$ et $(f+g)'=f'+g'$.
##### 2. Produit

Pour tout $x \in I\setminus \{ a \}$ :$$
\begin{align}
\frac{(fg)(a)-(fg)(x)}{x-a}&=\frac{g(x)(f(x)-f(a))+f(a)(g(x)-g(a))}{x-a} \\
&=\underbrace{ \left( \frac{f(x)-f(a)}{x-a} \right)}_{ \xrightarrow[x\to a^\neq]{} f'(a)}\underbrace{ g(x) }_{ \xrightarrow[x\to a^\neq]{}g(a) }  +   \underbrace{ \left( \frac{g(x)-g(a)}{x-a}  \right)}_{ \xrightarrow[x\to a^\neq]{}g'(a) }f(a) \\
\frac{(fg)(a)-(fg)(x)}{x-a}&\xrightarrow[x\to a^\neq]{}f'(a)g(a)+f(a)g'(a)
\end{align}
$$Donc $f\times g$ est dérivable en $a$ et $(f\times g)'=f'g+fg'$.
##### 3. Quotient

On suppose que $g(a)\neq 0$.
Par continuité, $g$ est non-nulle au voisinage de $a$, donc il existe $\eta>0$ tel que $\forall x \in I,|x-a|\leq \eta\implies g(x)\neq 0$.

Pour tout $x \in I\cap[a-\eta,a+\eta]\setminus \{ a \}$ :
$$
\begin{align}
\frac{\frac{f(x)}{g(x)}-\frac{f(a)}{g(a)}}{x-a}&=\frac{g(x)f(x)-f(x)g(x)}{g(x)g(a)(x-a)} \\
&=\frac{g(x)(f(x)-f(a))-f(a)(g(x)-g(a))}{g(x)g(a)(x-a)} \\
&=\underbrace{ \frac{1}{g(x)} }_{ \xrightarrow[x\to a^\neq]{} \frac{1}{g(a)} }\times \frac{1}{g(a)}\times \left( g(a) \underbrace{ \frac{f(x)-f(a)}{x-a} }_{ \xrightarrow[x\to a^\neq]{}f'(a) } -f(a) \underbrace{ \frac{g(x)-g(a)}{x-a} }_{ \xrightarrow[x\to a^\neq]{}g'(a) }\right)  \\
\frac{\frac{f(x)}{g(x)}-\frac{f(a)}{g(a)}}{x-a}&\xrightarrow[x\to a^\neq]{} \frac{f'(a)g(a)-f(a)g'(a)}{g(a)^2}
\end{align}
$$
Donc $\frac{f}{g}$ est dérivable en $a$ et $\left( \frac{f}{g} \right)'= \frac{f'g-fg'}{g^2}$
##### 4. Inverse

C'est un cas particulier du quotient avec $f:x\mapsto 1$.
D'où le résultat : $\frac{1}{g}$ est dérivable en $a$ et $\left( \frac{1}{g} \right)'=-\frac{g'}{g^2}$

##### 5. Composition

$g$ est dérivable en $f(a)$ donc il existe une fonction $\varepsilon:J\to \mathbb{R}$ telle que $\varepsilon(y)\xrightarrow[y\to f(a)]{}0$ et $\forall y \in J,g(y)=g(f(a))+g'(f(a))(y-f(a))+\varepsilon(x)(y-f(a))$

Pour tout $x \in I$, $g(f(x))=g(f(a))+g'(f(a))(f(x)-f(a))+\varepsilon(f(x))(f(x)-f(a))$.
Et donc, pour tout $x \in I\setminus \{ a \}$ :
$$
\begin{align}
\frac{g(f(x)-g(f(a)))}{x-a}&=g'(f(a))\underbrace{ \left( \frac{f(x)-f(a)}{x-a} \right) }_{ \xrightarrow[x\to a^\neq]{}f'(a) }+\underbrace{ \varepsilon(f(x)) }_{ \xrightarrow[x\to a^\neq]{}0 }\left( \frac{f(x)-f(a)}{x-a} \right) \\
\frac{g(f(x)-g(f(a)))}{x-a}&\xrightarrow[x\to a^\neq ]{}g'(f(a))\times f'(a)
\end{align}
$$
Donc $(g\circ f)$ est dérivable en $a$ et $(g\circ f)'=(g'\circ f)\times f'$

#### Remarques


