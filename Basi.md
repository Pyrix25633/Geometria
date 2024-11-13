$V$ spazio vettoriale finitamente generato
Un insieme di vettori $B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}\subset V$ è una base di $V$ se è un insieme di generatori di $V$ linearmente indipendente

$\forall \underline{v}\in V$ si scrive in modo unico come combinazione lineare di $B$
Dimostrazione:
$$\begin{flalign}\underline{v}=\sum_{i=1}^{n} \lambda_{i}\underline{v}_{i}=\sum_{i=1}^{n} \mu_{i}\underline{v}_{i}\implies \underline{0}=\underline{v}-\underline{v}=\sum_{i=1}^{n} (\lambda_{i}-\mu_{i})\underline{v}_{i}\implies\lambda_{i}=\mu_{i}\;\;\;\forall i\in \{ 1,\dots,n \} &&\end{flalign}$$perché $B$ è linearmente indipendente

$\{ \underline{v}_{1},\dots,\underline{v}_{k} \}\subset \mathbb{R}^{n}$ è una base di $\mathbb{R}^{n}\iff k=n$ e $\mathrm{rg}(\begin{bmatrix}\begin{array}{c|c|c}\underline{v}_{1}&\dots&\underline{v}_{k}\end{array}\end{bmatrix})=n$
