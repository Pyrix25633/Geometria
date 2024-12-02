# Prodotto scalare
$V$ spazio vettoriale reale
Un prodotto scalare su $V$ è una funzione lineare che $\forall \underline{v},\underline{w}\in V$ associa $\underline{v}\cdot \underline{w}$ tale che:
- $\underline{v}\cdot \underline{w}=\underline{w}\cdot \underline{v}\;\;\;\forall \underline{v},\underline{w}\in V$
- $(\lambda \underline{v})\cdot \underline{w}=\lambda(\underline{v}\cdot \underline{w})\;\;\;\forall \underline{v},\underline{w}\in V,\;\lambda \in \mathbb{R}$
- $\underline{v}\cdot(\underline{w}+\underline{u})=\underline{v}\cdot \underline{w}+\underline{v}\cdot \underline{u}\;\;\;\forall \underline{v},\underline{w},\underline{u}\in V$
- $\underline{v}\cdot \underline{v}\geq0\;\;\;\forall \underline{v}\in V$ e $\underline{v}\cdot \underline{v}=0\iff \underline{v}=\underline{0}$
Uno spazio vettoriale reale dotato di prodotto scalare è detto spazio vettoriale euclideo

# Disuguaglianza di Cauchy-Schwartz
$V$ spazio vettoriale euclideo
$\underline{v},\underline{w}\in V\implies(\underline{v}\cdot \underline{w})^{2}\leq(\underline{v}\cdot \underline{v})(\underline{w}\cdot \underline{w})$

# Norma
$V$ spazio vettoriale euclideo
La norma di un vettore è $||\underline{v}||=\sqrt{\underline{v}\cdot \underline{v}}\in \mathbb{R}_{\geq0}$
Proprietà:
- $||\underline{v}||\geq0\;\;\;\forall \underline{v}\in V$ e $||\underline{v}||=0\iff \underline{v}=\underline{0}$
- $||\lambda \underline{v}||=|\lambda|||\underline{v}||\;\;\;\forall \underline{v}\in V,\;\lambda \in \mathbb{R}$
- $||\underline{v}+\underline{w}||\leq ||\underline{v}||+||\underline{w}||\;\;\;\forall \underline{v},\underline{w}\in V$

# Distanza
La distanza tra due vettori $\underline{v},\underline{w}\in V$ è $\mathrm{d}(\underline{v},\underline{w})=||\underline{v}-\underline{w}||$
Proprietà:
- $\mathrm{d}(\underline{v},\underline{w})\geq0$ e $\mathrm{d}(\underline{v},\underline{w})=0\iff \underline{v}=\underline{w}\;\;\;\forall \underline{v},\underline{w}\in V$
- $\mathrm{d}(\underline{v},\underline{w})=\mathrm{d}(\underline{w},\underline{v})\;\;\;\forall \underline{v},\underline{w}\in V$
- $\mathrm{d}(\underline{v},\underline{w})\leq \mathrm{d}(\underline{v},\underline{u})+\mathrm{d}(\underline{u},\underline{w})\;\;\;\forall \underline{v},\underline{w},\underline{u}\in V$

# Ortogonalità
$V$ spazio vettoriale euclideo, $\underline{v},\underline{w}\in V$ sono detti ortogonali se $\underline{v}\cdot \underline{w}=0$

Se $\underline{v}_{1},\dots,\underline{v}_{m}\neq0$ sono ortogonali a coppie, ovvero $\forall i\neq j\in \{ 1,\dots,m \}\;\;\underline{v}_{i}\cdot \underline{v}_{j}=0\implies \{ \underline{v}_{1},\dots,\underline{v}_{m} \}$ è linearmente indipendente
Dimostrazione:
$\lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{m}\underline{v}_{m}=\underline{0}$ $\underline{v}_{i}\cdot(\lambda_{1}\underline{v}_{1}+{\dots}+\lambda_{m}\underline{v}_{m})=\lambda_{1}\underline{v}_{1}\cdot \underline{v}_{i}+{\dots}+\lambda_{i}\underline{v}_{i}\cdot \underline{v}_{i}+{\dots}+\lambda_{m}\underline{v}_{m}\cdot \underline{v}_{i}=\lambda_{i}\underline{v}_{i}\cdot \underline{v}_{i}=0\implies\lambda_{i}=0$

Se $\mathrm{dim}(V)=n$ e $\underline{v}_{1},\dots,\underline{v}_{n}$ sono ortogonali a coppie $\implies \{ \underline{v}_{1},\dots,\underline{v}_{n} \}$ è una base

# Proiezioni ortogonali
$\underline{u}\ne\underline{0}\in V$
La proiezione ortogonale lungo $\underline{u}$ è la funzione
$$\begin{flalign}\mathrm{pr}_{\underline{u}}(\underline{v})=\left( \frac{\underline{u}\cdot \underline{v}}{||\underline{u}||^{2}} \right)\underline{u} &&\end{flalign}$$

# Base ortonormale
$V$ spazio vettoriale euclideo
Delta di Kronecker: $$\begin{flalign}\delta_{ij}:=\begin{cases}
1,\;i=j \\
0,\;i\neq k
\end{cases} &&\end{flalign}$$
- $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}\subset V$ è ortonormale se $\underline{v}_{i}\cdot \underline{v}_{j}=\delta_{ij}$
- Se $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}$ è una base allora è detta base ortonormale

