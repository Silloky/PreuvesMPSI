---
anki_linked: 0
raisonnements:
outils:
  - limites
kh_n:
  - "4"
display_title: Croissances comparées
---
# Croissances comparées

> [!objectif]
> 1. $\frac{e^x}{x}\xrightarrow[x\to +\infty]{}+\infty$
> 2. $\forall n\in \mathbb{N}^*, \frac{e^x}{x^n} \xrightarrow[x\to + \infty]{}+\infty$
> 3. $\frac{(e^x)^{a}}{x^b} \xrightarrow[n \to \infty]{} + \infty$
> 4. $\forall a\geq 1, \forall p >1, \frac{n^a}{p^n} \xrightarrow[x \to + \infty]{} 0$
> 5. $\forall a \geq 1, \forall q \in]-1,1[, n^aq^n \xrightarrow[n\to +\infty]{}0$
> 6. $\forall p > 1, \frac{p^n}{n!} \xrightarrow[x\to +\infty]{}0$ 
### Démonstration

##### 1. $\frac{e^x}{x}\xrightarrow[x\to +\infty]{}+\infty$
On a $\forall x>0, e^{x/2}\geq \frac{x}{2}$, donc $e^x\geq \frac{x^{2}}{4}$, et donc $\frac{e^{ x }}{x}\geq \frac{x}{4}\xrightarrow[x\to +\infty]{}+\infty$
##### 2. $\forall n\in \mathbb{N}^*, \frac{e^x}{x^n} \xrightarrow[x\to + \infty]{}+\infty$
Soit $n\geq 1$.
On a $\frac{x}{n}\xrightarrow[x \to +\infty]{}+\infty$ et $\frac{e^x}{x}\xrightarrow[x\to +\infty]{}+\infty$
Donc en composant : $\frac{e^{ x/n }}{x/n}\xrightarrow[x\to +\infty]{}+\infty$, donc en passant à la puissance $n$ :
$\frac{e^x}{x^n}\times n^n \xrightarrow[x \to +\infty]{}+\infty$
Or $n^n$ est fixé, d'où $\frac{e^x}{x^n} \xrightarrow[x\to + \infty]{}+\infty$
##### 3. $\frac{(e^x)^{a}}{x^b} \xrightarrow[n \to \infty]{} + \infty$
Soit $a\in]0,1[$ et $b\geq 1$.
On a $\forall x>0, \frac{(e^x)^a}{x^b}=\frac{e^{ax}}{e^{b\ln(x)}}=e^{ax-b\ln(x)}$
Or $ax-b\ln(x)=x(a-b\frac{\ln(x)}{x})\xrightarrow[x\to +\infty]{}+\infty$
D'où $\frac{(e^x)^{a}}{x^b} \xrightarrow[n \to \infty]{} + \infty$
##### 4. $\forall a\geq 1, \forall p >1, \frac{n^a}{p^n} \xrightarrow[x \to + \infty]{} 0$
Soit $a\geq 1$ et $p>1$.
Pour tout $n\geq 1$, on a $\frac{n^a}{p^n}=n^a\times p^{-n}=e^{a\ln(n)-n\ln(p)}$.
Or $a\ln(n)-n\ln(p)=n\left(a \frac{\ln(n)}{n}-\ln(p)\right)\xrightarrow[x\to +\infty]{}-\infty$
Par composition, $e^{a\ln(n)-n\ln(p)}=\frac{n^a}{p^n} \xrightarrow[x \to + \infty]{} 0$
##### 5. $\forall a \geq 1, \forall q \in]-1,1[, n^aq^n \xrightarrow[n\to +\infty]{}0$
Soit $a\ge 1$. Soit $q\in]-1,1[$.
***Si $q=0$*** : $q^n=0$, d'où le résultat
***Si $q\neq 0$*** :
$\forall n\geq 1, |n^aq^n|=n^a|q|^n=e^{a\ln(n)+n\ln(|q|)}$.
Or $a\ln(n)+n\ln(|q|)=n\left(a \frac{\ln(n)}{n}+\ln(|q|)\right)\xrightarrow[n \to +\infty]{}-\infty$
Par composition, $e^{a\ln(n)+n\ln(|q|)}=n^aq^n\xrightarrow[n \to +\infty]{}0$
##### 6. $\forall p > 1, \frac{p^n}{n!} \xrightarrow[x\to +\infty]{}0$
[[lim_0_(p&n div n!)|Voir document à part]]

#### Remarques


