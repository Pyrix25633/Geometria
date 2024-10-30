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