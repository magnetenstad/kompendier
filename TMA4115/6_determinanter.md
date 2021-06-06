
## Determinanter

### Determinanter for 2 x 2-matriser
For en $2 \times 2$-matrise
$$ A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} $$
er determinanten definert ved:
$$ \det{A} = \begin{vmatrix} a & b \\ c & d \end{vmatrix} = ad - bc $$
Arealet av parallellogrammet utspent av kolonnene i $A$ er lik
$$ | \det{A} | $$


### Determinanter for 3 x 3-matriser
For en $3 \times 3$-matrise
$$ A =
\begin{bmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{bmatrix} $$
er determinanten definert ved:
$$ \begin{align*}
    \det{A} &=
    \begin{vmatrix}
    a_{11} & a_{12} & a_{13} \\
    a_{21} & a_{22} & a_{23} \\
    a_{31} & a_{32} & a_{33} \\
    \end{vmatrix} \\
    &=
	  a_{11}\begin{vmatrix} a_{22} & a_{23} \\ a_{32} & a_{33} \end{vmatrix}
    - a_{12}\begin{vmatrix} a_{21} & a_{23} \\ a_{31} & a_{33} \end{vmatrix}
    + a_{13}\begin{vmatrix} a_{21} & a_{22} \\ a_{31} & a_{32} \end{vmatrix}
	\\
    &= a_1 \cdot a_2 \times a_3 = |a_1|\,|a_2|\,|a_3|\,\sin{\alpha}\cos{\theta}
\end{align*} $$


### Determinanter: generell definisjon


### Kofaktorekspansjon


### Determinanter og radoperasjoner
**Teorem 6.5.** La $A$ være en $n \times n$-matrise, og la $B$ være en matrise vi får ved å utføre en radoperasjon på $A$. Da har vi følgende sammenheng mellom determinantene til $A$ og $B$, basert på hvilken type radoperasjon vi utførte:
\begin{table}[h]
    \centering
    \begin{tabular}{c|c}
        Radoperasjon & Resultat 
        \hline 
        Gange en rad med et tall $k$ & $\det{B} = k \cdot \det{A}$ 
        Legge til et multiplum av én rad i en annen & $\det{B} = \det{B}$ 
        Bytte om to rader & $\det{B} = -\det{A}$
    \end{tabular}
\end{table}


### Triangulære matriser
**Teorem 6.8.** La $A$ være en (øvre eller nedre) triangulær $n \times n$-matrise. Da er determinanten til $A$ lik produktet av tallene på diagonalen i $A$:
$$ \det{A} = a_{11} \cdot a_{22} \cdot \cdots \cdot a_{nn} $$


### Flere regneregler for determinanter
**Teorem 6.10.** Determinanten til et produkt av to matriser er produktet av determinantene. Altså: Hvis $A$ og $B$ er to $n \times n$-matriser, så er
$$ \det{AB} = (\det{A})(\det{B}) $$
**Teorem 6.11.** Determinanten endrer seg ikke når vi transponerer matrisen. Altså: Hvis $A$ er en $n \times n$-matrise, så er
$$ \det{A} = \det{A^{\top}} $$


### Karakterisering av inverterbarhet
**Teorem 6.12.** La $A$ være en $n \times n$-matrise. Følgende påstander er ekvivalente:

-  $A$ er inverterbar.
-  $\det{A} \neq 0$.
-  Kolonnene i $A$ er lineært uavhengige.
-  Kolonnene i $A$ utspenner $\mathbb{C}^n$.




