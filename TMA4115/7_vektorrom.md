
## Vektorrom


### Reelle og komplekse vektorrom


### Aksiomer for vektorrom


### Definisjonen av vektorrom
**Definisjon.** La $V$ være en mengde, og anta at vi har definert to operasjoner:
$$ \begin{gather*}
    \text{addisjon av vektorer:} \ u + v \\
    \text{skalarmultiplikasjon:} \ c \cdot u
\end{gather*} $$
Addisjon skal være definert for alle elementer $u$ og $v$ i $V$, og skalarmultiplikasjonen for alle skalarer $c$ og alle $u$ i $V$. Resultatet av operasjonene skal alltid være et element i $V$. Dersom mengden $V$ og de to operasjonene oppfyller vektorromsaksiomene (V1)-(V8), så sier vi at $V$ er et *vektorrom*, og vi kaller elementene i $V$ for *vektorer*.


### Første eksempler


### Generelle egenskaper og lineær uavhengighet
**Definisjon.** La $v_1, v_2, \dots, v_n$ være vektorer i vektorommet $V$. Disse vektorene er *lineært* uavhengige dersom likningen
$$c_1 \cdot v_1 + c_2 \cdot v_2 + \cdots + c_n \cdot v_n = 0 $$
ikke har andre lsninger enn den trivielle løsningen $c_1 = c_2 = \cdots = c_n = 0.$ I motsatt tilfelle kalles de *lineært avhengige*.

**Teorem 7.3.** Gitt $n$ vektorer $v_1, v_2, \dots, v_n$ i et vektorrom $V$. Hvis

-  en av vektorene er en lineærkombinasjon av de andre, eller
-  en av vektorene er $0$,

så er vektorene lineært avhengige.


### Flere eksempler på vektorrom

-  Polynomer av begrenset grad.
-  Alle polynomer.
-  Kontinuerlige funksjoner.
-  Deriverbare og glatte funksjoner.
-  Matriser.



### Underrom
**Definisjon.** Et *underrom* av et vektorrom $V$ er en delmengde $U \subseteq V$ som i seg selv utgjør et vektorrom, med addisjon og skalarmultipliskasjon definert på samme måte som i $V$.

**Teorem 7.9.** La $V$ være et vektorrom. En delmengde $U \subseteq V$ er et underrom av $V$ hvis og bare hvis følgende tre betingelser er oppfylt.

-  Nullvektoren $0$ i $V$ ligger i $U$.
-  For alle vektorer $u$ og $v$ i $U$ er også summen $u + v$ i $U$.
-  For alle vektorer $u$ i $U$ og alle skalarer $c$ er også skalarproduktet $cu$ u $U$.

**Teorem 7.11.** En mengde $\text{Sp}\{v_1, v_2, \dots, v_n\}$ utspent av vektorer i et vektorrom $V$ er alltid et underrom av $V$.


### Endeligdimensjonale vektorrom
**Definisjon.** Et vektorrom $V$ er *endeligdimensjonalt* hvis det finnes en endelig mengde av vektorer i $V$ som utspenner $V$. Ellers er $V$ *uendeligdimensjonalt*.


### Basis
**Definisjon.** En *basis* fpr et vektorrom $V$ er en liste
$$ B = (b_1, b_2, \dots, b_n) $$
av vektorer i $V$ som både utspenner $V$ og er lineært uavhengige.

**Teorem 7.14.** La $V$ være et vektorrom med basis
$$ B = (b_1, b_2, \dots, b_n) $$
Da kan hver vektor $v$ i $V$ skrives som en lineærkombinasjon
$$ v = c_1b_1 + c_2b_2 + \cdots + c_nb_n $$
av basisvektorene i $B$, på en entydig måte.

**Definisjon.** Tallene $c_1, c_2, \dots, c_n$ i teorem 7.14 kalles *koordinatene* til vektoren $v$ *med hensyn på* basisen $B$. Vi definerer notasjonen $[\,v\,]_B$ for vektoren i $\mathbb{C}^n$ som består av koordinatene til v:
$$ [\,v\,]_B = \begin{bmatrix}
    c_1 \\ c_2 \\ \vdots \\ c_n
\end{bmatrix} $$
**Teorem 7.16.** La $V$ være et vektorrom med basis $B$. Koordinatene til en lineærkombinasjon av vektorer er tilsvarende lineærkombinasjonen av koordinatene til hver vektor:
$$ [\, c_1v_1 + c_2v_2 + \cdots + c_tv_t\,]_B = c_1 \cdot [\,v\,]_B + c_2 \cdot [\,v_2\,]_B + \cdots + c_t \cdot [\,v_t\,]_B $$
**Teorem 7.18.** La $V$ være et endeligdimensjonalt vektorrom. Da kan enhver endelig mengde som utspenner $V$ reduseres til en basis for $V$. Mer presist: Hvis $G$ er en endelig mengde av vektorer slik at $\text{Sp}\,G = V$, så finnes en delmengde $B \subseteq G$ slik at vektorene i $B$ utgjør en basis for $V$.

