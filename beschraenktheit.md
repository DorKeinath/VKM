# Beschränktheit

## Definitionen
$$ a_n $$ beschränkt $$ \Leftrightarrow \exists s,S: s \leq a_n \leq S $$

Supremum = Kleinste obere Schranke

Infimum = Größte untere Schranke

## Bemerkung

Beschränkte Folgen habe nicht notwendig einen Grenzwert. Beweis:

$$ a_n = (-1)^n \frac{2+n}{2n+3}  $$ hat zwei Häufungspunkte: $$ \frac{1}{2} , -\frac{1}{2}  $$ .

Da der hintere Faktor monoton fallend ist (s.o.) gilt: $$ a_1 \leq a_n \leq a_2 $$ .

## Beweise mittels Definition

### $$ a_n = \frac{10n+7}{5+2n}  $$

1. Untere Schranke: Da $$ a_n $$ monoton wächst (s.o.), kann als untere Schranke das Infimum genommen werden: $$ a_1 = \frac{3}{7}  $$.
2. Obere Schranke: Polynomdivision ergibt $$ a_n = 5 - \frac{32}{2n+5}$$. Da der hintere Summand $$ > 0 $$ ist, ist $$ a_n $$ nie $$ 5 $$ oder größer.
3. Ergebnis: $$ \frac{3}{7} \leq a_n \leq 5 $$.

### $$ a_n = \frac{2n+1}{n+1}  $$
Oben haben wir gezeigt, dass $$ a_n $$ monoton wächst. Die Polynomdivision hat zudem ergeben, dass $$ a_n  = 2 - \frac{1}{n+1}  $$.
<div class="aufgabe">Also?<div class="loesung">Lösung: $$ 1 \leq a_n \leq 2 $$ </div></div>

## Beweise mittels vollständiger Induktion

### $$ a_{n+1} = \sqrt{5 a_n},\quad a_1 = 1 $$

zz: $$ a_n $$ beschränkt

Behauptung: $$ S = 5 $$

IA: $$ a_1 = 1 < 5 $$

IV: $$ a_n \leq 5 $$

IS, $$ n \rightarrow n+1 $$: $$a_{n+1} = \sqrt{5 a_n} \stackrel{\textsf{IV}}{\leq} \sqrt{25} = 5$$

> Zeigen Sie, dass aus der Annahme, dass der Limes der Folge $$a$$ ist, $$ a = 5 $$ folgt, indem Sie die Definition der Folge betrachten.

Man spricht hier von *beidseitigem Grenzübergang*.
