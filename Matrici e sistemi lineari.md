### Spazio delle ennuple
$\mathbb{R}^{n}=\{ (a_{1},\dots,a_{n}):a_{i}\in \mathbb{R},\;i=1,\dots,n \}$ è lo spazio delle ennuple di numeri reali
Operazioni:
- Somma: $\underline{a}+  \underline{b}=(a_{1},\dots,a_{n})+(b_{1},\dots,b_{n})=(a_{1}+b_{1},\dots,a_{n}+b_{n})$
- Prodotto per uno scalare: $\lambda  \cdot\underline{a}=\lambda\cdot(a_{1},\dots,a_{n})=(\lambda\cdot a_{1},\dots,\lambda\cdot a_{n})$

# Sistema lineare
Un sistema di equazioni lineari di $m$ equazioni in $n$ incognite è
$$\begin{flalign}\begin{cases}
a_{11}x_{1}+{\dots}+a_{1n}x_{n}=b_{1} \\
\dots \\
a_{m1}x_{m}+{\dots}+a_{mn}x_{n}=b_{m}
\end{cases} &&\end{flalign}$$
Una soluzione del sistema lineare è una ennupla $(t_{1},\dots,t_{n})$ soluzione di tutte le equazioni
Se esistono soluzioni il sistema è detto compatibile, altrimenti è detto incompatibile
Se $b_{1}={\dots}=b_{m}=0$ il sistema è detto omogeneo

# Matrice
Una matrice di ordine $m\times n$ a coefficienti reali è una tabella
$$\begin{flalign}
A=
\begin{bmatrix}
a_{11} & \dots & a_{1n} \\
\dots \\
a_{m_{1}} & \dots & a_{mn}
\end{bmatrix}
=[a_{ij}] \in M_{m\times n}(\mathbb{R})
&&\end{flalign}$$
Se $m=n$ la matrice è quadrata e gli elementi $\{ a_{11},\dots,a_{nn} \}$ formano la diagonale principale di $A$
$A^{T}=[a_{ji}]$ è detta matrice trasposta di $A$
$A=A^{T} \implies A$ è simmetrica
$\underline{0}_{m\times n}=[0]_{ij}$ è detta matrice nulla di ordine $m\times n$
Una matrice di ordine $m\times1$ è detta matrice colonna o vettore colonna
$$\begin{flalign}A=\begin{bmatrix}
a_{11} \\
\dots \\
a_{m1}
\end{bmatrix} &&\end{flalign}$$
Una matrice di ordine $1\times n$ è detta matrice riga o vettore riga
$$\begin{flalign}A=\begin{bmatrix}
a_{11} & \dots & a_{1n}
\end{bmatrix} &&\end{flalign}$$
La matrice opposta di $A=[a_{ij}]$ è $-A=[-a_{ij}]$

### Somma
$A,B\in M_{m\times n}(\mathbb{R}),\;A=[a_{ij}],\;B=[b_{ij}]$
$A+B=[a_{ij}+b_{ij}]$
Proprietà:
- Commutativa: $A+B=B+A$
- Associativa: $(A+B)+C=A+(B+C)$
- Elemento neutro: $A+\underline{0}=A$
- Elemento opposto: $A+(-A)=\underline{0}$
<div class="page-break" style="page-break-before: always;"></div>

### Prodotto per uno scalare
$A \in M_{m\times n}(\mathbb{R}),\;\lambda \in \mathbb{R}$
$\lambda\cdot A=[\lambda\cdot a_{ij}]$
Proprietà:
- Associativa: $\lambda\cdot(\mu\cdot A)=(\lambda\cdot \mu)\cdot A$
- Elemento neutro: $1\cdot A=A$
- Distributiva: $(\lambda+\mu)\cdot A=\lambda A+\mu A$
- Distributiva: $\lambda\cdot(A+B)=\lambda A+\lambda B$

### Combinazione lineare
$A,B\in M_{m\times n}(\mathbb{R}),\;\lambda,\mu \in \mathbb{R}$
$\lambda A+\mu B\in M_{m\times n}(\mathbb{R})$ è detta combinazione lineare di $A$ e $B$ a coefficienti $\lambda$ e $\mu$

# Prodotto di matrici
Una matrice $A$ è detta conformabile a sinistra con $B \iff$
$A=[a_{ij}]\in M_{m\times n}(\mathbb{R}),\;B=[b_{jk}]\in M_{n\times p}(\mathbb{R})$
e $A\cdot B=C=[c_{ik}]\in M_{m\times p}(\mathbb{R})$ dove
$$\begin{flalign}c_{ik}=\sum_{j=1}^{n} a_{ij}\cdot b_{jk} &&\end{flalign}$$

