# Reihen

## Definition
Eine Reihe ist eine Folge, deren Glieder aus den Summen von Folgengliedern besteht. Das n-te Glied einer Reihe, also die Summe der ersten n Summanden nennt man auch n-te *Partialsumme*, sie sieht also so aus:

$$ s_n = \sum_{k=1}^n a_k $$

Die Glieder einer Reihe sind also Partialsummen.

Die unendliche Summe

$$ \sum_{k=1}^{\infty} a_k $$

wird für zweierlei verwendet

1. als Bezeichnung der Reihe (also als Folge der Partialsummen) $$ s_n = \sum_{k=1}^{\infty} a_k $$

2. als Grenzwert $$ s $$ der Reihe: $$ \sum_{k=1}^{\infty} a_k = \lim\limits_{n \to \infty} s_n = \lim\limits_{n \to \infty} \sum_{k=1}^{n} a_k = s $$


## Geometrische Reihe

$$ s_n = \sum_{k=0}^{\infty} q^k  \quad , \; q \neq 1$$

z.B.

$$ s_n = \sum_{k=0}^{\infty} 2^k = 1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8} + \ldots $$
also
$$ s_0 = 1, \quad s_1 = \frac{3}{2}, \; \ldots  $$

Diese geometrische Reihe konvertiert gegen 2 (d.i. die Lösung des Paradoxons von Zenon).

Die Summe mit den $$ \ldots $$ deutet nur an, wie die Summanden der Partialsummen aussehen. Besser wäre es vielleicht, Kommas zu verwenden, aber das habe ich noch nie gesehen:

$$ \sum_{k=0}^{\infty} 2^k = \sum 1 , \frac{1}{2} , \frac{1}{4} , \frac{1}{8} , \ldots $$

Die geometrische Reihe

$$ s_n = \sum_{k=0}^{\infty} (-1)^k $$

konvergiert nicht, sondern hat zwei Häufungspunkte: bei 0 und 1.

## Arithmetische Reihen

Bei Reihen, deren Partialsummen aus einer arithmetischen Folge entstehen, spricht man von arithmetischen Reihen.

Das schöne ist bei ihnen, dass sich die Partialsummen direkt berechnen lassen, weil der Abstand zweier aufeinander folgender Glieder konstant ist, also z.B. mit Abstand $$d$$: $$ a_k = a_0 + kd $$ .

Die *Gaußsche Summenformel*, auch *der kleine Gauß* genannt, ist eine Darstellung der n-ten Partialsumme der einfachsten arithmetischen Reihe:

$$ \sum_{k=1}^{n} k = 1+2+3+ \ldots + n = \frac{n(n+1)}{2}  $$


### Übung
Berechne den Grenzwert der Reihe

$$ s_n = \frac{\sum_{k=1}^{\infty} k}{n^2}  $$


## Harmonische Reihe

$$ s_n = \sum_{k=1}^{\infty} \frac{1}{k}  $$

Obwohl die harmonische Folge eine Nullfolge ist, divergiert die harmonische Reihe.

[Mehr zur harmonischen Reihe auf Wikipedia](https://de.wikipedia.org/wiki/Harmonische_Reihe)