**Teorem 7.19.** Ethvert endeligdimensjonalt vektorrom har en basis.

**Teorem 7.20.** La $V$ være et endeligdimensjonalt vektorrom. Enhver endelig mengde av vektorer i $V$ som er lineært uavhengig kan utvides til en basis. Mer presist: Hvis $L$ er en endelig mengde av vektorer som er lineært uavhengige, så finees en basis for $V$ som inneholder alle vektorene i $L$.


### Dimensjon
**Teorem 7.21.** La $V$ være et vektorrom med en basis $B$ som består av $n$ vektorer. La $v_1, v_2, \dots, v_m$ være $m$ vektorer i $V$, der $m > n$. Da er disse vektorene lineært avhengige.

**Teorem 7.22.** La $V$ være et endeligdimensjonalt vektorrom. Da har enhver basis for $V$ samme størrelse.

**Definisjon.** La $V$ være et endeligdimensjonalt vektorrom. Vi definerer *dimensjonen* til $V$ som antall vektorer i en basis for $V$. Vi bruker notasjonen $\dim{V}$ for dimensjonen til $V$. Hvis $B$ er en basis for $V$, har vi altså
$$ \dim{V} = |B| $$

**Teorem 7.23.** La $V$ være et vektorrom med et underrom $U$. Hvis $V$ er endeligdimensjonalt, så er $U$ også endeligdimensjonalt, og
$$ \dim{U} \leq \dim{V} $$


### Vektorrom tilknyttet en matrise
**Nullrommet.** Vi definerer *nullrommet* til en reell $m \times n$-matrise $A$ som løsningsmengden til likningen $Ax = 0$, altså delmengden av $\mathbb{R}^n$:
$$ \text{Null}\,A = \{ x \in \mathbb{R}^n \,|\, Ax = 0 \} $$
**Kolonnerommet.** Vi definerer *kolonnerommet* til en reell $m \times n$-matrise
$$ A = [\, a_1 \ a_2 \ \cdots \ a_n \,] $$
som underrommet av $\mathbb{R}^m$ utspent av kolonnene i $A$:
$$ \text{Col}\,A = \text{Sp} \{\, a_1, a_2, \dots, a_n \,\} $$
Vi kan også beskrive kolonnerommet ved
$$ \text{Col}\,A = \{\, Av \,|\, v \in \mathbb{R}^n \,\} $$
Vi finner en basis for kolonnerommet ved:

-  Bruk gausseliminasjon for å finne trappeformmatrisen $A'$ som er radekvivalant til $A$.
-  Se på $A'$ for å finne ut hvilke av kolonnene i $A$ som er pivotkolonner.
-  Pivotkolonnene danner en basis for $\text{Col}\,A$.

**Radrommet.** Vi definerer *radrommet* til en reell $m \times n$-matrise
$$ A = \begin{bmatrix} r_1^\top \\ r_2^\top \\ \vdots \\ r_m^\top \end{bmatrix} $$
som underrommet av $\mathbb{R}^n$ utspent av radene i $A$:
$$ \text{Row}\,A = \text{Sp} \{\, r_1, r_2, \dots, r_m \,\} $$
Dette er det samme som kolonnerommet til den transponerte matrisen:
$$ \text{Row}\,A = \text{Col}\,A^\top $$
**Teorem 7.25} La $A$ være en $m \times n$-matrise, og la $E$ være trappeformmatrisen vi får når vi gausseliminerer $A$. Da har vi:

-  Dimensjonen til nullrommet til $A$ er lik antall frie variabler vi får når vi løser likningssystemet $Ax = 0$, altså antall kolonner uten pivotelementer i $E$.
-  Dimensjonen til kolonnerommet til $A$ er lik antall kolonner med pivotelementer i $E$.
-  Dimensjonen til radrommet til $A$ er lik antall rader som ikke er null i $E$.

**Teorem 7.26} La $A$ være en $m \times n$-matrise. Da har kolonnerommet og radommet til $A$ samme dimensjon. Dette kalles *rangen* til $A$.
$$ \text{dim Col}\,A = \text{dim Row}\,A = \text{rank}\,A$$
**Teorem 7.27} La $A$ være en $m \times n$-matrise. Da er
$$ \text{dim Null}\,A + \text{rank}\,A = n $$

