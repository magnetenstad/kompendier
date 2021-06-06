
## Lineær uavhengighet


### Lineært spenn: overflødige vektorer
Dersom en vektor $u$ ikke utvider spennet til en mengde vektorer $v_1, \cdots, v_n$ så er vektorene $u, v_1, \cdots, v_n$ lineært avhengige.


### Lineær uavhengighet i $R^3$


### Definisjon av lineær uavhengighet
**Definisjon.** Vektorene $v_1, v_2, \cdots, v_n$ er lineært uavhengige dersom likningen
$$ x_1 v_1 + x_2 v_2 + \cdots + x_n v_n = 0 $$
ikke har andre løsninger enn den trivielle løsningen $x_1 = x_2 = \cdots = x_n = 0$. I motsatt tilfelle kalles de lineært avhengige.


### Lineær uavhengighet for to vektorer
**Teorem 5.6.** To vektorer $u$ og $v$, begge ulik $0$, er lineært uavhengige hvis og bare hvis $u \neq cv$, for en skalar $c \neq 0$.


### Hvordan sjekke lineær uavhengighet?
**Teorem 5.8.** La $A$ være en matrise. Følgende påstander er ekvivalente:

-  Kolonnene i $A$ er lineært uavhengige.
-  Likningen $Ax = 0$ har bare den trivielle løsningen $x = 0$.
-  Vi får ingen frie variabler når vi løser $Ax = 0$.
-  Når vi gausseliminerer $A$, får vi et pivotelement i hver kolonne.

Teorem 5.8 gir oss en grei metode for å sjekke lineær uavhengighet. Hvis vi har vektorer
$$ v_1, v_2, \dots, v_n $$
kan vi finne ut om de er lineært uavhengige på denne måten:

-  Lag en matrise $A = [ \ v_1 \ v_2 \ \dots \ v_n \ ]$ med disse vektorene som kolonner.
-  Gausseliminer $A$ til trappeform.
-  Hvis hver kolonne inneholder et pivotelement, er vektorene lineært uavhengige. Ellers er de lineært avhengige.

**Teorem 5.12.** Gitt $n$ vektorer $v_1, v_2, \dots, v_n$ i $\mathbb{R}^m$ eller $\mathbb{C}^m$. Hvis 
 -  en av vektorene er en lineærkombinasjon av de andre, eller
 -  $n > m$,

så er vektorene lineært avhengige.

**Teorem 5.13.** Vektorene $v_1, v_2, \dots, v_n$ er lineært uavhengige hvis og bare hvis ingen av dem kan skrives som en lineærkombinasjon av de andre.


### Like mange vektorer som dimensjonen
**Teorem 5.14.** Hvis vi har $n$ vektorer $v_1, v_2, \dots, v_n$ i $\mathbb{R}^n$, så er de lineært uavhengige hvis og bare hvis de utspenner hele $\mathbb{R}^n$, altså hvis og bare hvis
$$\text{Sp}\{v_1, v_2, \dots, v_n \} = \mathbb{R}^n $$



