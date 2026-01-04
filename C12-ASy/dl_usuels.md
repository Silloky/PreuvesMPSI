---
anki_linked: 0
raisonnements:
outils:
  - dl
kh_n:
  - "11"
display_title: Développement limités usuels
---
# Développement limités usuels

> [!objectif]
> 1. $\displaystyle \exp(x)\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n \frac{x^k}{k!} \right)+o(x^n)$
> 2. $\displaystyle \cos(x)\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n (-1)^k\frac{x^{2k}}{(2k)!} \right)+o(x^{2n+1})$
> 3. $\displaystyle \sin(x)\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n (-1)^{k}\frac{x^{2k+1}}{(2k+1)!} \right)+o(x^{2n+2})$
> 4. $\displaystyle \frac{1}{1-x} \underset{ 0 }{ = }\left( \sum\limits_{k=0}^n x^k \right)+o(x^{n})$
> 5. $\displaystyle \frac{1}{1+x} \underset{ 0 }{ = }\left( \sum\limits_{k=0}^n (-1)^k\frac{x^k}{k}\right)+o(x^{n})$
> 6. $\displaystyle \ln(1+x)\underset{ 0 }{ = }\left( \sum\limits_{k=1}^n (-1)^{k}\frac{x^{k}}{k} \right)+o(x^{n})$
> 7. $\displaystyle \tan(x)\underset{ 0 }{ = }x+ \frac{x^{3}}{3}+\frac{2x^5}{15}+\frac{17x^7}{315}+\frac{62x^9}{2835} +o(x^{10})$
> 8. $\displaystyle \cosh(x)\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n \frac{x^{2k}}{(2k)!} \right)+o(x^{2n+1})$
> 9. $\displaystyle \sinh(x)\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n \frac{x^{2k+1}}{(2k+1)!} \right)+o(x^{2n+2})$
> 10. $\displaystyle (1+x)^\alpha\underset{ 0 }{ = }1+\left[\sum\limits_{k=1}^n \frac{\prod\limits_{i=0}^{k-1}(\alpha-i)}{k!}x^k \right]+o(x^{n})$
### Démonstration

##### 1. $\exp$

Pour tout $k \in[\![0,n]\!]$, $\exp$ est $k$-fois dérivable et :
$$
\forall x \in \mathbb{R}, \exp ^{(k)}(x)=x^k\exp(x)
$$
Donc en $0$ : $\exp ^{(k)}(0)=1\times 1=1$.
Ainsi d'après la formule de Taylor-Young :
$$
\exp(x)\underset{ 0 }{ = } \left( \sum\limits_{k=0}^n \frac{\exp ^{k}(0)}{k!}(x-0)^k \right) +o(x^n) \underset{ 0 }{ = }\left( \sum\limits_{k=0}^n \frac{x^k}{k!} \right)+o(x^n)
$$
##### 2. $\cos$

$\cos$ est de classe $\mathcal{C}^\infty$ sur $\mathbb{R}$, et ses dérivées successives vérifient, pour tout $k \in \mathbb{N}$ : 
* si le rang est pair : $\cos ^{(2k)}(0)=(-1)^k$ (elle se comporte comme $\cos$ et $-\cos$)
* si le rang est impair : $\cos ^{(2k+1)}(0)=0$ (elle se comporte comme $\sin$ et $-\sin$)

Donc d'après la formule de Taylor-Young à l'ordre $2n$ :
$$
\begin{align}
\cos(x)&\underset{ 0 }{ = } \left( \sum\limits_{k=0}^{2n} \frac{\cos ^{(k)}(0)}{k!} x^k\right)+o(x^{2n}) \\
&\underset{ 0 }{ = } \left( \sum\limits_{\substack{k=0\\k\text{ pair}}}^{2n} \frac{\cos ^{(k)}(0)}{k!}x^k \right)+ \left( \sum\limits_{\substack{k=0\\k\text{ impair}}}^{2n} \frac{\cos ^{(k)}(0)}{k!}x^k \right)+o(x^{2n}) \\
&\underset{ 0 }{ = } \left( \sum\limits_{k=0}^{n} \frac{\cos ^{(2k)}(0)}{(2k)!}x^{2k} \right)+\left( \sum\limits_{k=0}^n \frac{\cos ^{(2k+1)}(0)}{(2k+1)!} x^{2k+1} \right)+o(x^{2n})   \\
&\underset{ 0 }{ = }\left( \sum\limits_{k=0}^n (-1)^k \frac{x^{2k}}{(2k)!} \right) +\left( \sum\limits_{0}^n 0 \right)+o(x^{2n}) \\
\cos(x)&\underset{ 0 }{ = } \left( \sum\limits_{k=0}^n(-1)^k \frac{x^{2k}}{(2k)!} \right) +o(x^{2n+1})
\end{align}
$$

##### 3. $\sin$
Comme $\cos$, mais c'est inversé, donc les dérivées de rang pair sont nulles.
Ainsi :
$$
\sin(x)\underset{ 0 }{ = }\left( \sum_{k=0}^n 0 \right) +\left( \sum_{k=0}^n (-1)^k \frac{x^{2k+1}}{(2k+1)!} \right)+o(x^{2n}) \\
$$

