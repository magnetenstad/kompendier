
## Diagonalisering
**Definsjon.** Vi sier at en $n \times $-matrise er *diagonaliserbar* hvis det finnes en diagonalmatrise $D$ og en inverterbar matrise $P$ slik at
$$ A = PDP^{-1} $$
Vi sier da at $P$ diagonaliserer $A$.

**Teorem 11.2.** En $n \times n$-matrise $A$ her diagonaliserbar hvis og bare hvis $A$ har $n$ lineært uavhengige egenvektorer.

**Teorem 11.3.** Hvis en $n \times n$-matrise $A$ har $n$ forskjellige egenverdier, så er $A$ diagonaliserbar.

**Teorem 11.4.** En $n \times n$-matrise $A$ er diagonaliserbar hvis og bare hvis $A$ har $n$ egenverdier og dimensjonen til egenrommet til hver egenverdi $\lambda$ er lik den algebraiske multiplisiteten til $\lambda$.

**Teorem 11.5.** En kompleks $n \times n$-matrise $A$ er diagonaliserbar hvis og bare hvis det finnes en basis for $\mathbb{C}^n$ som kun består av egenvektorer for $A$. En reell $n \times n$-matrise $A$ er diagonaliserbar som en reell matrise hvis og bare hvis det finnes en basis for $\mathbb{R}^n$ som kun består av egenvektorer for $A$.

**Teorem 11.6.** La $T: V \rightarrow V$ være en lineærtransformasjon. Vi antar at $T$ er diagonaliserbar og at $B = (v_1, \dots, v_n)$ er en basis som består av $T$ sine egenvektorer. Da er matrisen som beskriver $T$ med hensyn på basisen $B$ en diagonalmatrise $D$, med egenverdierne $\lambda_1, \dots, \lambda_n$ til $T$ på diagonalen.


### Eksempler


### Mer om komplekse egenverdier
**Teorem 11.11.** La $A$ være en reell $2 \times 2$-matrise med kompleks egenverdi $\lambda = a - bi$, med $b \neq 0$, og la $v \in \mathbb{C}^2$ være en egenvektor som hører til $\lambda$. Da kan vi faktorisere $A$ på følgende måte:
$$ A = PCP^{-1} \ \text{med} \ P = [\, \text{Re}\,v \ \text{Im}\,v\,] $$
og
$$ C = \begin{bmatrix}
    a & -b \\ b & a
\end{bmatrix} $$


### Symmetriske matriser
**Definisjon.** En reell matrise kalles *symmetrisk* dersom $A = A^T$.

**Teorem 11.14.** La $A$ være en symmetrisk $n \times n$-matrise. Da har $A$ $n$ reelle egenverdier (talt med multiplisitet) og $A$ er diagonaliserbar (som en reell matrise).


### Symmetri og ortogonalitet
**Teorem 11.16.** La $A$ være en symmetrisk $n \times n$-matrise. Egenvektorene til $A$ tilhørende to distinkte egenverdier er ortogonale.

**Definisjon.** En $n \times n$-matrise er *ortogonalt diagonaliserbar* dersom den har $n$ ortogonale egenvektorer.

**Teorem 11.17.** En reell $n \times n$-matrise er ortogonalt diagonaliserbar hvis og bare hvis den er symmetrisk.

**Definisjon.** En $n \times n$-matrise $A$ kalles *hermitsk* hvis
$$ A = A^* $$
**Teorem 11.18.** En hermitsk $n \times n$-matrise har $n$ reelle egenverdier (talt med multiplisitet) og er ortogonalt diagonaliserbar.

