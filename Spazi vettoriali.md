# Spazio vettoriale
Uno spazio vettoriale è un'insieme $V$ (i cui elementi sono vettori) su cui sono definite due operazioni:
- Somma tra elementi
- Prodotto di un elemento per uno scalare
che soddisfano le seguenti proprietà:
$\forall \underline{v},\underline{w},\underline{u}\in V,\;\lambda,\mu \in \mathbb{R}$
- Commutativa: $\underline{v}+\underline{w}=\underline{w}+\underline{v}$
- Associativa: $\underline{v}+(\underline{w}+\underline{u})=(\underline{v}+\underline{w})+\underline{u}$
- Elemento neutro: $\exists \underline{0}\in V:\underline{v}+\underline{0}=\underline{v}$
- Elemento opposto: $\exists-\underline{v} \in V:\underline{v}+(-\underline{v})=\underline{0}$
- Associativa: $\lambda(\mu \underline{v})=(\lambda \mu)\underline{v}$
- Elemento neutro: $1\underline{v}=\underline{v}$
- Distributiva: $(\lambda+\mu)\underline{v}=\lambda \underline{v}+\mu \underline{v}$
- Distributiva: $\lambda(\underline{v}+\underline{w})=\lambda \underline{v}+\lambda \underline{w}$

# Combinazione lineare
Siano:
- $V$ spazio vettoriale
- $\underline{v}_{1},\dots,\underline{v}_{k}\in V$
- $\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$

Il vettore
$$\begin{flalign}\underline{v}=\sum_{i=1}^{k}\lambda_{i}\underline{v}_{i}=\lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{k}\underline{v}_{k}\in V  &&\end{flalign}$$
è detto combinazione lineare dei vettori $\underline{v}_{1},\dots,\underline{v}_{k}$ con coefficienti $\lambda_{1},\dots,\lambda_{k}$
La combinazione lineare può essere scritta in "forma matriciale":
per ogni ennupla $\underline{v}_{i}=(v_{i1},\dots,v_{in})$ si considera il vettore colonna
$$\begin{flalign}\underline{v}_{i}=\begin{bmatrix}
v_{i1} \\
\dots \\
v_{in}
\end{bmatrix} &&\end{flalign}$$
e si accostano i $k$ vettori a formare una matrice $A=\begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots&\underline{v}_{k}\end{array}\end{bmatrix}$,considerando il vettore colonna composto dagli scalari
$$\begin{flalign}\underline{\lambda}=\begin{bmatrix}
\lambda_{1} \\
\dots \\
\lambda_{k}
\end{bmatrix} &&\end{flalign}$$
si può scrivere
$$\begin{flalign}\underline{v}=\sum_{i=1}^{k}\lambda_{i}\underline{v}_{i}=A\underline{\lambda} &&\end{flalign}$$
<div class="page-break" style="page-break-before: always;"></div>

# Sottospazio vettoriale
$V$ spazio vettoriale reale
Un sottoinsieme non vuoto di $V$, $U\subset V$, è detto sottospazio vettoriale di $V$ se è chiuso rispetto alle due operazioni di $V$:
- $\forall \underline{u}_{1},\underline{u}_{2}\in U\;\;\;\underline{u}_{1}+\underline{u}_{2}\in U$
- $\forall \underline{u}\in U,\lambda \in \mathbb{R}\;\;\;\lambda \underline{u}\in U$
o equivalentemente $\forall \underline{u}_{1},\underline{u}_{2}\in U,\lambda_{1},\lambda_{2} \in \mathbb{R}\;\;\;\lambda_{1} \underline{u}_{1}+\lambda_{2} \underline{u}_{2}\in U$
Inoltre $\underline{0}\in U$, infatti $\forall \underline{u}\in U\;-1\cdot \underline{u}=-\underline{u}\in U \implies \underline{u}-\underline{u}\in U$
Se $U$ contiene almeno un vettore non nullo, allora $U$ contiene infiniti elementi

# Insieme di generatori
$V$ spazio vettoriale reale
Dati $\underline{v}_{1},\dots,\underline{v}_{k}\in V$, l'insieme di tutte le loro combinazioni lineari è detto sottospazio generato da $\underline{v}_{1},\dots,\underline{v}_{k}$
$\langle\underline{v}_{1},\dots,\underline{v}_{k}\rangle=\mathrm{Span}(\underline{v}_{1},\dots,\underline{v}_{k})=\{ \lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{k}\underline{v}_{k}:\lambda_{1},\dots,\lambda_{k}\in \mathbb{R} \}\subset V$
$V=\mathrm{Span}(\underline{v}_{1},\dots,\underline{v}_{k})\implies V$ è finitamente generato e $\{ \underline{v}_{1},\dots,\underline{v}_{k} \}$ è un insieme di generatori di $V$
$\{ \underline{v}_{1},\dots,\underline{v}_{k} \}\subset \mathbb{R}^{n}$ è un sistema di generatori di $\mathbb{R}^{n}\iff \mathrm{rg}(\begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots&\underline{v}_{k}\end{array}\end{bmatrix})=n\implies k\geq n$

# Sistemi lineari omogenei e sottospazi
L'insieme delle soluzioni del sistema lineare omogeneo $A\underline{x}=\underline{0}$ è un sottospazio di $\mathbb{R}^{n}$
Ogni sottospazio di $\mathbb{R}^{n}$ può essere realizzato come l'insieme delle soluzioni di un sistema lineare omogeneo opportuno
$\underline{x}\in \mathrm{Span}(\underline{v}_{1},\dots,\underline{v}_{k})\subset \mathbb{R}^{n}\iff \begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots&\underline{v}_{k}\end{array}\end{bmatrix}\underline{\lambda}=\underline{x}$ è compatibile

# Dipendenza-indipendenza lineare
$V$ spazio vettoriale reale

### Insieme di vettori linearmente dipendenti
$\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente dipendente se $\exists\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$ non tutti nulli tali che
$$\begin{flalign}\sum_{i=1}^{k} \lambda_{i}\underline{v}_{i}=\underline{0} &&\end{flalign}$$
Se $\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente dipendente e se $k\geq2\implies \exists i\in \{ 1,\dots,k \}:\mathrm{Span}(\underline{v}_{1},\dots,\underline{v}_{k})=\mathrm{Span}(\underline{v}_{1},\dots,\check{\underline{v}_{i}},\dots,\underline{v}_{k})$
Dimostrazione:
per ipotesi $\exists\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$ non tutti nulli tali che $\lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{k}\underline{v}_{k}=\underline{0}$,
sia $i\in \{ 1,\dots,k \}:\lambda_{i}\neq{0}\implies \underline{v}_{i}=-\frac{\lambda_{1}}{\lambda_{i}}\underline{v}_{1}-{\dots}-\frac{\lambda_{i-1}}{\lambda_{i}}\underline{v}_{i-1}-{\dots}-\frac{\lambda_{i+1}}{\lambda_{i}}\underline{v}_{i+1}-{\dots}-\frac{\lambda_{k}}{\lambda_{i}}\underline{v}_{k}$

### Insieme di vettori linearmente indipendenti
Se invece
$$\begin{flalign}\sum_{i=1}^{k} \lambda_{i}\underline{v}_{i}=\underline{0}\implies\lambda_{i}=0\;\;\;\forall i\in\{ 1,\dots,k \} &&\end{flalign}$$
allora $\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente indipendente
