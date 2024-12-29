$V$ spazio vettoriale, $f:V\to V$ endomorfismo
# Endomorfismo diagonalizzabile
$A,B\in M_{n}(\mathbb{R})$ sono dette simili $\iff \exists C\in M_{n}(\mathbb{R}):A=C^{-1}BC$
$f$ è detto diagonalizzabile $\iff \exists B$ base di $V:M_{B}^{B}(f)$ è diagonale

$f:V\to V$ diagonalizzabile, $B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}$ base di $V:M_{B}^{B}(f)$ è diagonale
$$\begin{flalign}M_{B}^{B}(f)=\begin{bmatrix}
\lambda_{1} & \dots & 0 \\
\dots & &\dots \\
0 & \dots & \lambda_{n}
\end{bmatrix} \implies f(\underline{b}_{i})=\lambda_{i}\underline{b}_{i} &&\end{flalign}$$
# Autovalori e autovettori
$\underline{v}\in V,\underline{v}\neq \underline{0}$ è detto autovettore se $\exists\lambda \in \mathbb{R}:f(\underline{v})=\lambda \underline{v}$
$\lambda \in \mathbb{R}$ è detto autovalore se $\exists \underline{v}\in V,\underline{v}\neq \underline{0}:f(\underline{v})=\lambda \underline{v}$
Lo spettro di $f$ è l'insieme degli autovalori di $f$
$\lambda \in \mathbb{R}$ autovalore, l'autospazio relativo a $\lambda$ è $E(\lambda):=\{ \underline{v}\in V,\underline{v}\neq \underline{0}:f(\underline{v})=\lambda \underline{v} \}$

$\lambda_{1},\dots,\lambda_{k}\in \mathbb{R}$ autovalori distinti di $f$
$\underline{v}_{1},\dots \underline{v}_{k}\in V:f(\underline{v})=\lambda \underline{v}\implies \{ \underline{v}_{1},\dots,\underline{v}_{k} \}$ è linearmente indipendente
Dimostrazione:
- Caso base: $k=1$, $\{ \underline{v}_{1} \}$ è linearmente indipendente
- Caso induttivo:
  $\mu_{1}\underline{v}_{1}+{\dots}+\mu_{k}\underline{v}_{k}=\underline{0}$, $f(\underline{0})=\underline{0}$
  $f(\mu_{1}\underline{v}_{1}+{\dots}+\mu_{k}\underline{v}_{k})=\underline{0}$
  $\mu_{1}\lambda_{1}\underline{v}_{1}+{\dots}+\mu_{k}\lambda_{k}\underline{v}_{k}=\underline{0}$
  Inoltre $\lambda_{k}(\mu_{1}\underline{v}_{1}+{\dots}+\mu_{k}\underline{v}_{k})=\lambda_{k}\underline{0}=\underline{0}$
  $\implies\mu_{1}\lambda_{1}\underline{v}_{1}+{\dots}+\mu_{k}\lambda_{k}\underline{v}_{k}-\lambda_{k}(\mu_{1}\underline{v}_{1}+{\dots}+\mu_{k}\underline{v}_{k})=$
  $=\mu_{1}(\lambda_{1}-\lambda_{k})\underline{v}_{1}+{\dots}+\mu_{k-1}(\lambda_{k-1}-\lambda_{k})\underline{v}_{k-1}+\mu_{k}(\lambda_{k}-\lambda_{k})\underline{v}_{k}=\underline{0}$
  Supponendo $\{ \underline{v}_{1},\dots,\underline{v}_{k-1} \}$ linearmente indipendente
  $$\begin{flalign}\begin{cases}\mu_{1}(\lambda_{1}-\lambda_{k})=0 \\\dots \\\mu_{k-1}(\lambda_{k-1}-\lambda_{k})=0\end{cases}\implies \begin{cases}\mu_{1}=0 \\\dots \\\mu_{k-1}=0\end{cases}&&\end{flalign}$$
  $\implies\mu_{k}\underline{v}_{k}=\underline{0}$ e per definizione $\underline{v}_{k}\neq \underline{0}\implies \mu_{k}=0$

