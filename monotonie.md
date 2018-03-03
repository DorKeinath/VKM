# Monotonie von Folgen

## Definition

Eine Folge heißt monton wachsend (fallend), wenn für alle Folgenglieder gilt: $$ a_{n+1} \geq a_n $$ ($$ a_{n+1} \leq a_n $$). Bei *streng* monoton sind strenge Ungleichzeichen gemeint.

## Beweise mittels Definition
Stellen Sie eine Vermutung bezüglich des Monotonieverhaltens der Folge auf und beweisen Sie sie mittels der Definition.

1. <div class="aufgabe">$$ a_n = \frac{1}{n} $$ <div class="loesung">Lösung: monoton fallend </div></div>
2. <div class="aufgabe">$$ a_n = \frac{8n}{n^2+1} $$ <div class="loesung">Lösung: monoton fallend </div></div>
3. <div class="aufgabe">$$ a_n = \frac{10n -7}{5+2n} $$ <div class="loesung">Lösung: monoton wachsend </div></div>
4. <div class="aufgabe"> $$ a_n = \frac{2+n}{2n+3} $$ <div class="loesung">Lösung: monoton fallend </div></div>
5. <div class="aufgabe"> $$ a_n = \frac{2n+1}{n+1}  $$ <div class="loesung">Lösung: monoton wachsend </div></div>
6. <div class="aufgabe"> $$ a_{n+1} = \frac{1}{4} a_n^2+1, \; a_1 = 1 $$ <div class="loesung">Lösung: Siehe Glosauer Beispiel 4.20, S. 79</div></div>

## Beweise mittels Induktion

### $$ a_{n+1} = \sqrt{5 a_n},\quad a_1 = 1 $$

zz: $$ a_n $$ wächst monoton

IA: $$ a_2 = \sqrt{5} > 1 = a_1 $$.

IV: $$ a_{n+1} > a_n $$

IS, $$ n \rightarrow n+1 $$: $$ a_{n+2} = \sqrt{5a_{n+1}} \stackrel{\textsf{IV}}{\geq} \sqrt{5a_n} = a_{n+1} $$

### Übungen
1. <div class="aufgabe">$$ a_1 = 1,\; a_{n+1} = \sqrt{1 + a_n} $$ <div class="loesung">Lösung: Monoton wachsend. $$a_{n+1} = \sqrt{a_n + 1} \stackrel{\textsf{IV}}{<} \sqrt{a_{n+1}+1} = a_{n+2}$$ </div></div>
2. Sehr schwierig: $$ a_n = (1+\frac{1}{n})^n $$ ist streng monoton wachsend. Tipp: Man braucht die Bernoulli-Ungleichung $$ (1+x)^n > 1+nx\; \text{(für}\; x \geq -1\text{)} $$