### Identità
$I_{m}=[\delta_{ij}]$ è la matrice quadrata di ordine $m\times m$ dove
$$\begin{flalign}\delta_{ij}:=\begin{cases}
1,\;i=j \\
0,\;i\neq j
\end{cases} &&\end{flalign}$$

# Matrice associata al sistema lineare
Ad un sistema lineare si possono associare tre matrici:
- Matrice dei coefficienti: $A\in M_{m\times n}(\mathbb{R})$
- Matrice dei termini noti: $\underline{b}\in M_{m\times 1}(\mathbb{R})$
- Matrice completa: $(A|\underline{b})\in M_{m\times n+1}(\mathbb{R})$
$$\begin{flalign}
(A|\underline{b})=\left[\begin{array}{ccc|c}
a_{11} & \dots & a_{1n} & b_{1} \\
\dots \\
a_{m_{1}} & \dots & a_{mn} & b_{m}
\end{array}\right]
&&\end{flalign}$$

# Operazioni elementari
$\lambda\neq 0,\;\mu\neq 0$
- Scambio di due righe $R_{i}$ e $R_{j}$: $S_{ij}$
- Prodotto di una riga $R_{i}$ per uno scalare $\lambda$: $D_{j}(\lambda)$
- Somma di una riga $R_{i}$ con un'altra $R_{j}$ moltiplicata per uno scalare $\mu$: $E_{ij}(\mu)$
<div class="page-break" style="page-break-before: always;"></div>

# Matrice a scalini
Una matrice è detta a scalini se $\forall R_{i},R_{i+1}$ coppia di righe consecutive si verifica una delle seguenti condizioni:
- $R_{i}$ e $R_{i+1}$ sono entrambe non nulle e il numero di zeri che precedono il primo numero non nullo di $R_{i}$ è inferiore rispetto a quello di $R_{i+1}$
- $R_{i+1}$ è nulla

# Algoritmo di Gauss-Jordan
- Si cerca la prima colonna che contiene un numero, il primo dall'alto si chiama $p_{1}$
- Si scambiano le righe in modo da portare $p_{1}$ sulla prima riga
- Si utilizzano le operazioni elementari del tipo $E_{i_{1}}(\mu)$ finché tutti i termini sottostanti a $p_{1}$ diventano nulli
- Si itera l'algoritmo sulla matrice ottenuta escludendo la prima riga

# Rango
Il rango di una matrice $A$, $\mathrm{rg}(A)$, è il numero di pivot di una sua forma a scalini

# Matrice ridotta per righe
Una matrice è ridotta per righe se:
- è a scalini
- e ogni pivot è $1$ ed è l'unico elemento non nullo della propria colonna

# Riduzione all'indietro
Si parte da una matrice a scalini
- Per ogni pivot $p_{k}$ si esegue l'operazione $D_{k}\left( \frac{1}{k} \right)$ in modo che $p_{k}$ diventi $1$
- Si riducono a $0$ tutti i termini della colonna di $p_{k}$ tramite operazioni del tipo $E_{ik}(\mu)$

# Teorema di Rouchè-Capelli
Dato un sistema lineare in $n$ incognite, tale sistema è compatibile $\iff \mathrm{rg}(A)=\mathrm{rg}(A|\underline{b})$
Se tale sistema è compatibile allora:
- $\mathrm{rg}(A)=n \implies$ ha un'unica soluzione
- $\mathrm{rg}(A)<n \implies$ ha infinite soluzioni

# Soluzioni di un sistema lineare
$A\in M_{m\times n}(\mathbb{R})$
$A\underline{x}=\underline{0}$ sistema lineare omogeneo, $\underline{v},\underline{w}$ vettori colonna soluzioni del sistema (ovvero $A\underline{v}=\underline{0},\;\underline{A}w=\underline{0}$), $\lambda,\mu \in \mathbb{R}$
Anche la combinazione lineare $\lambda \underline{v}+\mu \underline{w}$ è soluzione del sistema poiché $A(\lambda \underline{v}+\mu \underline{w})=\lambda A\underline{v}+\mu A\underline{w}=\lambda\underline{0}+\mu\underline{0}=\underline{0}$

### Nucleo
Il nucleo di $A$, $\mathrm{N}(A)$, è l'insieme delle soluzioni del sistema omogeneo $A\underline{x}=\underline{0}$

