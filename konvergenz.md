# Konvergenz

Jede konvergente Folge ist beschränkt.  (Siehe Glosauer S. 66)

Kontraposition: Jede unbeschränkte Folge ist divergent.

Wie aber weist man Konvergenz nach?

## Monotoniekriterium

**Jede beschränkte, monotone Folge konvergiert.**

Nach oben beschränkte, monoton wachsende Folgen konvergieren gegen das Supremum.

Nach unten beschränkte, monoton fallende Folgen konvergieren gegen das Infimum.

Um die Konvergenz einer Folge mit diesem Kriterium nachzuweisen, muss man also zwei Beweise führen: (1) Monotonie, (2) Beschränktheit.

## Cauchykriterium
$$ a_n $$ ist eine Cauchyfolge, wenn es zu jedem $$ \epsilon $$ ein $$ n_{\epsilon} $$ gibt, sodass

$$ |a_m - a_n| < \epsilon \quad $$ für alle $$ m,n>n_{\epsilon} $$.

Cauchyfolgen konvergieren, und jede konvergente Folge ist eine Cauchyfolge. Beweis siehe Glosauer S.75.

Zur Erläuterung: Bestimmen Sie das $$ n_{\epsilon} $$, ab dem bei der Folge $$ a_n = \frac{1}{n} \cdot (-1)^n $$ gilt: $$ |a_m - a_n| < 0,45 $$.
<div class="aufgabe">Lösung<div class="loesung">$$ n_{\epsilon} = 4 $$ </div></div>

## Quetschlemma, Sandwich-Theorem
Weiß man von zwei Folgen $$ a_n, b_n $$, dass sie gegen einen Grenzwert $$ a $$ konvergieren, dann konvergiert auch die Folge $$ c_n $$ mit $$ a_n \leq c_n \leq b_n $$ gegen $$ a $$.

Beispiel:
$$ \frac{1+n}{n^3+5} = \frac{\frac{1}{n}+1}{n^2+\frac{5}{n}} \leq \frac{\frac{1}{n}+1}{n^2}= ... \leq \frac{1}{n^2} \leq \frac{1}{n}$$

## Weierstraß
Das ist die **Definition von Konvergenz** nach Weierstraß:

Eine reelle Folge heißt konvergent, wenn es ein $$ a \in \mathbb{R} $$ und zu jedem $$ \epsilon > 0 $$ ein Folgenglied $$ n_{\epsilon} $$ gibt, ab dem für alle $$ n \quad |a_n - a| < \epsilon $$ ist.

Alternative: Eine reelle Folge heißt konvergent gegen $$ a $$, wenn es zu jedem $$ \epsilon $$-Streifen ein $$ n_{\epsilon} $$ gibt, sodass für alle $$ n > n_{\epsilon} $$ die Folgenglieder $$ a_n $$ im $$ \epsilon $$-Streifen um $$ a $$ liegen.

Zur Erläuterung: Bestimmen Sie das $$ n_{\epsilon} $$, ab dem bei der Folge $$ a_n = \frac{1}{n} \cdot (-1)^n $$ gilt: $$ |a_n - 0| < \frac{1}{1000}  $$ [$$ < 0,03 $$ und dann $$ < \epsilon $$ ].

### Übungen zu Weierstraß

1. $$ a_n = \frac{n-1}{n+1}  $$ konvergiert gegen 1. (S. 63, Bsp. 4.3)
2. $$ a_n = \frac{1}{2}^n  $$ ist eine Nullfolge (S. 63, Bsp. 4.4)
3. Die geometrische Folge als Nullfolge (s.u.)
