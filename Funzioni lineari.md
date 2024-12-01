$V,V'$ spazi vettoriali reali
Una funzione lineare $f:V\to V'$ è una funzione tale che:
- $f(\underline{v}+\underline{w})=f(\underline{v})+f(\underline{w})\;\;\;\forall \underline{v},\underline{w}\in V$
- $f(\lambda \underline{v})=\lambda f(\underline{v})\;\;\;\forall \underline{v}\in V,\;\lambda \in \mathbb{R}$
Alternativamente $f(\lambda \underline{v}+\mu \underline{w})=\lambda f(\underline{v})+\mu f(\underline{w})\;\;\;\forall \underline{v},\underline{w}\in V,\;\lambda,\mu \in \mathbb{R}$
$V$ è detto dominio di $f$
$V'$ è detto codominio di $f$
Se $f$ è biunivoca è detta isomorfismo di spazi vettoriali
Se $V=V'$, $f$ è detta endomorfismo

$f(\underline{0}_{V})=\underline{0}_{V'}$
Dimostrazione: $f(\underline{v}+(-\underline{v}))=f(\underline{v})+f(-\underline{v})=f(\underline{v})-f(\underline{v})$

# Nucleo
$f:V\to V'$ funzione lineare
$\mathrm{Ker}(f)=\{ \underline{v}\in V:f(\underline{v})=\underline{0}_{V'} \}\subset V$ è detto nucleo di $f$

$\mathrm{Ker(f)}\subset V$ è un sottospazio vettoriale
Dimostrazione: $f(\lambda \underline{v}+\mu \underline{w})=\lambda f(\underline{v})+\mu f(\underline{w})=\lambda \underline{0}_{V'}+\mu \underline{0}_{V'}=\underline{0}_{V'} \implies \lambda \underline{v}+\mu \underline{w}\in \mathrm{Ker}(f)\;\;\;\forall \underline{v},\underline{w}\in V,\;\lambda,\mu \in \mathbb{R}$
Le seguenti condizioni sono equivalenti:
- $\mathrm{Ker}(f)=\{ \underline{0}_{V} \}$
- $f$ è iniettiva
- Se $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}\subset V$ è linearmente indipendente $\implies \{ f(\underline{v}_{1}),\dots,f(\underline{v}_{m}) \}\subset V'$ è linearmente indipendente

# Immagine
$f:V\to V'$ funzione lineare
$\mathrm{Im}(f)=\{ \underline{v}'\in V':\exists \underline{v}\in V:f(\underline{v})=\underline{v}' \}\subset V'$

$\mathrm{Im}(f)\subset V'$ è un sottospazio vettoriale
Dimostrazione:
$\underline{v}',\underline{w}'\in \mathrm{Im}(f)\implies \exists \underline{v},\underline{w}\in V:\underline{v}'=f(\underline{v}),\underline{w}'=f(\underline{w})$
$\lambda \underline{v}'+\mu \underline{w}'=\lambda f(\underline{v})+\mu f(\underline{w})=f(\lambda \underline{v}+\mu \underline{w})\implies\lambda \underline{v}'+\mu \underline{w}'\in \mathrm{Im}(f)$

$f:V\to V'$ lineare e suriettiva $\implies V'=\mathrm{Im}(f)$

Le seguenti condizioni sono equivalenti:
- $\mathrm{Im}(f)=V'$
- $f$ è suriettiva
- Se $\{ \underline{v}_{1},\dots,\underline{v}_{n} \}$ è un sistema di generatori di $V$ e $f:V\to V'$ funzione lineare $\implies \{ f(\underline{v}_{1}),\dots,f(\underline{v}_{n}) \}$ è un sistema di generatori di $\mathrm{Im}(f)$

# Funzioni lineari definite da matrici
$V=\mathbb{R}^{n},\;V'=\mathbb{R}^{m},\;A\in M_{m\times n}(\mathbb{R}),\;T_{A}:V\to V',\;T_{A}(\underline{x})=A\underline{x}$
$V''=\mathbb{R}^{p},\;B\in M_{p\times m}(\mathbb{R}),\;T_{B}:V'\to V'',\;T_{B}(\underline{y})=B\underline{y}$
$T_{B}\circ T_{A}:V\to V'',\;(T_{B}\circ T_{A})(\underline{x})=(BA)\underline{x}$ composizione è anch'essa una funzione lineare associata alla matrice $BA\in M_{p\times n}(\mathbb{R})$
$T_{B}\circ T_{A}=T_{BA}$
Se $A\in M_{n}(\mathbb{R})$ è invertibile $\implies T_{A^{-1}}\circ T_{A}=T_{A^{-1}A}=T_{I_{n}}=Id_{\mathbb{R}^{n}}:\mathbb{R}^{n}\to \mathbb{R}^{n},\;Id_{\mathbb{R}^{n}}(\underline{x})=\underline{x}$

# Teorema nullità più rango
$V$ spazio vettoriale finitamente generato, $V'$ spazio vettoriale, $f:V\to V'$ funzione lineare
$\mathrm{dim}(V)=\mathrm{dim}(\mathrm{Ker}(f))+\mathrm{dim}(\mathrm{Im}(f))$

$A\in M_{m\times n}(\mathbb{R}),\;T_{A}:\mathbb{R}^{n}\to \mathbb{R}^{m},\;T_{A}(\underline{x})=A\underline{x}$
$\mathrm{Ker}(T_{A})=\mathrm{N}(A),\;\mathrm{Im}(T_{A})=\mathrm{C}(A)$
Applicando il teorema: $n=\mathrm{dim}(\mathrm{Ker}(T_{A}))+\mathrm{dim}(\mathrm{Im}(T_{A}))=\mathrm{null}(A)+\mathrm{rg}(A)$

Se $f:V\to V'$ è inoltre un isomorfismo $\implies \mathrm{dim}(V)=\mathrm{dim}(V')$
Dimostrazione: $\mathrm{dim}(V)=\mathrm{dim}(\mathrm{Ker}(f))+\mathrm{dim}(\mathrm{Im}(f))=0+\mathrm{dim}(V')$ (iniettiva + suriettiva)

# Matrici rappresentative
$V$ spazio vettoriale reale, $B=\{ \underline{b}_{1},..,\underline{b}_{n} \}$ base di $V$
Per definire una funzione (o mappa o applicazione) lineare $f:V\to V'$ è sufficiente definire le immagini degli elementi della base $f(\underline{b}_{i})=\underline{c}_{i}\in V'$
$\underline{v}\in V$ è definito come combinazione lineare degli elementi di $B$
$$\begin{flalign}\underline{v}=\sum_{i=1}^{n} v_{i}\underline{b}_{i},\;v_{i}\in R \implies f(\underline{v})=f\left( \sum_{i=1}^{n} v_{i}\underline{b}_{i} \right)=\sum_{i=1}^{n} v_{i}f(\underline{b}_{i})=\sum_{i=1}^{n} v_{i}\underline{c}_{i}\in V' &&\end{flalign}$$

$V$ spazio vettoriale, $\mathrm{dim}(V)=n$, $B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}$ base di $V$
$\underline{c}_{1},\dots,\underline{c}_{n}\in V'\;\;\forall i\in \{ 1,\dots,n \}\;\exists!f:V\to V':f(\underline{b}_{i})=\underline{c}_{i}$

# Costruzione della matrice rappresentativa
$A=\{ \underline{a}_{1},\dots,\underline{a}_{n} \}$ base di $V$, $B=\{ \underline{b}_{1},\dots,\underline{b}_{m} \}$ base di $V'$, $f:V\to V'$
$$\begin{flalign}f(\underline{a}_{1})=\sum_{i=1}^{m} \alpha_{i1}\underline{b}_{i} &&\end{flalign}$$
$\dots$
$$\begin{flalign}f(\underline{a}_{n})=\sum_{i=1}^{m} \alpha_{in}\underline{b}_{i} &&\end{flalign}$$
$M_{A}^{B}(f)=[\alpha_{ij}]\in M_{m\times n}(\mathbb{R})$ è detta matrice rappresentativa di $f$ rispetto alle basi $A$ e $B$

# Coordinate e matrici rappresentative
$V,V'$ spazi vettoriali reali con basi $A,B$, $f:V\to V'$ funzione lineare, $M=M_{A}^{B}(f)$
$$\begin{flalign}\mathrm{dim}(V)=n\;\;T_{A}:V\to \mathbb{R}^{n}\;\;T_{A}(\underline{v})=(v_{1},\dots,v_{n})\;\;\underline{v}=\sum_{i=1}^{n} v_{i}\underline{a}_{i} &&\end{flalign}$$
$$\begin{flalign}\mathrm{dim}(V')=m\;\;T_{B}:V\to \mathbb{R}^{m}\;\;T_{B}(\underline{w})=(w_{1},\dots,w_{n})\;\;\underline{w}=\sum_{i=1}^{n} w_{i}\underline{b}_{i} &&\end{flalign}$$
$T_{M}:\mathbb{R}^{n}\to \mathbb{R}^{m}\;\;T_{M}(\underline{x})=M\underline{x}$

<iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJWIl0sWzIsMCwiViciXSxbMCwyLCJcXG1hdGhiYntSfV57bn0iXSxbMiwyLCJcXG1hdGhiYntSfV57bX0iXSxbMCwyLCJUX3tBfSJdLFswLDEsImYiLDJdLFsxLDMsIlRfe0J9IiwyXSxbMiwzLCJUX3tNfSJdXQ==&embed" width="300" height="300" style="border-radius: 8px; border: none;"></iframe>

Il diagramma è "commutativo", $T_{M}=T_{B}\circ f\circ T_{A}^{-1}$, $f=T_{B}^{-1}\circ T_{M}\circ T_{A}$

$\mathrm{Ker}(T_{M})=T_{A}\mathrm{Ker(f)}\;\;\mathrm{Ker}(f)=T_{A}^{-1}\mathrm{Ker}(T_{M})$
$\mathrm{Im}(T_{M})=T_{B}\mathrm{Im}(f)\;\;\mathrm{Im}(f)=T_{B}^{-1}\mathrm{Im}(T_{M})$
# Cambiamento di base
$V=V'$, $A,B$ due basi distinte di $V$, $f=Id_{V}:V\to V,\;f(\underline{v})=\underline{v}$
$M_{A}^{B}:=M_{A}^{B}(Id_{V})$ è detta matrice di transizione dalla base $A$ alla base $B$
$$\begin{flalign}\underline{v}=\sum_{i=1}^{n} x_{i}\underline{a}_{i}=\sum_{i=1}^{n} y_{i}\underline{b}_{i}\implies M_{A}^{B}\cdot \begin{bmatrix}
x_{1} \\
\dots \\
x_{n}
\end{bmatrix}=\begin{bmatrix}
y_{1} \\
\dots \\
y_{n}
\end{bmatrix} &&\end{flalign}$$
$M_{A}^{B}=(M_{B}^{A})^{-1}$