# Come trovare gli autovalori
$B$ base di $V$, $A=M_{B}^{B}(f)$
$\lambda$ è un autovalore di $f\iff \exists \underline{x}\in V:f(\underline{x})=\lambda \underline{x}\iff A\underline{x}=\lambda \underline{x}=\lambda I\underline{x}$
$\iff(A-\lambda I)\underline{x}=\underline{0}\iff$ il sistema lineare omogeneo ammette soluzioni non banali $\mathrm{\det}(A-\lambda I)=0$
<div class="page-break" style="page-break-before: always;"></div>

### Polinomio caratteristico
Il polinomio caratteristico di $f$ è il polinomio nella variabile $\lambda$
$\chi_{f}(\lambda)=\det(A-\lambda I)$ 
Il polinomio caratteristico non dipende dalla scelta della base

$f$ è diagonalizzabile $\iff \exists$ una base di $V$ formata da autovettori di $f$
Dimostrazione: $f$ è diagonalizzabile $\iff \exists B$ base di $V:M_{B}^{B}(f)$ è diagonale, in particolare, se $B=\{ \underline{b}_{1},\dots,\underline{b}_{n} \}$ e $n=\mathrm{dim}(V)$, si ha $f(\underline{b}_{i})=\lambda_{i}\underline{b}_{i}$
$\iff \chi_{f}(\lambda)=\det(A-\lambda I)=(\lambda_{1}-\lambda)\cdot{\dots}\cdot(\lambda_{k}-\lambda)$
Le soluzioni del polinomio caratteristico sono $\lambda_{1},\dots,\lambda_{n}$, ossia gli autovalori
Siccome $f(\underline{b}_{i})=\lambda \underline{b}_{i}\implies \underline{b}_{i}$ sono gli autovettori

# Come determinare gli autovettori
$\lambda_{i}$ autovalore di $f$, $\mathrm{E}(\lambda_{i})=\{ \underline{x}\in V:f(\underline{x})=\lambda_{i} \underline{x} \}$
$f(\underline{x})=\lambda_{i}\underline{x}\iff f(\underline{x})-\lambda_{i}Id(\underline{x})=\underline{0}\iff(f-\lambda_{i} Id)(\underline{x})=\underline{0}$ $\iff(A-\lambda_{i}I)\underline{x}=\underline{0}$
$\mathrm{E}(\lambda_{i})=\mathrm{Ker}(f-\lambda_{i}Id)=\{ \underline{x}:(A-\lambda_{i}I)\underline{x}=\underline{0} \}$

# Molteplicità algebrica e geometrica
$\lambda_{0}\in \mathbb{R}$ autovalore di $f$
La molteplicità algebrica di $\lambda_{0}$, $\mathrm{a(\lambda_{0})}$, è la molteplicità di $\lambda_{0}$ come radice di $\chi_{f}(\lambda)$
La molteplicità geometrica di $\lambda_{0}$, $\mathrm{g}(\lambda_{0})$, è la dimensione dell'autospazio $\mathrm{E}(\lambda_{0})$
$1\leq \mathrm{g}(\lambda_{0})\leq \mathrm{a}(\lambda_{0})$

# Criterio di diagonalizzabilità
$f$ è diagonalizzabile $\iff \chi_{f}(\lambda)$ è totalmente riducibile e $\mathrm{a}(\lambda_{i})=\mathrm{g}(\lambda_{i})\;\;\forall\lambda_{i}$
Dimostrazione: "$\impliedby$"
$$\begin{flalign}\sum_{i=1}^{r} \mathrm{g}(\lambda_{i})=\sum_{i=1}^{r} \mathrm{a}(\lambda_{i})=\mathrm{dim}(V) &&\end{flalign}$$
$g_{i}=\mathrm{g}(\lambda_{i})$
$A_{i}=\{ \underline{a}_{i1},\dots,\underline{a}_{ig_{i}} \}$ base di $\mathrm{E}(\lambda_{i})$
$(\mu_{11}\underline{a}_{11}+{\dots}+\mu_{1g_{1}}\underline{a}_{1g_{1}})+{\dots}+(\mu_{r1}\underline{a}_{r1}+{\dots}+\mu_{rg_{r}}\underline{a}_{rg_{r}})=\underline{w}_{1}+{\dots}+\underline{w}_{r}=0$ e $\{ \underline{w}_{1},\dots,\underline{w}_{r} \}$ è linearmente indipendente $\implies \underline{w}_{1},\dots,\underline{w}_{r}=0\implies \mu_{i1},\dots,\mu_{ig_{i}}=0\;\;\forall i\in \{ 0,\dots,r \}$

