
## Komplekse tall


### Den imaginære enheten
Vi definerer den imaginære enheten $i$, ved
$$ i^2 = -1 $$
Merk at $ \sqrt{ab} = \sqrt{a} \, \sqrt{b} $ bare gjelder for $a, b > 0$.

Komplekse tall er tall på formen
$$ z = a + bi $$
der $a, b \in \mathbb{R}$, og $i$ er den imaginære enheten.

Mengden av komplekse tall er $\mathbb{C}$.


### Operasjoner på komplekse tall
Regneregler for komplekse tall følger regnereglene for reelle tall.


#### Konjugat
La $z = a + bi$ være et komplekst tall. Da er $z$ *konjugert* gitt ved
$$ z = a - bi $$
Merk at $z\overline{z} = a^2 + b^2$ er et reelt tall.


### Polare koordinater
Polarkoordinater er nyttige når en multipliserer og tar potenser av komplekse tall.

La $r$ være avstanden fra det komplekse tallet $z =
a + bi$ til origo, og la $\theta$ være vinkelen $z$ gjør med den reelle aksen. Da har vi at
$$ \begin{gather*}
    a = Re \, z = r \, \cos{\theta} \\
    b = Im \, z = r \, \sin{\theta}
\end{gather*} $$
$r$ kalles *modulus} eller *absoluttverdi} til $z$ og $\theta$ kalles *vinkelen} eller *argumentet} til $z$.
$$ \begin{gather*}
    r = |z| = \sqrt{a^2 + b^2} = \sqrt{z\overline{z}} \\
    \theta =
    \begin{cases}
        \arctan \frac{b}{a} & \text{for } a > 0 \\
        \arctan \frac{b}{a} + \pi & \text{for } a < 0 \\
        \pi / 2 & \text{for } a = 0, \, b > 0 \\
        3\pi / 2 & \text{for } a = 0, \, b < 0 
    \end{cases}
\end{gather*} $$


#### Trekantulikheten
La $z$ og $w$ være komplekse tall. Da gjelder at
$$ |z + w| \leq |z| + |w| $$


### Eulers formel
Eulers formel er gitt ved
$$ e^{ix} = \cos{x} + i \, \sin{x} $$
der $x \in \mathbb{R}$ og $i$ er den imaginære enheten.

Det følger at
$$ z = r(\cos{\theta} + i \, \sin{\theta}) = re^{i\theta} $$


### Røtter av komplekse tall
Et polynom $f(z) = z^n + a_{z-1}z^{n-1} + ... + a_1<+a_0$, $z \in \mathbb{C}$ kan alltid faktoriseres
$$f(z) = \prod_{i=1}^n (z - z_i)$$
der $z_i \in \mathbb{C}$ er løsninger av likningen $f(z) = 0$.



