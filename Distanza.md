# Tra due punti
$P=(x_{P},y_{P},z_{P}),\;Q=(x_{Q},y_{Q},z_{Q})$
$d(P,Q)=|\overrightarrow{PQ}|=\sqrt{(x_{Q}-x_{P})^{2}+(y_{Q}-y_{P})^{2}+(z_{Q}-z_{P})^{2}}$

# Tra un punto e un piano
$P=(x_{P},y_{P},z_{P}),\;\pi:ax+by+cz+d=0$
$$\begin{flalign}d(P,\pi)=\frac{|a\cdot x_{P}+b\cdot y_{P}+c\cdot z_{P}+d|}{\sqrt{a^{2}+b^{2}+c^{2}}} &&\end{flalign}$$

# Tra un punto e una retta
$P=(x_{P},y_{P},z_{P}),\;r:(x_{r},y_{r},z_{r})+t(x_{t},y_{t},z_{t})$
$Q(t)=(x_{r}+tx_{t},\;y_{r}+ty_{t},\;z_{r}+tz_{t})$
$\overrightarrow{PQ(t)}=(x_{r}+tx_{t}-x_{P},\;y_{r}+ty_{t}-y_{P},\;z_{r}+tz_{t}-z_{P})$
Si impone $\overrightarrow{PQ(t)}\cdot(x_{t},y_{t},z_{t})=0$ trovando $t_{0}$
$d(P,r)=d(P,Q(t_{0}))$

# Tra due rette
$r:(x_{r},y_{r},z_{r})+t(x_{t},y_{t},z_{t}),\;r':(x_{r'},y_{r'},z_{r'})+s(x_{s},y_{s},z_{s})$
Si impone
$$\begin{flalign}\begin{cases}
\overrightarrow{P(t)Q(s)}\cdot(x_{t},y_{t},z_{t})=0 \\
\overrightarrow{P(t)Q(s)}\cdot(x_{s},y_{s},z_{s})=0
\end{cases} &&\end{flalign}$$
trovando $t_{0}$ e $s_{0}$
$d(r,r')=d(P(t_{0}),Q(s_{0}))$
