# Bruchgleichungen

## PL: Def und zwei Beispiele

Def.: Eine Bruchgleichung ist eine Gleichung, in der eine Variable im Nenner steht.

Die folgenden Beispiele in zwei Spalten aufschreiben. Beim leichten Beispiel Platz für Ergänzungen lassen.

### Beispiel (leicht)

$$ \frac{x}{2} = \frac{7}{4} + \frac{1}{x}  $$

### Beispiel (schwer)

$$ \frac{1}{x-1} + \frac{1}{x+1} - \frac{1}{x^2-1} = 1 $$

Wir verwenden (ungeschickterweise) als Hauptnenner $$ (x+1)(x-1)(x^2-1) $$ .

[Lösungen der entstehenden Gleichung](http://www.wolframalpha.com/input/?i=(x%2B1%29(x%5E2-1%29%2B(x-1%29(x%5E2-1%29-(x%2B1%29(x-1%29%3D(x%2B1%29(x-1%29(x%5E2-1%29)

<!-- Für die Verlinkung die Klammer zu ) durch %29 ersetzen. -->

> Finde das Problem!

[Lösung der Bruchgleichung](https://www.wolframalpha.com/input/?i=1%2F(x-1%29%2B1%2F(x%2B1%29-1%2F(x%5E2-1%29+%3D+1)

#### Bemerkung

Das Quadrieren ist keine Äquivalenzumformung.
$$ -2 = 2  \Rightarrow \mathbb{L} = \{ \} $$

> Welche Lösungsmenge hat die quadrierte Gleichung?

### Verfahren

1. Definitionsmenge aufschreiben.
2. Nenner von Variable befreien durch Multiplikation mit dem Hauptnenner.
3. Die entstehende Gleichung lösen.
4. Überprüfen, ob die gefundenen Lösungen in der Definitionsmenge (siehe 1.) sind.

#### Tricks

Trick zum *Finden eines kleinen Hauptnenners*: Alle Nenner faktorisieren, z.B. mit Bin 3 oder wie in der vorletzten Stunde.

Beispiel: $$ \frac{1}{x^3-4x} = \frac{1}{x(x-2)(x+2)}  $$

Trick zum *Anpassen der Produkte*: Zähler und Nenner mit $$ -1 $$  multiplizieren.

$$ \frac{1}{a-b} = \frac{-1}{-(a-b)} = \frac{-1}{b-a}   $$

## PA: Übungen

* Buch Beispiel 7.9 b)
* Buch Aufgabe 7.4 a)
* <div class="aufgabe"> $$ \frac{x-6}{x^2-x} + \frac{5}{x-1} = \frac{5}{x} $$ <div class="loesung"> Lösung: $$ \mathbb{L} = \{ \} $$ </div></div>
* <div class="aufgabe"> $$ \frac{1}{x-3} - \frac{1}{x+4} = \frac{7}{x^2+x-12} $$ <div class="loesung"> Lösung: $$ \mathbb{L} = \mathbb{R} \backslash \{-4;3 \} $$ </div></div>
* <div class="aufgabe"> $$ \frac{3}{x-1} \leq 1 $$ (Vorübung für die nächste Stunde) <div class="loesung">Lösung: Siehe Buch Beispiel 7.10 </div></div>



# Bruchungleichungen
## PL Obige Übung als Ungleichung
$$ \frac{x-6}{x^2-x} + \frac{5}{x-1} > \frac{5}{x} $$

Im 1. Fall dürfen wollen wir die Ungleichung multiplizieren, ohne das Zeichen umzudrehen. Das dürfen wir wenn $$ x(x-1)>0 $$
$$ \Leftrightarrow (x>0  \wedge x>1) \vee (x<0 \wedge x<1)$$
$$ \Leftrightarrow x>1 \vee x<0 $$
Fassen wir die Terme zusammen und lösen nach x auf, ergibt sich $$ x>1 $$.

Insgesamt gilt für x also $$ (x>1 \vee x<0) \wedge x>1 $$, und damit ergibt sich für diesen Fall also $$ \mathbb{L_1} = (1;\infty) $$.

Beim 2. Fall bleibt $$ 0 < x < 1 $$ übrig und $$ x<1 $$. Also  $$ \mathbb{L_2} = (0,1) $$.

 Insgesamt also $$ \mathbb{L} = \mathbb{R}^{+} \backslash \{1 \} $$ .

### Bemerkung
Die Lösungsmenge darf mit Hilfe des **Zahlenstrahls** markiert werden.

## PA: Übungen

* $$ \frac{4}{x} + \frac{1}{2-x} < \frac{1}{x(x-2)}  $$. [Lösung](https://www.wolframalpha.com/input/?i=4%2Fx%2B1%2F(2-x%29%3C1%2F(x(x-2%29%29)
* Handout "Bruchungleichungen"
* Buch Beispiele 7.10 b) + 7.11 + 7.12
* Buch Aufgabe 7.5
