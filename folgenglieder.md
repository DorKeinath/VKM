# Folgen

Eine Folge ist eine Liste, also eine Objekt, das aus mehreren Objekten besteht, die durchnummeriert werden können. Zum Beispiel sind Koordinaten und Tripel (endliche) Folgen. Eine Folge mit n Gliedern nennt man auch **n-Tupel**.
Wir definieren $$ n \in \mathbb{N} $$ und nehmen auch die $$ 0 $$ dazu.

## Explizite und rekursive Darstellung

Man kann nicht nur (was sich aber immer empfiehlt!) die Anfangsglieder aufschreiben bzw. ausrechnen, sondern versuchen Darstellungsformen zu finden, die alle, also interessanterweise unendlich viele, Folgenglieder beschreibt.

Schön wäre es, wenn man immer eine **explizite Darstellung**, eine Funktionsvorschrift, ein Bildungsgesetz, hätte z.B.

$$ a_n = 2n $$

> Wie lautet die explizite Darstellung der ungeraden Zahlen?

> Wie lautet die explizite Darstellung der Folge  $$ 1, 2, 4, 8,... $$ ?

[Lösung](https://oeis.org/search?q=1%2C2%2C4%2C8&sort=&language=german&go=Suche)

> Wie lautet die Darstellung der Folge  $$ 3, 8, 13,18,23 $$ ?

[Lösung](https://oeis.org/search?q=+3%2C8%2C13%2C18%2C23+&sort=&language=german&go=Suche)

Die andere Darstellungsform nennt man **rekursiv**, von lat. 'recurrere' *zurücklaufen*.

> Wie lauten die rekursiven Darstellungen der obigen Folgen?

## Folgen mit Namen

Ist die Differenz zwischen zwei aufeinander folgenden Gliedern konstant, spricht man von einer **arithmetischen** Folge.

Ist der Quotient zwischen zwei aufeinander folgenden Gliedern konstant, spricht man von einer **geometrischen** Folge.

## Übungen mit Python
### Aufgabe 1
Berechne die Folgenglieder (sofern das in endlicher Zeit möglich ist) für $$ n=0,1,2,3,4,5,10, 100, 1000, 100000, 100001 $$ (die zu zeitintensiven kannst du überspringen).

1. $$ a_n = \frac{1}{n}  $$

1. $$ a_n = 2 ( \frac{1}{3} )^n  $$

1. $$ a_n = \frac{n}{2n+1}  $$

1. $$ a_n = (-2)^n $$

1. <div class="aufgabe">$$ a_n = \sqrt{n+1}- \sqrt{n-1} $$<div class="loesung">Lösung mit Grenzwertsätzen: Zähler und Nenner mit Wurzel + Wurzel multiplizieren, ergibt, dass es eine Nullfolge ist. </div></div>

1. <div class="aufgabe">$$ a_n = \sqrt[n]{n} $$<div class="loesung">Lösung: Geht gegen 1.</div></div>

1. <div class="aufgabe">$$ a_n = \sqrt[n]{n!} $$<div class="loesung">Lösung: Geht gegen unendlich.</div></div>

1. <div class="aufgabe">$$ a_{n+1}=\frac{1}{2} (a_n + \frac{2}{a_n} )$$<div class="loesung">Lösung: Der Grenzwert ist $$\sqrt{2}$$. Dahinter steckt das Heron-Verfahren, weshalb man von der Newton-Heron-Folge spricht, siehe S. 79 Beispiel 4.22 </div></div>

1. $$ a_n = (1+\frac{1}{n} )^n $$

1. $$ a_n = \frac{n}{\sqrt[n]{n!}}  $$

1. <div class="aufgabe">$$ a_n = \frac{n}{2n+1} + \sqrt[n]{n} $$ <div class="loesung">Lösung: Geht gegen $$0 ,5+1 $$ </div></div>

1. $$ a_n = \frac{3n^2 + n + 2}{4n^2+6}  $$

> <div class="aufgabe">Kommt dir das jeweils größte berechnete Folgenglied der Folgen 9. und 10. bekannt vor?<div class="loesung">Den Grenzwert der Folgen nennt man e. </div></div>

### Aufgabe 2
Überprüfe deine Ergebnisse, indem du die Folge mit Python programmierst und damit deine Folgenglieder berechnen lässt. Dazu kannst du z.B. in eine Datei namens *folge.py* den folgenden Code schreiben und im Terminal mit `python folge.py` das Programm starten.

```python
#!/usr/bin/env python3
# -*- coding: utf-8 -*-

# Es wird im Terminal angezeigt, was gegeben ist:
print('Es ist a_n = 2n')
# Der folgende Algoritmus wird unendlich oft durgeführt.
while True:
    # Es wird eine Tastatureingabe abgefragt:
    n = input('Welches n willst du berechnen? ')
    # Das entsprechende Folgenglied wird mittels Funktionsvorschrift ausgerechnet:
    a_n = 2*n
    # Das Ergebnis wird im Terminal angezeigt:
    print('a_' + str(n) + ' = ' + str(a_n))
```

Für die Funktionsvorschriften kannst die folgenden Codes verwenden:

```python
# Für's Teilen kannst du in der dritten Zeile mit der folgenden
#  Zeile ein Paket importieren, oder eine dezimale 0 verwenden.
from __future__ import division
# Für die Quadratwurzel kann man auch ein Paket importieren oder einfach mit einem
#  Bruch potenzieren, wobei der Nenner eine dezimale 0 dabei haben sollte.
from math import sqrt
# Für die Fakultät kann man das folgende Paket importieren:
from math import factorial

2.0/3 # bedeutet 2/3 und ist 0,66666.
2**3  # bedeutet 2^3, ist also 8.
4**(1/2.0) # bedeutet 4^(1/2), also die Wurzel von 4, ist also 2.
sqrt(4) # bedeutet die Quadratwurzel von 4, ist also 2.
factorial(6) # bedeutet 6!
```

Falls du die ersten zehn Folgenglieder auf einmal berechnen lassen willst, kannst du auch eine for-Schleife verwenden:

```python
for n in range(10):
    a_n = n + 1
    print(a_n)
```
Das `range(10)` ist dabei die Liste der natürlichen Zahlen von 0 bis 9, also $$ [0,1,2,3,4,5,6,7,8,9] $$.

### Aufgabe 3
Schreibe eine rekursive Version der Funktion $$ f(n)=3 \cdot n $$.

Zum Beispiel kann man die Folge $$ a_n = 2n $$ rekursiv als $$ a_n = a_{n-1} + 2 $$ und mit dem Anfangswert $$ a_0 = 0 $$  definieren. Als Python-Code sieht das z.B. so aus:

```python
def folge(n):
    if n == 0:
        return 0
    else:
        return folge(n-1) + 2
f = input('Wie viele Folgenglieder sollen berechnet werden? ')
# range(f) ist die Liste der natürlichen Zahlen von 0 bis f-1:
for i in range(f):
    print(folge(i))
```

Weiteres Beispiel: Die Ergebnisse der Fakultätsfunktion lassen sich so berechnen:

```python
def fakultaet(n):
    if n == 1:
        print(str(n))
        return 1
    else:
        print(str(n))
        return n * fakultaet(n-1)

f = input('f ')
print('Ergebnis: ' + str(fakultaet(f)))
```

### Aufgabe 4
Versuche, die bisher verwendeten Folgen als rekursive Funktionen zu programmieren.

### Aufgabe 5
Schreibe ein Programm für die Fibonacci-Folge.

$$ a_n = a_{n-1} + a_{n-2} $$
$$ a_0=0 $$
$$ a_1=1 $$

[Lösungen](https://stackoverflow.com/questions/494594/how-to-write-the-fibonacci-sequence)

### Aufgabe 6
Falls du ehrgeizig bist, schreibe jeweils ein Programm für die Zahlen im Pascalschen Dreieck, und für die Folge der Primzahlen ([Sieb des Eratosthenes](https://de.wikipedia.org/wiki/Sieb_des_Eratosthenes)).

[Lösungen](https://www.python-kurs.eu/python3_rekursive_funktionen.php)
