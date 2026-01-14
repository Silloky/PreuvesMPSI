---
anki_linked: 0
raisonnements:
outils:
  - polynome
  - sommes
kh_n:
display_title: Puissance n-ième de l'indéterminée
---
# Puissance $n$-ième de l'indéterminée

> [!objectif]
> On pose $X=(0,1,0,0,0,\dots)$ l'indéterminée de polynômes de $\mathbb{K}[X]$.
> Alors :
>$$
> \forall n\in \mathbb{N},X^n=(\delta_{n,k})_{k\in \mathbb{N}}=(0,\dots,\underbrace{ 1 }_{ \text{en position $n$} },0,0,0,\dots)
> $$
### Démonstration

Pour tout $n\in \mathbb{N}$, on pose $H_{n}:X^n=(\delta_{n,k})_{k\in \mathbb{N}}$

***Initialisation*** :
En $0$ : $X^0=(1,0,0,\dots)=(\delta_{0,k})_{k\in \mathbb{N}}$
D'où $H_{0}$.

***Hérédité*** :
Soit $n\in \mathbb{N}$. On suppose $H_{n}$. 
$X^n$ est une suite qui s'annule à partir d'un certain rang, donc $X^n$ est un polynôme.
Soit $k\in \mathbb{N}$.
$$
\begin{align}
[X^{n+1}]_{k}&=[X^n\times X]_{k} \\
&=\sum_{k'=0}^k[X^n]_{k'}[X]_{k-k'} \\
&=\sum_{k'=0}^k\delta_{n,k'}\underbrace{ \delta_{1,k-k'} }_{ \neq 0\text{ si }k'=k-1 } \\
&=\delta_{n,k-1}\delta_{1,1} \\
&=\delta_{n,k-1} \\
[X^{n+1}]_{k}&=\delta_{n+1,k}
\end{align}
$$
D'où $H_{n+1}$

D'où le résultat.

#### Remarques


