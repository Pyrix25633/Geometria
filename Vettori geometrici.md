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
$\underline{v}\cdot  \underline{w}=|\underline{v}|\cdot |\underline{w}|\cdot \cos(\sigma)$
$\underline{v}\cdot  \underline{w}=x_{1}x_{2}+y_{1}y_{2}+z_{1}z_{2}$

# Modulo
$|\underline{v}|=\sqrt{x^{2}+y^{2}+z^{2}}$

# Proiezione
Sia $\underline{e}$ un versore, la proiezione ortogonale di $\underline{v}$ su $\underline{e}$ è il vettore geometrico $(\underline{v}\cdot  \underline{e})\cdot\underline{e}$
Se $\underline{w}$ è un vettore qualunque, la proiezione ortogonale di $\underline{v}$ su $\underline{w}$ è la proiezione di $\underline{v}$ sulla normalizzazione di $\underline{w}$, ovvero
$$\begin{flalign}\left( \underline{v}\cdot  \frac{\underline{w}}{|\underline{w}|} \right)\cdot\frac{\underline{w}}{|\underline{w}|}=\left( \underline{v}\cdot  \frac{\underline{w}}{|\underline{w}|^{2}} \right)\underline{w} &&\end{flalign}$$

# Punto in coordinate
Ad ogni punto $A$ è definito da una terna di coordinate $A=(x,y,z)$

# Vettore geometrico in coordinate
$\underline{v}=\overrightarrow{AB}=(x_{B}-x_{A},y_{B}-y_{A},z_{B}-z_{A})$