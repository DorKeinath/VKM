# Besondere Folgen

Die Schüler erarbeiten in Partnerarbeit eine Präsentation zu einem der folgenden Themen

* Heron-Verfahren (inkl. [Veranschaulichung](https://de.wikipedia.org/wiki/Heron-Verfahren#Geometrische_Veranschaulichung_des_Heron-Verfahrens))
* Newton-Verfahren [https://de.wikipedia.org/wiki/Newton-Verfahren](https://de.wikipedia.org/wiki/Newton-Verfahren)
* Geometrische Folge (inkl. geometrisches Mittel)
* Arithmetische Folge (inkl. arithmetisches Mittel) [https://de.wikipedia.org/wiki/Arithmetische_Folge](https://de.wikipedia.org/wiki/Arithmetische_Folge)

## Heron-Verfahren
(Siehe Glosauer S. 79 Beispiel 4.22 )

$$ a_1 = 1; \quad a_{n+1}=\frac{1}{2} \left(a_n + \frac{2}{a_n} \right)$$

Der Grenzwert ist $$ \sqrt{2} $$.

Dahinter steckt das Heron-Verfahren, weshalb man von der **Newton-Heron-Folge** spricht. ("Newton" deswegen, weil das Heron-Verfahren auf dem Newton-Verfahren beruht.)

[Veranschaulichung](https://de.wikipedia.org/wiki/Heron-Verfahren#Geometrische_Veranschaulichung_des_Heron-Verfahrens) von $$ \sqrt{9} $$.

> Zeigen Sie, dass die Folge (ab $$ n=2 $$) streng monoton fällt.

1. Wir wenden die Definition der Monotonie an.
2. Nach der Vereinfachung der Differenz bleibt ein Bruch.
3. Der Nenner des Bruchs ist $$ > 0 $$ (Vollständige Induktion).
4. Der Zähler des Bruchs ist $$ < 0 $$ (Bin1, Ausklammern, Bin2).

> Zeigen Sie, dass aus der Annahme, dass der Limes der Folge $$a$$ ist, $$ a = \sqrt{2} $$ folgt, indem Sie die Definition der Folge betrachten.

## Geometrische Folge

$$ a_n = q^n $$ nennt man **geometrische Folge**.

Für $$ |q|<1 $$ ist es eine *Nullfolge*.

Für $$ |q|>1 $$ ist sie *divergent*.

Beweis mit *Weierstraß* (Glosauer S. 63 Bsp. 4.2, S. 64 Bsp. 4.5 und S. 66 Bsp. 4.7).

### Zinseszinsfolge

$$ B_1 = B_0 + \frac{p}{100} \cdot B_0 = B_0(1+\frac{p}{100} )  $$

$$ B_2 = B_1(1+\frac{p}{100} ) =B_0(1+\frac{p}{100} )^2 $$

...

$$ B_n = B_0 (1+\frac{p}{100})^n $$

Das ist eine geometrische Folge mit $$ q = 1+\frac{p}{100} $$

> Ist die Zinseszeinsfolge eine Nullfolge oder divergent?

### Bemerkungen
Manchmal sieht man auch die Definition $$ a_n = a_0 \cdot q^n $$.

Die rekursive Darstellung ist $$ a_{n+1} = a_n \cdot q $$

## Harmonische Folge


## Arithmetische Folge

### Bemerkungen
$$ a_{n+1} = a_n + d $$

Jedes Folgenglied ist **arithmetisches Mittel** seiner Nachbarglieder:

$$ a_n = \frac{a_{n+1}+a_{n-1}}{2}  $$