# Metodo di Gram-Schmidt
Input: $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}$ insieme di vettori linearmente indipendenti
Output: $\{ \underline{a}_{1},\dots,\underline{a}_{m} \}$ insieme ortonormale tale che $\langle\underline{v}_{1},\dots,\underline{v}_{m}\rangle=\langle \underline{a}_{1},\dots,\underline{a}_{m}\rangle$
Procedimento:
1) $\underline{a}_{1}'=\underline{v}_{1}$
   $$\begin{flalign}\underline{a}_{i}'=\underline{v}_{i}-\sum_{j=1}^{i-1} \mathrm{pr}_{\underline{a}_{j}'}(\underline{v}_{i}) &&\end{flalign}$$
2) $\{ \underline{a}_{1}',\dots,\underline{a}_{m}' \}$ è ortogonale per costruzione
3) $$\begin{flalign}\underline{a}_{i}=\frac{\underline{a}_{i}'}{||\underline{a}_{i}'||} &&\end{flalign}$$
4) $\{ \underline{a}_{1},\dots,\underline{a}_{m} \}$ è un insieme ortonormale

# Complemento ortogonale
$V$ spazio vettoriale euclideo, $S\subset V$ sottoinsieme
$S^{\perp}=\{ \underline{v}\in V:\forall \underline{s}\in S\;\;\underline{v}\cdot \underline{s}=0 \}$ è il complemento ortogonale di $S$
$S^{\perp}\subset V$ è un sottospazio
Dimostrazione: $(\lambda \underline{v}+\mu \underline{w})\cdot \underline{s}=\lambda \underline{v}\cdot \underline{s}+\mu \underline{w}\cdot \underline{s}=0\;\;\;\forall \underline{v},\underline{w}\in S^{\perp},\;\underline{s}\in S,\;\lambda,\mu \in \mathbb{R}$

$S^{\perp}=\langle S\rangle^{\perp}$

$S\subset V\implies \mathrm{dim}(\langle S\rangle)+\mathrm{dim}(\langle S\rangle^{\perp})=\mathrm{dim}(V)$
Dimostrazione:
$\{ \underline{u}_{1},\dots,\underline{u}_{p} \}$ base ortonormale di $\langle S\rangle$, $f:V\to \mathbb{R}^{p},\;f(\underline{v})=(\underline{v}\cdot \underline{u}_{1},\dots,\underline{v}\cdot \underline{u}_{p})$
- $f$ è lineare: segue dalle proprietà del prodotto scalare
- $f$ è suriettiva:
  $f(\underline{u}_{1})=(\underline{u}_{1}\cdot \underline{u}_{1},\dots,\underline{u}_{1}\cdot \underline{u}_{p})=(1,\dots,0)$
  $\dots$
  $f(\underline{u}_{p})=(\underline{u}_{p}\cdot \underline{u}_{1},\dots,\underline{u}_{p}\cdot \underline{u}_{p})=(0,\dots,1)$
  $\{ f(\underline{u}_{1}),\dots,f(\underline{u}_{p}) \}=\{ \underline{e}_{1},\dots,\underline{e}_{p} \}\implies \mathrm{Im}(f)=\mathbb{R}^{p}$ e $\mathrm{dim}(\mathrm{Im}(f))=p=\mathrm{dim}(\langle S\rangle)$
- $\mathrm{Ker}(f)=\{ \underline{v}\in V:f(\underline{v})=\underline{0} \}=\{ \underline{v}\in V:\forall i\in \{ 1,\dots,p \}\;\;\underline{v}\cdot \underline{u}_{i}=0 \}=\langle S\rangle^{\perp}$$\implies \mathrm{dim}(\mathrm{Ker}(f))=\mathrm{dim}(\langle S\rangle^{\perp})$

# Matrici ortogonali
$A\in M_{n}(\mathbb{R})$ è ortogonale se
- è invertibile
- $A^{-1}=A^{T}$
$O_{n}(\mathbb{R})=\{ A\in M_{n}(\mathbb{R}):AA^{T}=A^{T}A=I_{n} \}$

Se $A\in O_{n}(\mathbb{R})\implies \det(A)=\pm1$
Dimostrazione: $\det(AA^{T})=\det(I_{n})\implies \det(A)\det(A^{T})=1\implies \det(A)^{2}=1\implies \det(A)=\pm1$

$A\in O_{n}(\mathbb{R})\iff$ le colonne di $A$ sono una base ortonormale di $\mathbb{R}^{n}$ rispetto al prodotto scalare canonico
Dimostrazione:
$$\begin{flalign}A=\begin{bmatrix}
\begin{array}{c|c|c}
\underline{a}_{1} & \dots & \underline{a}_{n}
\end{array}
\end{bmatrix},\;A^{T}=\begin{bmatrix}
\underline{a}_{1} \\
\hline
\dots \\
\hline
\underline{a}_{n}
\end{bmatrix}&&\end{flalign}$$
$A^{T}A=I_{n}=[\underline{a}_{i}\cdot \underline{a}_{j}]=\delta_{ij}$

# Isometrie
$V$ spazio vettoriale euclideo, $f:V\to V$ funzione lineare biunivoca
$f$ è detta isometria se $\forall \underline{v},\underline{w}\in V\;\;\underline{v}\cdot \underline{w}=f(\underline{v})\cdot f(\underline{w})$

Se $f$ è un'isometria $\implies$
- $||\underline{v}||=||f(\underline{v})||\;\;\;\forall \underline{v}\in V$
- $\mathrm{d}(\underline{v},\underline{w})=\mathrm{d}(f(\underline{v}),f(\underline{w}))\;\;\;\forall \underline{v},\underline{w}\in V$

$V$ spazio vettoriale euclideo, $f:V\to V$ funzione lineare, $B$ base ortonormale di $V$
$f$ è un'isometria $\iff M_{B}^{B}(f)$ è ortogonale
