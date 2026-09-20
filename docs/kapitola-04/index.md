# Debugování kódu s AI

!!! abstract "Cíl kapitoly"
    Kapitola popisuje možnosti jak AI používat při debugování kódu ve výuce programování. První polovina kapitoly přímo navazuje na předchozí kapitolu.

---

Kromě využití umělé inteligence při psaní kódů je možné ji využít také při jeho degugování. AI může studentovi vodicími otázkami pomoci pochopit, proč daný program nefunguje správně, a vést ho při jeho opravě. Dále je možné nechat AI vytvořit kód a jeho debugování přenechat studentovi. Konkrétní příklad aktivity zaměřené na debugování kódu s AI naleznete *[zde](../kapitola-07/ladeni-chyb.md)*.

---

## 4.1 Debugování kódu s pomocí AI
Podobně jako *[AI tutor](../kapitola-03/index.md)* s využitím *[Pedagogického promtování](../kapitola-02/index.md)* dokáže umělá inteligence idenfikovat pravděpodobný problém v kódu, vysvětlit chybové hlášky, pomoci studentovi pochopit proč kód nefunguje, nebo ho navést k nalezení a ladění chyb. Pro účely vzdělávání není vhodné nechat AI opavit celý kód samotnou bez zapojení studenta. Řešení problému by mělo být na studentovi a AI by měla sloužit jako pomocník, se kterým se student může radit. Nestačí po studentovi požadovat pouze opravu kódu. Student by měl pochopit, kde chyba vznikla, jakým způsobem ji opravil a následně ověřit, že program funguje správně. Nejprve by si měl student sám zkusit chybu najít a vymyslet způsob, jakým ji opraví, potom se může poradit s AI.

V rámci promptu může být AI instruována, aby při pomoci studentovi s debugováním zohledňovala například následující otázky:

- Je problém v chybějící znalosti studenta?
- Je aktuální kód a postup na dobré cestě?
- Jak blízko je student k nalezení řešení?
- Zvládl student předchozí radu?
- Má student rozumný plán?

---

## 4.2 Debugování vygenerováného kódu od AI

Opravit kód, který vegenerovala AI může pro studenty kognitivně náročnější, proto by měl být tento typ úlohy zařazen do výuky jako pokročilejší úloha. Jako kód pro úlohu lze použít kód, který AI záměrně na pokyn vygenerovala s chybou, nebo kód, ve kterém AI při generování neúmyslně vytvořila chybu. Student by nejprve měl sám ověřit jak dobře kód funguje, například jestli kód postrádá klíčovou logiku, nebo stačí pouze upravit okrajové případy. Potom začít s debugováním a případně se poradit s AI, jak je popsáno výše.

Při opravování AI-generovaného kódu může být problém způsoben i snadno přehlédnutelnou chybou, jako je záměna *<* za *<=* nebo *elif* za *if* nebo špatné zacházení s výstupem (*print* namísto *return*). Proto je nutné vždy kriticky ověřit AI výstup, jak je popsáno v *[předchozí kapitole](../kapitola-03/index.md)*.

---

## Shrnutí kapitoly

!!! success "Klíčové poznatky"
    - Při debugování by měl opravit kód student a AI sloužit jako poradce.
    - Debugování kódu vygenerevaného od AI může představovat kognitivně náročnější úlohu.
    - AI výstup je nutné kriticky zhodnotit a ověřit.

---

*[← Předchozí kapitola: AI jako tutor](../kapitola-03/index.md)*<br>
*[Další kapitola: AI párové programování →](../kapitola-05/index.md)*
