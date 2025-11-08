---
anki_linked: 0
raisonnements:
  - disjonction_de_cas
  - absurde
outils:
  - trigo
kh_n:
  - "4"
display_title: arctan(x)+arctan(1/x)
---
# Calcul de $\arctan(x)+\arctan\left( \frac{1}{x} \right)$

> [!objectif]
>$$
> \forall x \in \mathbb{R}^*,\arctan(x)+\arctan\left( \frac{1}{x} \right)=\begin{cases}
> \frac{\pi}{2} &\text{si }x>0 \\
> -\frac{\pi}{2} &\text{si }x<0
> \end{cases}
> $$
### Démonstration

Soit $x \in \mathbb{R}^*$.
On pose $a=\arctan(x)\in \left] -\frac{\pi}{2}, \frac{\pi}{2} \right[$ et $b=\arctan\left( \frac{1}{x} \right)\in \left] -\frac{\pi}{2}, \frac{\pi}{2} \right[$, donc $a+b \in]-\pi,\pi[$ 

Par l'absurde, on suppose que $a+b \not\equiv \frac{\pi}{2}\pmod \pi$.
Donc $a+b\in \mathbb{R}\setminus\left\{ \frac{\pi}{2}+2k\pi\mid k\in \mathbb{Z} \right\}$, donc $\tan(a+b)$ est défini.
Or $1-\tan(a)\tan(b)=1-\frac{x}{x}=0$ est le dénominateur de $\tan(a+b)$, donc $\tan(a+b)$ n'est pas défini, ce qui est absurde.

Donc $a+b \equiv \frac{\pi}{2}\pmod \pi$
Or $a+b \in]-\pi,\pi[$, donc $a+b \in \left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$.

***Si $x>0$*** :
Alors $a\in\left] 0, \frac{\pi}{2} \right[$ et $b\in \left] 0, \frac{\pi}{2} \right[$
Donc $a+b \in\,]0,\pi[ \,\cap\left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$.
On en déduit que : $a+b=\frac{\pi}{2}$

***Si $x<0$*** :
Alors $a\in\left] - \frac{\pi}{2}, 0 \right[$ et $b\in \left] - \frac{\pi}{2}, 0\right[$
Donc $a+b \in\,]-\pi,0[\,\cap\left\{ -\frac{\pi}{2}, \frac{\pi}{2} \right\}$.
On en déduit que : $a+b=-\frac{\pi}{2}$

Donc :
$$
\forall x \in \mathbb{R}^*,\arctan(x)+\arctan\left( \frac{1}{x} \right)=
\begin{cases}
\frac{\pi}{2} &\text{si }x>0 \\
-\frac{\pi}{2} &\text{si }x<0
\end{cases}
$$
#### Remarques