### Nullità
La nullità di $A$, $\mathrm{null}(A)$, è il numero delle colonne di $\mathrm{rref}(A)$ che non contengono pivot, ossia il numero di variabili libere da cui dipendono le soluzioni
$\mathrm{null}(A)+\mathrm{rg}(A)=n$

### Insieme delle soluzioni
$A\underline{x}=\underline{b}$ sistema lineare compatibile:
- $\underline{b}=\underline{0} \implies$ l'insieme delle soluzioni è chiuso rispetto alla somma e al prodotto per uno scalare
- $\underline{b}\neq \underline{0} \implies$ se $\underline{x}_{0}$ è una soluzione, allora tutte le soluzioni sono della forma $\underline{x}_{0}+\underline{v}$, con $\underline{v}$ soluzione del sistema lineare omogeneo $A\underline{x}=\underline{0}$, infatti $A(\underline{x}_{0}+\underline{v})=A\underline{x}_{0}+A\underline{v}=\underline{b}+\underline{0}=\underline{b}$

# Matrici delle operazioni elementari
Le operazioni elementari possono essere realizzate tramite la moltiplicazione a sinistra per delle matrici quadrate
$I_{m}\xrightarrow{S_{ij}}S_{ij}$
$I_{m}\xrightarrow{D_{i}(\lambda)}D_{i}(\lambda)$
$I_{m}\xrightarrow{E_{ij}(\mu)}E_{ij}(\mu)$
$A\in M_{m\times n}(\mathbb{R})$, $\mathrm{rref}(A)$ può essere ottenuta moltiplicando $A$ a sinistra per una opportuna matrice quadrata $P\in M_{m\times m}(\mathbb{R})$ ottenuta dal prodotto di matrici di operazioni elementari: $PA=\mathrm{rref(A)}$

# Matrice inversa
$A\in M_{n}(\mathbb{R})$, $\exists B\in M_{n}(\mathbb{R}):AB=BA=I_{n} \implies A$ è invertibile e $B$ è detta inversa di $A$ e si denota con $A^{-1}$

### Inversa dell'identità
$I_{n}^{-1}=I_{n}$

### Inverse delle matrici delle operazioni elementari
$S_{ij}^{-1}=S_{ji}=S_{ij}$
$D_{i}(\lambda)^{-1}=D_{i}(\lambda^{-1})$
$E_{ij}(\mu)^{-1}=E_{ij}(-\mu)$

### Inverso del prodotto
$(AB)^{-1}=A^{-1}B^{-1}$
Dimostrazione: $(AB)(AB)^{-1}=A(BB^{-1})A^{-1}=AI_{n}A^{-1}=I_{n}$

### Invertibilità di una matrice
$A\in M_{n}(\mathbb{R})$ è invertibile $\iff \mathrm{rg}(A)=n$
Dimostrazione:
$\mathrm{rg}(A)=\mathrm{rg}(\mathrm{rref}(A))$
$\exists P\in M_{n}(\mathbb{R}):\mathrm{rref}(A)=PA$
$A=P^{-1}\mathrm{rref}(A)$, $A$ è invertibile $\implies \mathrm{rref}(A)$ è invertibile e non può avere righe di zeri $\implies \mathrm{rg}(A)=n \implies \mathrm{rg}(\mathrm{rref}(A))=n \implies \mathrm{rref}(A)=I_{n}\implies PA=I_{n}\implies A=P^{-1}$

### Calcolo della matrice inversa
$A\in M_{n}(\mathbb{R})$
1) $B=(A\mid I_{n})\in M_{n\times2n}(\mathbb{R})$
2) $\mathrm{rref}(B)=(I_{n}\mid P)=(I_{n}\mid A^{-1})$
Dimostrazione:
$\mathrm{rref(B)}=PB=(PA\mid PI_{n})=(\mathrm{rref}(A)\mid P)=(I_{n}\mid A^{-1})$
<div class="page-break" style="page-break-before: always;"></div>

### Soluzioni di un sistema lineare tramite matrice inversa
$A\in M_{n}(\mathbb{R})$ invertibile, $A\underline{x}=\underline{b}$ sistema lineare
$\underline{x}=A^{-1}\underline{b}$
Dimostrazione:
$A^{-1}A\underline{x}=A^{-1}\underline{b} \iff I_{n}\underline{x}=A^{-1}\underline{b}\iff \underline{x}=A^{-1}\underline{b}$