##### 4. Inverse de $1-x$

La somme des $n+1$ premiers termes d'une suite géométrique de raison $x$ vaut $\sum_{k=0}^nx^n= \frac{1-x^{n+1}}{1-x}$.
D'où au voisinage de $0$ :
$$
\begin{align}
\frac{1}{1-x}&\underset{ 0 }{ = }\sum_{k=0}^nx^k- \frac{x^{n+1}}{1-x} \\
&\underset{ 0 }{ = }\sum_{k=0}^nx^n+x^k \frac{-x}{1-x} \\
\frac{1}{1-x} &\underset{ 0 }{ = }\sum_{k=0}^nx^k+o(x^n)
\end{align}
$$
Car $\frac{-x}{1-x}\xrightarrow[x\to 0]{}0$, donc $x^n \times \frac{-x}{1-x}\underset{ 0 }{ = }o(x^n)$.

##### 5. Inverse de $1+x$

Par changement de variable dans le DL de $\frac{1}{1-x}$, on obtient :
$$
\begin{align}
\frac{1}{1+x}&=\frac{1}{1-(-x)} \\
&\underset{ 0 }{ = } \sum_{k=0}^n(-x)^k+(-1)^no(x^n) \\
\frac{1}{1+x} &\underset{ 0 }{ = }\sum_{k=0}^n(-1)^kx^k+o(x^n)
\end{align}
$$
##### 6. $\ln(1+x)$

On utilise le $DL_{n}(0)$ de $\frac{1}{1+x}$.
D'après le théorème de l'intégration des DL :
$$
\ln(1+x)=\int\limits^x_{0} \frac{1}{1+x}\mathrm{d}\underset{ 0 }{ = }\ln(1)+\sum_{k=1}^n(-1)^{k+1} \frac{x^k}{k}+o(x^n)
$$
##### 7. $\tan$

Voir la [[dl_tan|page]] à part.

##### 8. $\cosh$

On sait que $\cosh(x)= \frac{e^x+e^{-x}}{2}$.
Or à l'ordre $2n+1$ :
* $\displaystyle e^x\underset{ 0 }{ = }\sum_{k=0}^{2n+1} \frac{x^k}{k!}+o(x^{2n+1})=\sum_{\substack{k=0 \\ k\text{ pair}}}^{2n+1} \frac{x^k}{k!}+\sum_{\substack{k=0 \\ k\text{ impair}}}^{2n+1} \frac{x^k}{k!}+o(x^{2n+1})$
* $\displaystyle e^{-x}\underset{ 0 }{=}\sum_{k=0}^{2n+1}(-1)^k \frac{x^k}{k!}+o(x^{2n+1})=\sum_{\substack{k=0 \\ k\text{ pair}}}^{2n+1} \frac{x^k}{k!}-\sum_{\substack{k=0 \\ k\text{ impair}}}^{2n+1} \frac{x^k}{k!}+o(x^{2n+1})$

D'où par somme :
$$
\cosh(x)\underset{ 0 }{ = } \frac{1}{2}\times 2\sum_{\substack{k=0 \\ k\text{ pair}}}^{2n+1} \frac{x^k}{k!}+o(x^{2n+1})\underset{ 0 }{ = }\sum_{\substack{k=0 \\ k\text{ pair}}}^{2n} \frac{x^k}{k!}+o(x^{2n+1})\underset{ 0 }{ = }\sum_{k=0}^n \frac{x^{2k}}{(2k)!}+o(x^{2n+1})
$$
##### 9. $\sinh$

On réutilise les DL de $e^x$ et $e^{-x}$ précédents, et on prend la différence :
$$
\sinh(x)\underset{ 0 }{ = } \frac{1}{2}\times 2\sum_{\substack{k=0 \\ k\text{ impair}}}^{2n+1} \frac{x^k}{k!}+o(x^{2n+1})\underset{ 0 }{ = }\sum_{0}^n \frac{x^{2k+1}}{(2k+1)!}+o(x^{2x+1})
$$
##### 10. $(1+x)^\alpha$

$f(x)=(1+x)^\alpha$ est de classe $\mathcal{C}^\infty$ et $\mathbb{R}$ pour tout $x \in \mathbb{R}$, la dérivée $k$-ième vaut :
$$
f^{(k)}(x)=\prod_{i=0}^{k-1}(\alpha-i)\times(1+x)^{\alpha-k}
$$
Donc en $0$ : $\displaystyle f^{(k)}(0)=\prod_{i=0}^{k-1}(\alpha-i)$
Ainsi d'après la formule de Taylor-Young :
$$
\begin{align}
f(x)&\underset{ 0 }{ = }\sum_{k=0}^n \frac{f^{(k)}(0)}{k!}x^k +o(x^n) \\
f(x)&\underset{ 0 }{ = }\sum_{k=0}^n \frac{x^k}{k!} \prod_{i=0}^k(\alpha-i)+o(x^n)
\end{align}
$$

#### Remarques


