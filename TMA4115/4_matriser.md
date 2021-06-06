
## Matriser

### Definisjoner og notasjon


### Produkt av matrise og vektor
**Teorem 4.6.** Hvis $A$ er en $m \times n$-matrise, $v$ og $w$ er vektorer i $\mathbb{R}^n$ og $c$ er en skalar, så har vi følgende likheter:
$$ A(v + w) = Av + Aw $$
$$ A(cv) = c(Av) $$
**Teorem 4.9.** Hvis $A$ og $B$ er $m \times n$-matriser, $v$ er en vektorer i $\mathbb{R}^n$ og $c$ er en skalar, så har vi følgende likheter:
$$ (A + B)v = Av + Bv $$
$$ (cA)v = c(Av) $$


### Matriselikninger


### Sum og skalering av matriser


### Vektorer som matriser


### Matrisemultiplikasjon
Definisjon. La A være en $m \times n$-matrise med rader
$a_1, a_2, \dots, a_m$, og la B være en $n \times p$-matrise med
kolonner $b_1, b_2, \dots, b_p$. Produktet av A og B er definert ved:
$$ AB = \begin{bmatrix}
a_1b_1 & a_1b_2 & \cdots & a_1b_p \\
a_1b_1 & a_1b_2 & \cdots & a_1b_p \\
\vdots & \vdots & \ddots & \vdots \\
a_mb_1 & a_mb_2 & \cdots & a_mb_p 
\end{bmatrix} $$

**Teorem 4.13.** La $A$, $B$, og $C$ være matriser, $v$ en vektor, og $c$ et tall. I hver del av teoremet antar vi at størrelsene på matrisene og vektoren er slik at alle operasjonene som brukes er definert.
(a) Matrisemultiplikasjon er en assosiativ operasjon, det vil si:
$$ A(BC) = (AB)C $$
Et spesialtilfelle av dette er følgende:
$$ (AB)v = A(Bv) $$
(b) Å skalere et matriseprodukt er det samme som å skalene én av faktorene og deretter multiplisere:
$$ (cA)B = c(AB) = A(cB) $$
(c) Matrisemultiplikasjon distribuerer over addisjon av matriser, det vil si:
$$ A(B+C) = AB + AC $$
$$ (A + B)C = AC +\ BC $$


### Transponering
Operasjonen *transponering} går ut på å bytt om rader og kolonner.

**Teorem 4.15.** For enhver matrise $A$ har vi:
$$ (A^\top)^\top = A $$
Hvis $A$ og $B$ er matriser slik at produktet $AB$ er definert, så er:
$$ (AB)^\top = B^\top A^\top $$


### Identitetsmatriser
La $I = I_n$ være den kvadratiske $n \times n$-matrisen
$$ I_n = \begin{bmatrix}
1 & 0 & \cdots & 0 \\
0 & 1 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & 1
\end{bmatrix} $$
Da er $IA = A$ for enhver $n \times p$-matrise $A$ og $BI = B$ for enhver $m \times n$-matrise $B$. Spesielt er $Ix = x$ for enhver vektor $x$. Derfor kalles $I = I_n$ en identitetsmatrise, eller en $n \times n$-identitetsmatrise.


### Potenser av matriser
Hvis $A$ er en kvadratisk matrise, så kan vi gange $A$ med seg selv. Generelt definerer vi at $A$ opphøyd i $n$-te er produktet av $A$ med seg selv $n$ ganger:
$$ A^n = A \cdot A \cdot \cdots \cdot A $$
For tall har vi definert at $a^0 = 1$. For kvadratiske matriser har vi derimot
$$ A^0 = I_n $$


### Inverser
**Definisjon.** La $A$ være en $n \times $-matrise. En *invers} til $A$ er en $n \times n$-matrise $B$ som er slik at
$$ A \cdot B = I_n = B \cdot A $$
En matrise er *inverterbar} hvis den har en invers.

**Teorem 4.18.** Hvis en matrise er inverterbar, så har den nøyaktig én invers.

**Teorem 4.20.** La $A$ være en $n \times n$-matrise, og $b$ en vektor. Hvis $A$ er inverterbar, så har likningen $Ax = b$ entydig løsning, og løsningen er $x = A^{-1}b$.


### Samtidig løsning av flere systemer


### Beregning av inverser
**Teorem 4.25.** La $A$ være en $n \times n$-matrise.
(a) $A$ er inverterbar hvis og bare hvis $A \sim I_n$.

(b) Hvis $A$ er inverterbar, så kan vi finne inversen ved å gausseliminere matrisen
$$ \begin{bmatrix} A \ | \ I_n \end{bmatrix} $$
til redusert trappeform og lese av høyre halvdel av den resulterende matrisen. Med andre ord: Resultatet av gausseliminasjonen blir følgende matrise: 
$$ \begin{bmatrix} I_n \ | \ A^{-1} \end{bmatrix} $$

### Formel for invertering av $2 \times 2$-matrise
La
$$ A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} $$
Da er
$$ A^{-1} = \frac{1}{ad-bc} \, \begin{bmatrix} d & -b \\ -c & a \end{bmatrix} $$



