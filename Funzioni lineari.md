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

$\mathrm{Ker(f)}$ è un sottospazio vettoriale
Dimostrazione: $f(\lambda \underline{v}+\mu \underline{w})=\lambda f(\underline{v})+\mu f(\underline{w})=\lambda \underline{0}_{V'}+\mu \underline{0}_{V'}=\underline{0}_{V'} \implies \lambda \underline{v}+\mu \underline{w}\in \mathrm{Ker}(f)\;\;\;\forall \underline{v},\underline{w}\in V,\;\lambda,\mu \in \mathbb{R}$
Le seguenti condizioni sono equivalenti:
- $\mathrm{Ker}(f)=\{ \underline{0}_{V} \}$
- $f$ è iniettiva
- Se $\{ \underline{v}_{1},\dots,\underline{v}_{m} \}\subset V$ è linearmente indipendente $\implies \{ f(\underline{v}_{1}),\dots,f(\underline{v}_{m}) \}\subset V'$ è linearmente indipendente


# Immagine