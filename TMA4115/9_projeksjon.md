
## Projeksjon

### Ortogonal projeksjon i $R^2$


### Skalarproduktet i $R^n$
**Teorem 9.3.** Den ortogonale projeksjonen på en vektor $v$,
$$ \begin{gather*}
    P_v : \mathbb{R}^n \rightarrow \mathbb{R}^n \\
    P_v(w)=\frac{v \cdot w}{v \cdot v}\,v
\end{gather*} $$
er en lineærtransformasjon.


### Indreproduktrom
**Definisjon.** La $V$ være et reelt vektorrom. Et *indreproduktrom* i $V$ er en operasjon som tar inn to vektorer, $v$ og $w$, for å gi ut et reelt tall $\langle v, w \rangle$. Operasjonen tilfredsstiller
$$ \begin{align*}
    &\langle v, w \rangle = \langle w, v \rangle &\text{(symmetri)} \\
    &\langle v, (aw + bu) \rangle = a \langle v, w \rangle + b \langle v, u \rangle &\text{(linearitet)} \\
    &\langle v, v \rangle \geq 0 \text{, og } \langle v, v \rangle = 0 \text{ kun hvis } v = 0 &\text{(positivitet)}
\end{align*} $$
Vi sier at $V$, sammen med et valgt indreprodukt, er et *indreproduktrom*.
**Teorem 9.6.** (Pytagoras). La $V$ være et reelt indrproduktrom. Dersom vektorene $v$ og $w$ er ortogonale, er
$$ \lVert v + w \rVert = \lVert v \rVert^2 + \lVert w \rVert^2 $$
**Teorem 9.7.** (Cauchy-Schwarz). La $V$ være et reelt indreproduktrom. Alle vektorer $v$ og $w$ tilfredstiller
$$| \langle v, w \rangle | \leq \lVert v \rVert \lVert w \rVert $$
**Teorem 9.8.** La $V$ være et indreproduktrom. Den ortogonale projeksjonen på en vektor $v$,
$$ \begin{gather*}
    P_v : \mathbb{R}^n \rightarrow \mathbb{R}^n \\
    P_v(w)=\frac{\langle v, w \rangle}{\langle v, v \rangle}\,v
\end{gather*} $$
er en lineærtransformasjon.
**Teorem 9.9.** La $v$ og $w$ være to vektorer i et indreproduktrom $V$. Da er $P_v(w)$ og $w-P_v(w)$ ortogonale.


### Ortogonal projeksjon
**Definisjon.** En *ortogonal mengde* er en mengde av ikke-null vektorer $u_1, u_2, \dots, u_n$, slik at
$$ \langle u_i, u_k \rangle = 0 $$
for alle vektorer $u_i$ og $u_k$ i mengden med $i \neq k$. Dersom i tillegg $\lVert u_j \rVert = 1$ for alle vektorene, sier vi at mengden er *ortonormal*.
**Teorem 9.10.** En ortogonal mengde er lineært uavhengig.
**Definisjon.** Dersom en ortogonal mengde $u_1, u_2, \dots, u_n$ i $V$ også er en basis, sier vi at mengden er en *ortogonal basis* for $V$.
**Teorem 9.12.** Koordinatene til $v$ i en ortogonal basis $u_1, u_2, \dots, u_n$ er
$$ \begin{align*}
    v &= P_{u_1}(v) + P_{u_2}(v) + \dots + P_{u_n}(v) \\
    &= \frac{\langle u_1, v \rangle}{\langle u_1, u_1 \rangle}\,u_1
    + \frac{\langle u_2, v \rangle}{\langle u_2, u_2 \rangle}\,u_2
    + \dots + \frac{\langle u_n, v \rangle}{\langle u_n, u_n \rangle}\,u_n
\end{align*} $$
**Teorem 9.13.** La $u_1, u_2, \dots, u_n$ være en ortogonal basis for $U$, et underrom av $V$. Punktet
$$ \begin{align*}
    P_U(v) &= P_{u_1}(v) + P_{u_2}(v) + \dots + P_{u_n}(v) \\
    &= \frac{\langle u_1, v \rangle}{\langle u_1, u_1 \rangle}\,u_1
    + \frac{\langle u_2, v \rangle}{\langle u_2, u_2 \rangle}\,u_2
    + \dots + \frac{\langle u_n, v \rangle}{\langle u_n, u_n \rangle}\,u_n
