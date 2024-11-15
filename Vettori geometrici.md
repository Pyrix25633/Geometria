# Segmento orientato
Dati due punti $A,B$ nello spazio, un segmento orientato è un segmento con estremo iniziale $A$ ed estremo finale $B$ e si indica con $\overrightarrow{AB}$
Due segmenti orientati sono equivalenti se hanno la stessa direzione, lo stesso modulo e lo stesso verso

# Vettore geometrico
Un vettore geometrico è una classe di equivalenza di segmenti orientati
Il vettore nullo $\underline{0}$ è la classe di equivalenza del segmento orientato $\overrightarrow{AA}$, ha modulo nullo, direzione e verso sono indeterminati
$V^{3}$ è l'insieme di vettori geometrici nello spazio

# Somma
$\underline{v}=\overrightarrow{AB}=(x_{1},y_{1},z_{1}),\;\underline{w}=\overrightarrow{BC}=(x_{2},y_{2},z_{2})$
$\underline{v}+\underline{w}=\overrightarrow{AC}=(x_{1}+x_{2},y_{1}+y_{2},z_{1}+z_{2})$
Proprietà:
- Commutativa: $\underline{v}+\underline{w}=\underline{w}+\underline{v}$
- Associativa: $\underline{s}+(\underline{v}+\underline{w})=(\underline{s}+\underline{v})+\underline{w}$

# Opposto
L'opposto di $\underline{v}\neq \underline{0}$ è $-\underline{v}$, un vettore con lo stesso modulo, la stessa direzione e verso opposto
$\underline{v}+(-\underline{v})=\underline{0}$

# Prodotto per uno scalare
$\underline{v}\neq \underline{0},\;\lambda\neq0$
$\lambda  \underline{v}$ è un vettore con la stessa direzione, modulo $\lambda\cdot |\underline{v}|$ e verso:
- concorde se $\lambda>0$
- opposto se $\lambda<0$
Se invece $\lambda=0$ allora $\lambda  \underline{v}=\underline{0}$

# Versore
Un versore è un vettore geometrico con modulo $1$
Se $\underline{v}\neq 0$ la normalizzazione di $\underline{v}$ è definita come
$$\begin{flalign}\frac{\underline{v}}{|\underline{v}|} &&\end{flalign}$$

# Prodotto scalare di due vettori geometrici
Il prodotto scalare è lo scalare
$\underline{v}\cdot  \underline{w}=|\underline{v}|\cdot |\underline{w}|\cdot \cos(\sigma)$
$\underline{v}\cdot  \underline{w}=x_{1}x_{2}+y_{1}y_{2}+z_{1}z_{2}$

# Modulo
$|\underline{v}|=\sqrt{x^{2}+y^{2}+z^{2}}$

# Proiezione
Sia $\underline{e}$ un versore, la proiezione ortogonale di $\underline{v}$ su $\underline{e}$ è il vettore geometrico $(\underline{v}\cdot  \underline{e})\cdot\underline{e}$
Se $\underline{w}$ è un vettore qualunque, la proiezione ortogonale di $\underline{v}$ su $\underline{w}$ è la proiezione di $\underline{v}$ sulla normalizzazione di $\underline{w}$, ovvero
$$\begin{flalign}\left( \underline{v}\cdot  \frac{\underline{w}}{|\underline{w}|} \right)\cdot\frac{\underline{w}}{|\underline{w}|}=\left( \underline{v}\cdot  \frac{\underline{w}}{|\underline{w}|^{2}} \right)\underline{w} &&\end{flalign}$$

# Prodotto vettoriale
Il prodotto vettoriale $\underline{v}\times  \underline{w}$ è:
- il vettore nullo $\underline{0}$ se $\underline{v}$ e $\underline{w}$ sono paralleli o uno o entrambi sono nulli
- $\underline{u} \in V^{3}$ tale che:
	- modulo: $|\underline{u}|=|\underline{v}||\underline{w}|\cos(\sigma)$
	- direzione: ortogonale a $\underline{v}$ e $\underline{w}$
	- verso: dato dalla "regola della mano destra"
$\underline{v}\times  \underline{w}=(v_{2}w_{3}-v_{3}w_{2},\;v_{3}w_{1}-v_{1}w_{3},\;v_{1}w_{2}-v_{2}w_{1})$

Se $\underline{v},\underline{w}\neq \underline{0}$  e non paralleli $\implies |\underline{v}\times \underline{w}|$ è l'area del parallelogramma individuato da $\underline{v}$ e $\underline{w}$
Dimostrazione:
$h=|\underline{w}|\sin(\sigma),\;b=|\underline{v}|\implies b\cdot h=|\underline{v}||\underline{w}|\sin(\sigma)$

Proprietà:
- Anticommutativa: $\underline{v}\times \underline{w}=-\underline{w}\times \underline{v}$
- Associativa: $(\lambda \underline{v})\times \underline{w}=\underline{v}\times(\lambda \underline{w})=\lambda(\underline{v}\times \underline{w})$
- Distributiva: $(\underline{v}+\underline{w})\times \underline{u}=\underline{v}\times \underline{u}+\underline{w}\times \underline{u}$
- Distributiva: $\underline{v}\times(\underline{w}+\underline{u})=\underline{v}\times \underline{w}+\underline{v}\times \underline{w}$

# Prodotto misto
Il prodotto misto è lo scalare $\underline{v}\cdot(\underline{w}\times  \underline{u})$

Se $\underline{v},\underline{w},\underline{u}\neq\underline{0}$ e non paralleli $\implies |\underline{v}\cdot(\underline{w}\times \underline{u})|$ è il volume del parallelepipedo individuato da $\underline{v}$, $\underline{w}$ e $\underline{u}$
Dimostrazione:
$S=(\underline{w}\times \underline{u}),\;h=|\underline{v}|\cos(\sigma) \implies S\cdot h=|\underline{w}\times \underline{u}||\underline{v}|\cos(\sigma)$

# Punto in coordinate
Ad ogni punto $A$ è definito da una terna di coordinate $A=(x,y,z)$

# Vettore geometrico in coordinate
$\underline{v}=\overrightarrow{AB}=(x_{B}-x_{A},\;y_{B}-y_{A},\;z_{B}-z_{A})$

$\underline{i},\underline{j},\underline{k}$ sono i versori degli assi cartesiani a due a due ortogonali: $\underline{i}\cdot \underline{j}=\underline{i}\cdot \underline{k}=\underline{j}\cdot \underline{k}=0$
$\underline{v}=x\underline{i}+y\underline{j}+z\underline{k}$

$\underline{i}\times \underline{j}=\underline{w},\;\underline{j}\times \underline{i}=-\underline{w}$
