
## Lineære likningssystemer og gausseliminasjon


### Ekvivalente systemer
Vi sier at to ligningssystemer er ekvivalente dersom
de har samme løsningsmengder.


### Totalmatrisen til et system
Et lineært likningssystem med $m$ likninger og $n$ ukjente beskrives av en matrise. Denne kalles *totalmatrisen* eller *den utvidede matrisen* til likningssystemet. Vi lar gjerne en vertikal linje i matrisen skille venstre og høyre del av likningene.


### Radoperasjoner
Følgende tre måter å endre en matrise på kalles *radoperasjoner*:
- Gange alle tallene i en rad med det samme tallet. Dette betyr å gange en ligning med et tall. Vi kan ikke gange med 0.
-  Legge til et multiplum av en rad i en annen. Dette er å kombinere ligninger til nye ligninger.
-  Bytte rekkefølge på radene. Dette er det samme som å bytte rekkefølge på ligningene.
Vi sier at to matriser er radekvivalente hvis vi kan komme fra den ene til den andre ved å utføre en eller flere radoperasjoner. Vi bruker notasjonen $M \sim N$ for å si at to matriser $M$ og $N$ er radekvivalente.


### Trappeform, redusert trappeform og pivotelementer
**Definisjon.** Tallet lengst til venstre i en rad som ikke er $0$ kalles pivotelementet for den raden. (En rad med bare nuller har ikke noe pivotelement.)

**Definisjon.** En matrise er på trappeform dersom det ikke er annet enn $0$-ere under hvert pivotelement, og eventuelle nullrader er helt nederst.

**Definisjon.** En matrise er på redusert trappeform hvis den er på trappeform, pivotelementene er $1$ og alle tall som står over pivotelementer er $0$.


### Eksistens, entydighet og parametrisering av løsninger
For ethvert lineært ligningssystem må ett av de følgende punktene være sant:

-  Systemet har ingen løsning: Dette skjer når vi i redusert trappeform har en rad av typen $ 0 \ 0 \ ... \ 0 \ | \ b $ der $b \neq 0$.
-  Systemet har entydig løsning. Dette skjer når trappeform av totalmatrisen har pivotelement i alle kolonner unntatt den siste.
-  Systemet har uendelig mange løsninger. Dette skjer når vi får frie variabler. Vi får en fri variabel for hver kolonne (unntatt den siste) som ikke har pivotelement.



### Valgfrihet ved gausseliminasjon


### Lineære likninger med komplekse tall
Et lineært likningssett med komplekse koeffisienter og løsning, kan løses med gausseliminasjon på samme måte som i det reelle tilfellet.



