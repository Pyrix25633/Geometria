$V$ spazio vettoriale finitamente generato
Un insieme di vettori $B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}\subset V$ è una base di $V$ se è un insieme di generatori di $V$ linearmente indipendenti

$\forall \underline{v}\in V$ si scrive in modo unico come combinazione lineare degli elementi di $B$
Dimostrazione:
$$\begin{flalign}\underline{v}=\sum_{i=1}^{n} \lambda_{i}\underline{v}_{i}=\sum_{i=1}^{n} \mu_{i}\underline{v}_{i}\implies \underline{0}=\underline{v}-\underline{v}=\sum_{i=1}^{n} (\lambda_{i}-\mu_{i})\underline{v}_{i}\implies\lambda_{i}=\mu_{i}\;\;\;\forall i\in \{ 1,\dots,n \} &&\end{flalign}$$perché $B$ è linearmente indipendente

$\{ \underline{v}_{1},\dots,\underline{v}_{k} \}\subset \mathbb{R}^{n}$ è una base di $\mathbb{R}^{n}\iff k=n$ e $\mathrm{rg}(\begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots&\underline{v}_{k}\end{array}\end{bmatrix})=n$

# Estrazione di una base da un sistema di generatori
$\{ \underline{v}_{1},\dots,\underline{v}_{m} \}\subset \mathbb{R}^{n}$ sistema di generatori ($m\geq n$)
 1) $A=\begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots|\underline{v}_{m}\end{array}\end{bmatrix}$
 2) Si riduce $A$ in forma a scalini: i vettori corrispondenti alle colonne contenenti pivot formano una base

# Completamento di un sistema linearmente indipendente ad una base
$B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}\subset \mathbb{R}^{n}$ base di $V$, $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}\subset \mathbb{R}^{n}$ sistema linearmente indipendente ($m<n$)
$\implies \exists$ una base di $V$ formata da $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}$ e altri $n-m$ elementi di $B$
1) $[A|B]=\begin{bmatrix}\begin{array}{c|c|c|c|c|c}\underline{v}_{1}&\dots&\underline{v}_{m}&\underline{b}_{1}&\dots&\underline{b}_{n}\end{array}\end{bmatrix}$
2) Si riduce $[A|B]$ a scalini, si ottiene
	- $m$ pivot sulle prime $m$ colonne
	- la posizione dei rimanenti $n-m$ pivot individua gli $n-m$ elementi di $B$ da aggiungere a $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}$ per ottenere una base di $\mathbb{R}^{n}$

# Spazio delle righe e delle colonne
$A=\begin{bmatrix}\begin{array}{c|c|c}\underline{c}_{1}&\dots&\underline{c}_{n}\end{array}\end{bmatrix}=\begin{bmatrix}\underline{r}_{1}\\\hline\dots\\\hline \underline{r}_{m}\end{bmatrix}\in M_{m\times n}(\mathbb{R}),\;\underline{c}_{i}\in \mathbb{R}^{m},\;\underline{r}_{j}\in \mathbb{R}^{n}$
$\mathrm{C}(A)=\mathrm{Span}(\underline{c}_{1},\dots,\underline{c}_{n})\subset \mathbb{R}^{m}$ è lo spazio delle colonne di $A$
$\mathrm{R}(A)=\mathrm{Span}(\underline{r}_{1},\dots,\underline{r}_{m})\subset \mathbb{R}^{n}$ è lo spazio delle righe di $A$
$\mathrm{dim}(\mathrm{C}(A))=\mathrm{dim}(\mathrm{R}(A))=\mathrm{rg}(A)$
Dimostrazione:
