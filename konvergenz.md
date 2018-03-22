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
$$ a-n $$ ist eine Cauchyfolge, wenn es zu jedem $$ \epsilon $$ ein $$ n_{\epsilon} $$ gibt, sodass

$$ |a_m - a_n| < \epsilon \quad $$ für alle $$ m,n>n_{\epsilon} $$.

Cauchyfolgen konvergieren, und jede konvergente Folge ist eine Cauchyfolge. Beweis siehe Glosauer S.75

## Quetschlemma, Sandwich-Theorem
Weiß man von zwei Folgen $$ a_n, b_n $$, dass sie gegen einen Grenzwert $$ a $$ konvergieren, dann konvergiert auch die Folge $$ c_n $$ mit $$ a_n \leq c_n \leq b_n $$ gegen $$ a $$.

Beispiel:
$$ \frac{1+n}{n^3+5} = \frac{\frac{1}{n}+1}{n^2+\frac{5}{n}} \leq \frac{\frac{1}{n}+1}{n^2}= ... \leq \frac{1}{n^2} \leq \frac{1}{n}$$

## Weierstraß
Da ist die Definition von Konvergenz nach Weierstraß:

Eine reelle Folge heißt konvergent, wenn es ein $$ a \in \mathbb{R} $$ und zu jedem $$ \epsilon > 0 $$ eine Folgenglied $$ n_{\epsilon} $$ gibt, ab dem für alle $$ n $$
$$|a_n - a| < \epsilon $$ ist.