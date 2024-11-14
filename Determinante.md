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