\end{align*} $$
er et punktet i $U$ som har kortest avstand til $v$, altså
$$ \lVert v - P_U(v) \rVert = \text{min}_{u \in U} \lVert v - u \rVert $$
**Teorem 9.15.** La $u_1, u_2, \dots, u_n$ være en basis for et underrom $U$. En vektor $v$ er i det ortogonale komplementet til $U$ hvis og bare hvis $\langle u_i, v \rangle = 0$ for alle $i$.

**Teorem 9.17.** La $U$ være et underrom av et indreproduktrom $V$. Da gjelder
$$ \dim{U} + \dim{U^\perp} = \dim{V} $$
**Teorem 9.18.** La $A$ være en $m \times n$-matrise. Da vet vi
$$ \begin{align*}
    (\text{Col}\,A)^\perp &= \text{Null}\,A^T \\
    (\text{Null}\,A)^\perp &= \text{Col}\,A^T
\end{align*} $$


### Finne en ortogonal basis: Gram-Schmidts metode
**Teorem 9.19.** Mengden $u_1, u_2, \dots, u_n$ gitt ved
$$ \begin{align*}
    u_k &= v_k - \sum_{j=1}^{k-1}\,P_{u_j}(v_k) \\
    &= v_k - \sum_{j=1}^{k-1}\,\frac{\langle u_j, v_k \rangle}{\langle u_j, u_j \rangle}\,u_j
\end{align*} $$
er en ortogonal basis for rommet utspent av $v_1, v_2, \dots, v_n$.


### Beregne den ortogonale basisen
La $U$ være et underrom til et indreproduktrom $V$. Her er en metode for å regne ut den ortogonale projeksjonen $P_U$:

-  Ta utgangspunkt i en basis $v_1, v_2, \dots, v_n$ som spenner ut $U$.
-  Bruk så Gram-Schmidt til å finne en ortogonal basis $u_1, u_2, \dots, u_n$ for $U$.
-  Da kan man, for alle $v$ i $V$, beregne den ortogonale projeksjonen
$$P_U(x) = P_{u_1}(x) + P_{u_2}(x) + \dots + P_{u_n}(x) $$
-  Hvis $V = \mathbb{R}^n$, så får vi standardmatrisen
$$ [\, P_U \,] = [\, P_U(e_1) \ P_U(e_2) \ \dots \ P_U(e_n) \, ] $$
og da kan man, for alle $x$ i $V$, beregne den ortogonale projeksjonen $P_U(x) = [\, P_U \,]x$.



### Indreproduktrom mellom funksjoner
**Teorem 9.22.** Operasjonen
$$ \langle f, g \rangle = \frac{1}{b - a} \int_a^b f(x)\,g(x)\,dx $$
er et indreprodukt på $C([a, b])$.

**Teorem 9.27.** Vektorene $1$, $\cos{nx}$ og $\sin{mx}$, hvor $n, m = 1, 2, 3, \dots,$ er parvis ortogonale i $C_s([-\pi, \pi])$.


### Komplekse indreprodukt
**Definisjon.** La $V$ være et komplekst vektorrom. Et *indreproduktrom* i $V$ er en operasjon som tar inn to vektorer, $v$ og $w$, for å gi ut et komplekst tall $\langle v, w \rangle$. Operasjonen tilfredsstiller
$$ \begin{align*}
    &\langle v, w \rangle = \overline{ \langle w, v \rangle } &\text{(konj. sym.)} \\
    &\langle v, (aw + bu) \rangle = a \langle v, w \rangle + b \langle v, u \rangle &\text{(linearitet)} \\
    &\langle v, v \rangle \geq 0 \text{, og } \langle v, v \rangle = 0 \text{ kun hvis } v = 0 &\text{(positivitet)}
\end{align*} $$
Vi sier at $V$, sammen med et valgt indreprodukt, er et *indreproduktrom*.

**Teorem 9.29.** Alt som gjelder for reelle indreproduktrom, med unntak av vinkelen, gjelder også for komplekse indreproduktrom.

**Teorem 9.33.** La $A$ være en kompleks $m \times n$-matrise. Da har vi
$$ \begin{align*}
    (\text{Col}\,A)^\perp &= \text{Null}\,A^* \\
    (\text{Null}\,A)^\perp &= \text{Col}\,A^*
\end{align*} $$




