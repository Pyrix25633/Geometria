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