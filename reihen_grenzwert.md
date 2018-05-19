# Grenzwert von Reihen

## Berechnung mittels Teleskopsumme

$$ s_n = \sum_{k=1}^{\infty} \frac{1}{k(k+1)}   $$

Formt man die Partialsummen unter der Idee der Teleskopsumme um, sieht man, dass man (durch $$ +k-k $$ im Zähler) die n-te Partialsumme umschreiben kann zu:

$$ \frac{1}{k(k+1)} = \frac{1}{k} - \frac{1}{k+1}    $$

Damit ist

$$ s_n = 1 - \frac{1}{n+1}  $$

Also ist der Grenzwert der Reihe 1.

### Übung
Berechne die Grenzwerte der Reihe. Tipp: Binomische Formel.

<div class="aufgabe">
$$ s_n = \sum_{k=2}^{\infty} \frac{1}{k^2-1}   $$
<div class="loesung">$$ \frac{1}{k^2-1} = \frac{1}{k-1} + \frac{1}{k+1}  $$ . $$ s = \frac{3}{4}  $$
 </div></div>


## Grenzwert bei geometrischen Reihen

Die Idee der Teleskopsumme hilft auch bei den geometrischen Reihen:

$$ s_n \cdot (1-q) = \ldots = 1 - q^{n+1} $$

$$ \Rightarrow  \lim\limits_{n \to \infty}  s_n = \frac{1-q^{n+1}}{1-q} $$

Für $$ |q|< 1 $$ haben wir also den schönen Grenzwert

$$ s = \frac{1}{1-q}  $$

## Übungen

a) Berechne den Grenzwert der Reihe

$$ s_n = \sum_{k=0}^{\infty}\left(-\frac{1}{2}\right)^k   $$

b) Berechne $$ 0,999 \ldots $$  mittels Grenzzwertberechnung einer geometrischen Reihe. Tipp: $$ 0,999 \ldots = 9 \left( \frac{1}{10} \right) $$ 
