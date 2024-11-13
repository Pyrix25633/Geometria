$V$ spazio vettoriale

# Insieme di vettori linearmente dipendenti
$\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente dipendente se $\exists\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$ non tutti nulli tali che
$$\begin{flalign}\sum_{i=1}^{k} \lambda_{i}\underline{v}_{i}=\underline{0} &&\end{flalign}$$
Se $\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente dipendente e se $k\geq2\implies \exists i\in \{ 1,\dots,k \}:\mathrm{Span}(\underline{v}_{1},\dots,\underline{v}_{k})=\mathrm{Span}(\underline{v}_{1},\dots,\check{\underline{v}_{i}},\dots,\underline{v}_{k})$
Dimostrazione:
per ipotesi $\exists\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$ non tutti nulli tali che $\lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{k}\underline{v}_{k}=\underline{0}$,
sia $i\in \{ 1,\dots,k \}:\lambda_{i}\neq{0}\implies \underline{v}_{i}=-\frac{\lambda_{1}}{\lambda_{i}}\underline{v}_{1}-{\dots}-\frac{\lambda_{i-1}}{\lambda_{i}}\underline{v}_{i-1}-{\dots}-\frac{\lambda_{i+1}}{\lambda_{i}}\underline{v}_{i+1}-{\dots}-\frac{\lambda_{k}}{\lambda_{i}}\underline{v}_{k}$

# Insieme di vettori linearmente indipendenti
Se invece
$$\begin{flalign}\sum_{i=1}^{k} \lambda_{i}\underline{v}_{i}=\underline{0}\implies\lambda_{i}=0\;\;\;\forall i\in\{ 1,\dots,k \} &&\end{flalign}$$
allora $\{ \underline{v}_{1},\dots,\underline{v}_{k} \} \subset V$ è linearmente indipendente
