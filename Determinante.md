$A\in M_{n}(\mathbb{R}),\;i,j\in \{ 1,\dots,n \}$
$A_{ij}\in M_{n-1}(\mathbb{R})$ è la matrice ottenuta da $A$ rimuovendo la $i$-esima riga e la $j$-esima colonna

Il determinante è una funzione $\det:M_{n}(\mathbb{R})\to \mathbb{R}$ definita come:
 - Se $n=1,\;A=[a_{11}]$, $\det(A)=a_{11}$
 - Se $n\geq2$, $$\begin{flalign}\det(A)=\sum_{i=1}^{n} (-1)^{i+1}\cdot a_{i1}\cdot \det(A_{i1}) &&\end{flalign}$$
 Se $A\in M_{n}(\mathbb{R})$ è triangolare superiore, ovvero
 $$\begin{flalign}A=\begin{bmatrix}
a_{11} & a_{12} & \dots & a_{1n}\\
0 & a_{22} & \dots & a_{2n}\\
\dots & \dots & \dots & \dots\\
0 & 0 & \dots & a_{nn}
\end{bmatrix} &&\end{flalign}$$
$\implies \det(A)=a_{11}\cdot a_{22}\cdot {\dots}\cdot a_{nn}$
Quindi $\det(I_{n})=1$

# Teorema di Laplace
$A\in M_{n}(\mathbb{R}),\;i,j\in \{ 0,\dots,n \}$
$$\begin{flalign}\det(A)=\sum_{i=1}^{n} (-1)^{i+j}\cdot a_{ij}\cdot \det(A_{ij})=\sum_{j=1}^{n}(-1)^{i+j}\cdot a_{ij}\cdot \det(A_{ij})  &&\end{flalign}$$

Se $A$ ha una riga o una colonna nulla $\implies \det(A) = 0$

$A=[a_{ij}]\in M_{n}(\mathbb{R}),\;A^{T}=[a_{ji}]\in M_{n}(\mathbb{R}) \implies \det(A)=\det(A^{T})$

# Teorema di Binet
$A,B\in M_{n}(\mathbb{R})\implies \det(A\cdot B)=\det(A)\cdot \det(B)$

Inoltre se $A$ è invertibile $\implies \det(A^{-1})=\frac{1}{\det(A)}$

# Determinante delle matrici delle operazioni elementari
$A,S_{ij},D_{i}(\lambda),E_{ij}(\mu)\in M_{n}(\mathbb{R})$
- $\det(S_{ij})=-1\implies \det(S_{ij}\cdot A)=-\det(A)$
- $\det(D_{i}(\lambda))=\lambda\implies \det(D_{i}(\lambda)\cdot A)=\lambda\cdot \det(A)$
- $\det(E_{ij}(\mu))=1\implies \det(E_{ij}(\mu)\cdot A)=\det(A)$
Si può quindi semplificare il calcolo del determinante riducendo a scalini una matrice e moltiplicando il suo determinante per il prodotto dei determinanti delle operazioni elementari utilizzate

# Determinante, rango e identità
$A\in M_{n}(\mathbb{R})$
Le seguenti condizioni sono equivalenti:
- $\det(A)=0$
- $rg(A)=n$
- $A$ è invertibile

# Determinante e matrice inversa
$A=[a_{ij}]\in M_{n}(\mathbb{R})$
Il cofattore dell'elemento $a_{ij}$ è lo scalare $a_{ij}'=(-1)^{i+j}\cdot \det(A_{ij})$ e la matrice dei cofattori di $A$ è $A'=[a_{ij}']$

Se $A$ è invertibile $\implies A^{-1}=\frac{1}{\det(A)}(A')^{T}$

# Determinante e vettori geometrici
### Prodotto vettoriale
$\underline{v}=v_{1}\underline{i}+v_{2}\underline{j}+v_{3}\underline{k},\;\underline{w}=w_{1}\underline{i}+w_{2}\underline{j}+w_{3}\underline{k}$
$\underline{v}\times \underline{w}=$"$\det\begin{bmatrix}\underline{i}&\underline{j}&\underline{k}\\v_{1}&v_{2}&v_{3}\\w_{1}&w_{2}&w_{3}\end{bmatrix}$"

### Prodotto misto
$\underline{v}\cdot(\underline{w}\times \underline{u})=\det \begin{bmatrix}v_{1}&v_{2}&v_{3}\\w_{1}&w_{2}&w_{3}\\u_{1}&u_{2}&u_{3}\end{bmatrix}$

# Determinante e geometria nello spazio
### Complanarità di due rette
$r$ e $s$ sono complanari $\iff \{ \underline{v},\underline{w},\overrightarrow{PQ} \}$ sono linearmente dipendenti $\iff \det \begin{bmatrix}\begin{array}{c|c|c}\underline{v}&\underline{w}&\overrightarrow{PQ}\end{array}\end{bmatrix}=0$

### Equazione cartesiana di un piano
$A,B,C$ punti non allineati
$\pi$ è luogo dei punti $Q$ tali che $\overrightarrow{AQ}$ è combinazione lineare di $\overrightarrow{AB}$ e $\overrightarrow{AC}$
$Q=(x,y,z)\in \pi \iff \{ \overrightarrow{AB},\overrightarrow{AC},\overrightarrow{AQ} \}$ sono linearmente dipendenti $\iff \det \begin{bmatrix}\begin{array}{c|c|c}\overrightarrow{AB}&\overrightarrow{AQ}&\overrightarrow{AQ}\end{array}\end{bmatrix}=0$
