---
anki_linked: 0
raisonnements:
outils:
  - suites
  - sous-suites
kh_n:
  - "8"
display_title: Convergence de la suites des moyennes de Cesáro
---
# Convergence de la suite des moyennes de Cesáro

> [!objectif]
> Soit $(u_{n})$ une suite et $l\in \mathbb{R}$. Pour tout $n\in \mathbb{N}^*$, on pose $m_{n}=\frac{1}{n}\sum_{k=1}^{n}u_{k}$.
> Alors :
> 1. Si $u_{n}\to +\infty$ alors $m_{n}\to +\infty$
> 2. Si $u_{n}\to l$ alors $m_{n}\to +\infty$
### Démonstration

##### 1. $(u_{n})$ est divergente

Soit $M\in \mathbb{R}$. On suppose que $M>0$.
On a $u_{n}\to +\infty$, donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall k\geq N_{1},u_{k}\geq 2M \in \mathbb{R}$.
On pose $C=\sum_{k=1}^{N_{1}}u_{k} -2MN_{1}$. $\frac{C}{n}\to 0$, donc il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, \frac{C}{n}\leq | \frac{C}{n}-0 |\leq |M|>0$, donc $\frac{C}{n}\leq |M|$, donc $\frac{C}{n}\geq -M$

Soit $n\geq \max(N_{1},N_{2})$.
$$
\begin{align}
m_{n}&=\frac{1}{n}\sum_{k=1}^{n}u_{k} \\
&=\frac{1}{n}\sum_{k=1}^{N_{1}}u_{k}+\frac{1}{n}\sum_{k=N_{1}+1}^{n}u_{k_{1}} \\
&\geq\frac{1}{n}\sum _{k=1}^{N_{1}}u_{k} + \frac{1}{n}\sum_{k=1}^{n}2M \\
&=\frac{1}{n}\sum_{k=1}^{N_{1}}u_{k}+ \frac{n-N_{1}}{n}2M  \\
&= 2M+\frac{1}{n}\left( \sum_{k=1}^{N_{1}} u_{k} -2MN_{1}\right) \\
&=2M+\frac{C}{n} \\
&\geq2M-M \\
&= M
\end{align}
$$
Ainsi, on a démontré que :
$$
\forall M>0,\exists N\in \mathbb{N}, \forall n\geq N,u_{n}\geq M
$$
Donc c'est aussi vrai à fortiori pour tout $M\leq 0$.
Donc $m_{n}\to +\infty$
##### 2. $(u_{n})$ converge vers $l$

Soit $\varepsilon>0$.
On a $u_{n}\to l$ donc il existe $N_{1}\in \mathbb{N}$ tel que $\forall k\geq N_{1}, |u_{n}-l|\leq \frac{\varepsilon}{2}>0$.
Et il existe $N_{2}\in \mathbb{N}$ tel que $\forall n\geq N_{2}, \frac{1}{n} \left| \sum_{k=1}^{N_{1}} (u_{k}-l)\right|\leq \frac{\varepsilon}{2}$.

Soit $n\geq \max(N_{1},N_{2})$.
$$
\begin{align}
|m_{n}-l|&=\left| \frac{1}{n} \left(\sum_{k=1}^n u_{k} -  nl\right) \right|  \\
&=\frac{1}{n}\left| \sum_{k=1}^{n}(u_{k}-l) \right| \\
&= \frac{1}{n}\left| \sum_{k=1}^{N_{1}}(u_{k}-l) + \sum_{k=N_{1}+1}^{n}(u_{k}-l)\right|  \\
&\leq \frac{1}{n}\left| \sum_{k=1}^{N_{1}}(u_{k}-l) \right| +\frac{1}{n}\left| \sum _{k=N_{1}+1}^{n}(u_{k}-l) \right|  \\
&\leq \frac{\varepsilon}{2}+ \frac{1}{n}\sum_{k=N_{1}+1}^{n}|u_{k}-l| \\
&\leq \frac{\varepsilon}{2}+ \frac{n-N_{1}}{n} \frac{\varepsilon}{2} \\
&= \frac{\varepsilon}{2}+\left( 1- \frac{N_{1}}{n} \right)  \frac{\varepsilon}{2} \\
& \leq \frac{\varepsilon}{2}+\frac{\varepsilon}{2} \\ \\
|m_{n}-l| &\leq \varepsilon
\end{align}
$$
Donc $m_{n}\to l$.

#### Remarques


