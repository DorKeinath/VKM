# Grenzwertsätze

## EA: Grenzwertsätze abschreiben
S. 69 Satz 4.2

## Beispiel
Wir versuchen, die Sätze auf die folgende Folge anzuwenden:

$$ a_{n+1} = 2a_n +  3$$

Zunächst berechnen wir ein paar der ersten Folgenglieder.
Dann bestimmen wir mit den Grenzwertsätzen den Grenzwert der Folge. Wenn wir den Grenzwert $$ a $$ nennen, gilt:
$$ a = \lim\limits_{n \to \infty} a_{n+1} = ... $$

> Was folgern wir also?

<div class="aufgabe"> Lösung <div class="loesung">Wir folgern, dass es extrem wichtig ist, vor der Anwendung der Grenzwertsätze sicher zu gehen, dass die Voraussetzungen erfüllt sind, nämlich <i>dass</i> die Folgen konvergieren. Mit den Grenzwertsätzen berechnen wir dann, <i>welchen</i> Grenzwert die Folge hat.</div></div>

## 3 Wege
Ich kenne drei Wege zur Berechnung von Grenzwerten mittels Grenzwertsätzen. Ohne Grenzwertsätze verwendet man *Weierstraß* (was wir in den nächsten Stunden behandeln werden).

$$ a_n = \frac{2n+1}{n+1} $$

Um die Voraussetzung zu erfüllen, könnten wir zeigen, dass die Folge monoton steigend und begrenzt ist. Das holen wir in den nächsten Stunden nach. Wir glauben das erst mal, indem wir ein paar der ersten Folgenglied berechnen. Jetzt können wir Grenzwertsätze anwenden.

### Polynomdivision
$$ (2n+1):(n+1) = 2 R {-1} $$
$$ \Rightarrow  a_n = 2 - \frac{1}{n+1} $$
Jetzt können wir leicht den Limes gegen Unendlich betrachten.

### Ausklammern
$$ \frac{2n+1}{n+1} = \frac{n(2+\frac{1}{n})}{n(1+\frac{1}{n} )} = \frac{2+\frac{1}{n} }{1+\frac{1}{n} } $$
Und das geht, wie man denkt zu wissen, und was wir nächste Stunde zeigen werden, gegen 2.
Im ersten Schritt müssen wir annehmen, dass $$ n \ne 0 $$  ist.
### De l'Hospital
$$ \lim\limits_{n \to \infty} \frac{f(n)}{g(n)} = \lim\limits_{n \to \infty} \frac{f'(n)}{g'(n)}  = \frac{2+0}{1+0} = 2$$
Im ersten Schritt gehen wir davon aus, dass beide Funktionen monoton steigend sind.

Man versuche sich, um die Relevanz von De l'Hospital bewusst zu werden, an der Folge $$ a_n = \frac{\ln(n)}{\sqrt{n}}  $$ .

## Übungen
*Handout: Repetitorium S. 330+331*

1. Berechne, wenn möglich, mit Hilfe der Grenzwertsätze die Grenzwerte aus der [Aufgabe 1 aus der letzten Stunde](folgenglieder.md).
2. $$ \frac{4n^9 + 2n^3}{4n^{10} + 2 n^3}  $$
3. <div class="aufgabe">$$ \frac{(n^2+4n)(n^3-2n^2)}{(5+n)(n^4-1)}  $$ <div class="loesung">Lösung: Geht gegen 1. </div></div>
4. <div class="aufgabe">$$ \frac{2^n-3^n}{2^n+3^n} $$ <div class="loesung">Tipp: Schau dir erst die nächste Aufgabe an. Lösung: 1.</div></div>
5. <div class="aufgabe">$$ \frac{3^n}{2^n+2 \cdot 3^n}$$ <div class="loesung">Lösung: Den höchsten Summanden, hier den Zähler, auch im Nenner ausklammern... $$ \frac{1}{2} $$.</div></div>
6. <div class="aufgabe">$$ \sqrt{n^2+4n}-\sqrt{n^2+n} $$ <div class="loesung">Tipp: Da steht $$a-b$$ und man kann das zu einem Bruch mittels einer bekannten Formel so erweitern, dass die Wurzeln durch Quadrate wegfallen. Lösung: $$\frac{3}{2} $$ </div></div>
7. <div class="aufgabe">$$ a_{n+1} = \frac{1}{2}(a_n + \frac{5}{a_n} )  $$<div class="loesung">Tipp: Wenn der Grenzwert von $$a_n = a$$ ist, dann ist der von $$a_{n+1}$$? So, und jetzt in die Aufgabe 1 aus der letzten Stunde schauen. Lösung: $$ \sqrt{5} $$.  </div></div>

<!-- LS 262 -->
