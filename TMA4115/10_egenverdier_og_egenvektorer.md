
## Egenverdier og egenvektorer


### Definisjon av egenverdier og egenvektorer
**Definisjon.** La $T: V \rightarrow V$ være en lineærtransformasjon. En skalar $\lambda$ er en *egenverdi* for $T$ hvis det finnes en vektor $v \neq 0$ i $V$ slik at
$$ T(v) = \lambda \cdot v $$
Vektoren $v$ kalles en *egenvektor* for $T$ som hører til egenverdien $\lambda$. Når $T$ er gitt ved en $n \times n$-matrise $A$, så sier vi også at $\lambda$ er en egenverdi for $A$ og $v$ er egenvektor for $A$ som hører til egenverdien $\lambda$.


### Noen generelle observasjoner
**Teorem 10.3.** Anta at $\lambda$ er en egenverdi for en lineærtransformasjon $T: V \rightarrow V$, og at $v$ er en tilhørende egenvektor. Da er alle multipletter $cv$ av vektoren $v$, der $c$ er et tall som ikke er $0$, også egenvektorer som hører til egenverdien $\lambda$. Med andre ord er alle vektorer i mengden $\text{Sp}\{v\}$, unntatt nullvektoren, egenvektorer som hører til egenverdien $\lambda$.

**Teorem 10.4.** En $n \times n$-matrise $A$ har $0$ som egenverdi hvis og bare hvis den ikke er inverterbar.

**Teorem 10.5.** La $T: V \rightarrow V$ være en lineærtransformasjon. La $v_1, v_2, \dots, v_t$ være egenvektorer til $T$ som hører til forskjellige egenverdier $\lambda_1, \lambda_2, \dots, \lambda_t$. Da er vektorene $v_1, v_2, \dots, v_t$ lineært uavhengige.

**Teorem 10.6.** La $V$ være et $n$-dimensjonalt vektorrom og $T: V \rightarrow V$ være en lineærtransforamsjon. Hvis $T$ har $n$ forskjellige egenverdier, så finnes det en basis for $V$ som består egenvektorer av $T$.


### Noen geometriske eksempler


### Hvordan finne egenverdier og egenvektorer?
**Teorem 10.9.** La $A$ være en $n \times n$-matrise.

-  Egenverdiene til $A$ er alle løsninger $\lambda$ av likningen
$$ \det{(A - \lambda I_n)} = 0 $$
-  Hvis $\lambda$ er en egenverdi for $A$, så er de tilhørende egenvektrene gitt ved alle ikke-trivielle løsninger av likningen
$$ (A - \lambda I_n ) \cdot x = 0 $$

**Definisjon.** En *diagonalmatrise* er en kvadratisk matrise der alle tall utenfor diagonalen er $0$.

**10.10.** Egenverdiene til en diagonalmatrise er tallene på diagonalen.


### Egenrom
**Definisjon.** La $T: V \rightarrow V$ være en lineærtransformasjon, og anta at $\lambda$ er en egenverdi for $T$. Da er *egenrommet* til $\lambda$ mengden av alle egenvektorer som hører til $\lambda$, samt nullvektoren; altså mengden
$$ \{\, v \in V \ | \ T(v) = \lambda v \, \} $$
Dimensjonen til egenrommet kalles den *geometriske multiplisiteten* til $\lambda$.


### Fremgangsmåte for å finne egenverdier og egenvektorer


### Eksistens av egenverdier
**Teorem 10.14.** En kompleks $n \times n$-matrise $A$ har alltid $n$ egenverdier (talt med algebraisk multiplisitet).

**Teorem 10.15.** For en lineærtransformasjon $T: \mathbb{R}^n \rightarrow \mathbb{R}^n$ er det mulig at den ikke har noen reelle egenverdier. Hvis $n$ er et oddetall, har $T$ minst én reell egenverdi.

**Teorem 10.16.** De komplekse egenverdiene til en reell matrise kommer i komlekskonjugerte par.

**Teorem 10.20.** Egenrommet har dimensjon større enn eller lik $1$ og mindre enn eller lik den algebraiske multiplisiteten til egenverdien.