$f$ endomorfismo, $\mathrm{dim}(V)=n$, $\lambda_{1},\dots,\lambda_{k}$ autovalori di $f$ ($k\leq n$)
$f$ è diagonalizzabile $\iff$
$$\begin{flalign}\sum_{i=1}^{r} \mathrm{g}(\lambda_{i})=\sum_{i=1}^{r} \mathrm{a}(\lambda_{i})=\mathrm{dim}(V) &&\end{flalign}$$

$f$ endomorfismo tale che $\chi_{f}(\lambda)$ è totalmente riducibile e $\mathrm{a}(\lambda_{i})=1 \implies f$ è diagonalizzabile

$f$ endomorfismo diagonalizzabile, $A\in M_{n}(\mathbb{R})$ matrice rappresentativa $\implies$
$$\begin{flalign}\det(A)=\prod_{i=0}^{n} \lambda_{i} &&\end{flalign}$$
<div class="page-break" style="page-break-before: always;"></div>

# Matrici diagonalizzanti e cambiamenti di base
$f$ diagonalizzabile, $A$ base di $V$, $M=M_{A}^{A}(f)$, $\underline{v}_{1},\dots,\underline{v}_{n}$ autovettori
$B=\{ \underline{v}_{1},\dots,\underline{v}_{n} \}$ è una base di $V$
$M_{B}^{A}=[\begin{array}{c|c|c}\underline{v}_{1} & \dots & \underline{v}_{n}\end{array}]$
$$\begin{flalign}M_{B}^{B}(f)=M_{A}^{B}M_{A}^{A}(f)M_{B}^{A}=\begin{bmatrix}
\lambda_{1} & \dots & 0 \\
\dots & & \dots \\
0 & \dots & \lambda_{n}
\end{bmatrix} &&\end{flalign}$$

# Endomorfismi simmetrici
$V$ spazio vettoriale euclideo, $f$ endomorfismo è simmetrico se $f(\underline{v})\cdot \underline{w}=\underline{v}\cdot f(\underline{w})\;\;\forall \underline{v},\underline{w}\in V$

$f$ endomorfismo simmetrico, $\lambda_{1},\lambda_{2}$ autovalori distinti
$\underline{v}_{1}\in \mathrm{E}(\lambda_{1}),\underline{v}_{2}\in \mathrm{E}(\lambda_{2})\implies \underline{v}_{1}\cdot \underline{v}_{2}=\underline{0}$
Dimostrazione: $f(\underline{v}_{1})\cdot \underline{v}_{2}=\underline{v}_{1}\cdot f(\underline{v}_{2})\iff\lambda_{1}\underline{v}_{1}\cdot\underline{v}_{2}=\underline{v}_{1}\cdot\lambda_{2}\underline{v}_{2}\iff$ $(\lambda_{1}-\lambda_{2})(\underline{v}_{1}\cdot \underline{v}_{2})=0\implies \underline{v}_{1}\cdot \underline{v}_{2}=0$

# Teorema spettrale
$V$ spazio vettoriale euclideo, $f$ endomorfismo simmetrico $\implies \exists$ una base di $V$ fatta di autovettori di $f$ e $f$ è diagonalizzabile

$f$ è simmetrico $\iff M_{B}^{B}(f)$ è simmetrica, $B$ base ortonormale di $V$