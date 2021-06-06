
## Lineærtransformasjoner


### Funksjoner
**Definisjon.** En *funksjon* består av:

-  En mengde som kalles funksjonens *domene*.
-  En mengde som kalles funksjonens *kodomene*.
-  En regel som til hvert element i domenet tilordner et element i kodomenet.

**Definisjon.** La $f: A \rightarrow B$ være en funksjon. Vi sier at $f$ er *injektiv* (eller *en-til-en*) hvis det for hver $b$ i $B$ er maksimalt én $a$ i $A$ slik at $f(a) = b$. Vi sier at $f$ er *surjektiv* (eller *på*) hvis det for hver $b$ i $B$ finnes en $a$ i $A$ slik at $f(a) = b$. *Bildet* til $f$ er mengden av alle elementer i kodomenet som blir truffet av $f$, altså delmengden $\text{im} f = \{\, f(a) \ | \ a \in A \}$ av $B$.

Det følger umiddelbart fra definisjonen at en funksjon $f: A \rightarrow B$ er surjektiv hvis og bare hvis bildet til funksjonen er hele kodomenet: $\text{im} f = B$.


### Lineærtransformasjoner
**Definisjon.** La $V$ og $W$ være vektorrom. En funksjon $T: V \rightarrow W$ er en *lineærtransformasjon* hvis den oppfyller følgende to kriterier:

-  $T(u + v) = T(u) + T(v)$ for alle $u$ og $v$ i $V$.
-  $T(cu) = c \cdot T(u)$ for alle vektorer $u$ i $V$ og alle skalarer $c$.

**Teorem 8.3.** Hvis $T: V \rightarrow W$ er en lineærtrasformasjon, så oppfyller den følgende:

-  En lineærkombinasjon i $V$ sendes til den tilsvarende lineærkombinasjonen i $W$:
$$T(c_1v_1 + c_2v_2 + \cdots + c_rv_r) = c_1 \cdot T(v_1) + c_2 \ T(v_2) + \cdots + c_2 \cdots T(v_r) $$
-  Nullvektoren i $V$ sendes til nullvektoren i $W$: $$ T(0) = 0 $$

**Teorem 8.4.** La $V$ og $W$ være endeligdimensjonale vektorrom og la $T: V \rightarrow W$ være en lineærtransformasjon. Anta $B = (b_1, \dots, b_n)$ er en basis for $V$. Da er $T$ fullstendig bestemt av bildene $T(b1), \dots, T(b_n)$ av basisvektorene.


### Kjerne og bilde
**Definisjon.** La $T: V \rightarrow W$ være en lineærtransformasjon. *Kjernen* til $T$ er mengden av alle vektorer i $V$ som blir sendt til nullvektoren i $W$:
$$ \text{ker}\,T = \{\,v \in V \ | \ T(v) = 0 \} $$
**Teorem 8.8.** La $T: V \rightarrow W$ være en lineærtransformasjon.

-  Kjernen $\text{ket}\,T$ er et underrom av $V$.
-  Bildet $\text{im}\,T$ er et underrom av $W$.

**Teorem 8.9.** En lineærtransformasjon $T: V \rightarrow W$ er injektiv hvis og bare hvis $\text{ker}\,T=\{\,0\,\}$.


### Lineærtransformasjoner gitt ved matriser
**Teorem 8.11.** La $A$ være en $m \times n$-matrise, og la $T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ være en lineærtransformasjon gitt ved $T(x) = Ax$. Da er
$$ \text{ker}\,T = \text{Null}\,A \quad \text{og} \quad \text{im}\,T=\text{Col}\,A $$
**Teorem 8.13.** La $T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ være en lineærtransformasjon. Da er
$$ T(x) = Ax \quad \text{for alle } x \text{ i } \mathbb{R}^n $$
der $A$ er $m \times n$-matrisen gitt ved
$$ [ \ T(e_1) \ T(e_2) \ \cdots \ T(e_n) \ ] $$
hvor $(e_1, e_2, \dots, e_n)$ er standardmatrisen for $\mathbb{R}^n$.
**Definisjon.** Matrisen $A$ i teorem 8.13 kalles *standardmatrisen* til lineærtransformasjonen $T$.
**Teorem 8.14.** La $T: \mathbb{R}^n \rightarrow \mathbb{R}^m$ være en lineærtransformasjon og la $A$ være standardmatrisen til $T$. Da vet vi:

-  $T$ er surjektiv hvis og bare hvis kolonnene i $A$ utspenner hele $\mathbb{R}^m$.
-  $T$ er injektiv hvis og bare hvis kolonnene i $A$ er lineært uavhengige.



### Lineærtransformasjoner og basiser
**Teorem 8.15.** La $V$ og $W$ være endeligdimensjonale vektorrom, og la $B$ og $C$ være basiser for henholdsvis $V$ og $W$. La $T: V \rightarrow W$ være en lineærtransformasjon. Da finnes en matrise $A$ slik at
$$ [ \ T(x) \ ]_C = A \cdot [ \ x \ ]_B $$
for alle vektorer $x$ i $V$.

**Teorem 8.16.** La $V$ være et $n$-dimensjonalt vektorrom, og la $B = (b_1, b_2, \dots, b_n)$ og $C = (c_1, c_2, \dots, c_n)$ være to basiser for $V$. Da finnes en $n \times n$-matrise $A$ slik at
$$ [ \ x \ ]_C = A \cdot [ \ x \ ]_B $$
for alle vektorer $x$ i $V$.


### Isomorfi
**Definisjon.** La $T: V \rightarrow W$ være en lineærtransformasjon. En *invers* til $T$ er en lineærtransformasjon $S: W \rightarrow V$ som er slik at
$$ \begin{align*}
    S(T(v)) = v \quad &\text{for alle } v \text{ i } V \text{, og} \\
    T(S(w)) = w \quad &\text{for alle } w \text{ i } W
\end{align*} $$
**Definisjon.** Hvis $T: V \rightarrow W$ er en lineærtransformasjon som har en invers, så er $T$ en *isomorfi*. Da sier vi dessuten at vektorrommene $V$ og $W$ er *isomorfe*, og vi skriver $V \cong W$.

**Teorem 8.19.** En lineærtransformasjon er en isomorfi hvis og bare hvis den er både injektiv og surjektiv.

**Teorem 8.22.** Hvis $V$ er et $n$-dimensjonalt komplekst vektorrom, så er $V$ isomorft med $\mathbb{C}^n$. Og hvis $W$ er et $n$-dimensjonalt reelt vektorrom, så er $W$ isomorft med $\mathbb{R}^n$.




