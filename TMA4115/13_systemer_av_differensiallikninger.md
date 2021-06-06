
## Systemer av differensiallikninger


### Vektorfunksjoner
**Teorem 13.5.** Den deriverte av en vektorfunksjon $y: \mathbb{R} \rightarrow \mathbb{R}^n$ er lik vektorfunksjonen gitt ved å derivere hver komponent
$$ y'(t) = \begin{bmatrix}
    y_1'(t) \\ y_2'(t) \\ \vdots \\ y_n'(t)
\end{bmatrix} $$


### Systemer av differensiallikninger
**Teorem 13.7.** (Superposisjonsprinsippet). Løsningene til
$$ y' = Ay $$
utgjør et vektorrom. Det vil si at dersom $y_1$ og $y_2$ er løsninger av systemet, så er $c_1y_1 + c_2y_2$ en løsning for alle reelle tall $c_1$ og $c_2$.


### Løsningsteknikk for reell diagonaliserbare matriser
**Teorem 13.8.** La $A$ være en diagonaliserbar $n \times n$-matrise. Hvis $v_1, v_2, \dots, v_n$ er $n$ lineært uavhengige egenvektorer med tilhørende egenverdier $\lambda_1, \lambda_2, \dots, \lambda_n$, så er
$$ v_1e^{\lambda_1t}, v_2e^{\lambda_2t}, \dots, v_ne^{\lambda_nt} $$
en basis for løsningesrommet til $y' = Ay$. Med andre ord er
$$ c_1v_1e^{\lambda_1t}, c_2v_2e^{\lambda_2t}, \dots, c_nv_ne^{\lambda_nt} $$
en generell løsning av $y' = Ay$.


### Initialverdiproblemer
**Definisjon.** Et *initialverdiproblem* er et system sammen med en intialbetingelse $y(t_0) = y_0$ hvor $t_0$ er et reelt tall og $y_0$ er en vektor i $\mathbb{R}^n$.


### Todimensjonale system
Vi begrenser oss nå til todimensjonale system. Det betyr at $A$ har en reell $2 \times 2$-matrise. Det er tre forskjellige tilfeller vi må skille mellom avhengig av hva slags egenverdier $A$ har. Husk at egenverdiene er røttene til det karakteristiske polynomet $\det{(A-\lambda I)}$.

#### Tilfelle 1: To forskjellige reelle røtter

#### Tilfelle 2: To komplekse (ikke reelle) røtter
**Teorem 13.16.** Anta at $\alpha + i \beta$, $\beta \neq 0$, er en kompleks egenverdi til $A$ og la $v$ være en tilhørende kompleks egenvektor. Da danner
$$y_1(t) = e^{\alpha t}(\text{Re}(v)\cos{(\beta t)} - \text{Im}(v)\sin{(\beta t)})$$
og 
$$y_2(t) = e^{\alpha t}(\text{Re}(v)\sin{(\beta t)} + \text{Im}(v)\cos{(\beta t)})$$
en basis for det reelle løsningsrommet til $y' = Ay$.

#### Tilfelle 3: Én reell rot
**Teorem 13.32.** La $A$ være en reell $2 \times 2$-matrise med reell egenverdi $\lambda$ med algebraisk multiplisitet 2. La $v$ være en egenvektor til $\lambda$ og la $w$ være en vektor som oppfyller $(A - \lambda I)w = v$. Da er løsningene til systemet $y' = Ay$ på formen $$ y(t) = c_1e^{\lambda t}v + c_2e^{\lambda t}(tv + w) $$


### Inhomogene system
**Teorem 13.24.** Hvis $y_p(t)$ er en partikulær løsning av
$$ y'(t) = Ay(t) + f(t) $$
så er en generell løsning gitt av
$$ y(t) = y_h(t) + y_p(t) $$
hvor $y_h(t)$ er en generell løsning av den tilhørende homogene likningen.

**Merk.** Det forventes ikke at du kan finne partikulære løsninger av vilkårlige system. Du vil alltid få dem servert.


