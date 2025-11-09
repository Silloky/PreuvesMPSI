---
anki_linked: 0
raisonnements:
  - analyse_synthese
  - double_inclusion
outils:
kh_n:
  - "5"
display_title: Racines n-ièmes de l'unité
---
# Racines $n$-ièmes de l'unité

> [!objectif]
> Soit $n\in \mathbb{N}^*$. L'équation $z^n=1$ d'inconnue $z$ complexe a pour ensemble de solutions :
> $$
\left\{ e^{i \frac{2k\pi}{n}} \mid k\in [\![0,n-1]\!] \right\}
$$
### Démonstration

Soit $n\in \mathbb{N}^*$.

***Analyse*** :
Soit $z$ une solution.

*Pour le module*
On a $z^n=1$, donc $|z^n|=1$, donc $|z|^n=1$
Or $|z|\in \mathbb{R}_{+}$ donc $|z|=1$.
*Pour l'argument*
Il existe $t\in \mathbb{R}$ tel que $z=e^{it}$. Ainsi, $(e^{it})^n=1$, donc $e^{int}=e^{i0}$.
Donc $nt \equiv 0\pod{2\pi}$, autrement dit il existe $k\in \mathbb{Z}$ tel que $nt=0+2k\pi$, donc $t=\frac{2k\pi}{n}$

Donc $z\in \left\{ e^{i \frac{2k\pi}{n}} \mid k\in \mathbb{Z} \right\}$

***Synthèse*** :
Soit $k\in \mathbb{Z}$.
Or $\left( e^{i \frac{2k\pi}{n}} \right)^n=e^{i 2k\pi}=1$.
Donc $e^{i \frac{2k\pi}{n}}$ est bien solution.

On pose $A=\left\{ e^{i \frac{2k\pi}{n}} \mid k\in \mathbb{Z} \right\}$ et $B=\left\{ e^{i \frac{2k\pi}{n}} \mid k\in [\![0,n-1]\!] \right\}$.
Montrons $A=B$.

***Sens $\subset$*** :
Soit $z\in A$. Il existe $k\in \mathbb{Z}$ tel que $z=e^{i \frac{2k\pi}{n}}$.
On effectue la division euclidienne de $k$ par $n$ : 
Il existe $(q,r)\in \mathbb{Z}^{2}$ tel que $k=qn+r$ avec $r\in[\![0,n-1]\!]$.
Donc $z=e^{i \frac{2k\pi}{2}}=e^{i(2q\pi+2r\pi/n)}=e^{q\times 2i\pi}\times e^{i \frac{2r\pi}{n}}=e^{i \frac{2r\pi}{n}}$

***Sens $\supset$*** :
C'est évident, car $[\![0,n-1]\!]\subset \mathbb{Z}$

Donc $A=B$, et donc les racines $n$-ièmes de l'unité sont $\left\{ e^{i \frac{2k\pi}{n}} \mid k\in [\![0,n-1]\!] \right\}$

#### Remarques


