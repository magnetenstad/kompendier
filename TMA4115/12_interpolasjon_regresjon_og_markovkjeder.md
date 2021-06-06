
## Interpolasjon, regresjon og markovkjeder


### Minste kvadraters metode
**Definisjon.** Vi kaller $\hat{x}$ den *minste kvadraters løsning* for $Ax = b$.

**Teorem 12.1.** La $A$ være en $m \times n$-matrise og $b$ være en kolonne vektor i $\mathbb{R}^m$. Mengden av minste kkvadraters løsninger for systemet $Ax = b$ er lik løsningsmengden for systemet
$$ A^T(Ax-b)=0 $$
Hvis $n \times n$-matrisen $A^TA$ er inverterbar, finnes det for hver $b$, en unik minste kvadraters løsning $\hat{x}$ for systemet $Ax = b$.


### Interpolasjon og regresjon


### Markovkjeder
**Definisjon.** En *sannsynlighetsvektor* er en vektor $v$ i $\mathbb{R}^n$ der alle koordinatene er større eller lik $0$ og summen av koordinatene er lik $1$. En $n \times n$-matrise $M$ kalles en *stokastisk matrise* hvis kolonnene i $M$ er sannsynlighetsvektorer.

**Definisjon.** La $M$ være en stokastisk matrise og $x_0$ en sannsynlighetsvektor. Vi kalles følgen av vektorene
$$ \{\, x_n \,\} \text{ for } n = 0, 1, 2, \dots $$
en *Markovkjede.*

**Teorem 12.8.** En stokastisk matrise $M$ har alltid $\lambda = 1$ som egenverdi.

**Definisjon.** La $M$ være en stokastisk matrise. En egenvektor for $M$ som hører til egenverdi $1$ og er en sannsynlighetsvektor kalles en *likevektsvektor*.

**Definisjon.** En stokastisk matrise $M$ kalles *regulær* hvis det finnes en $k \geq 1$ slik at alle elementene i $M^k$ er større enn 0.

**Teorem 12.10.** La $M$ være en regulær stokastisk matrise. Da har $M$ en unik likevekstvektor $q$. For enhver utgangssannsynlighetsvektor $x_0$ konvergerer Markovkjeden $\{\, x_n \,\}$ til $q$ når $n \rightarrow \infty$.




