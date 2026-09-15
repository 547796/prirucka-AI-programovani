# Aktivita: Ladění chyb s AI asistentem

**Čas:** 45 minut &nbsp;|&nbsp; **Stupeň:** ZŠ / SŠ &nbsp;|&nbsp; **Jazyk:** Python

---

## Cíl aktivity

Žáci se naučí:

- formulovat dotaz na AI tak, aby dostali užitečnou nápovědu (ne hotové řešení),
- kriticky posoudit odpověď AI a ověřit ji spuštěním kódu,
- rozlišit vlastní chybu od chyby v odpovědi AI.

---

## Potřebné vybavení

- Počítač s přístupem k internetu (1 na žáka nebo dvojici)
- Přístup k ChatGPT nebo Claude (zdarma)
- Python prostředí – IDLE, Thonny nebo online (repl.it)

---

## Postup

### Fáze 1 – Příprava (5 min)

Učitel rozdá žákům záměrně chybný kód:

```python title="kod_s_chybami.py"
def secti_cisla(a, b)
    soucet = a + b
    return součet  # (1)!

vysledek = secti_cisla(3, 5)
print("Výsledek je: " + vysledek)
```

1. Pozor – proměnná má diakritiku, Python si s tím neporadí.

!!! tip "Tip pro učitele"
    Kód obsahuje 3 záměrné chyby. Žáci je mají nejprve najít **sami**, bez AI.

### Fáze 2 – Samostatná práce (10 min)

Žáci se pokusí chyby najít a opravit bez pomoci AI. Výsledky si zapíší.

### Fáze 3 – Práce s AI (20 min)

Žáci popíší chybu AI asistentu. Diskutujte předem, **jak se ptát**:

=== "Špatný prompt"
    ```
    Oprav mi tento kód.
    ```
    *(AI kód opraví, žák se nic nenaučí)*

=== "Dobrý prompt"
    ```
    Tento kód mi hází chybu: SyntaxError: invalid syntax.
    Nevíš, co by mohlo být špatně? Nepiš mi opravený kód,
    jen mi poraď, kde hledat.
    ```

### Fáze 4 – Reflexe (10 min)

Třídní diskuze:

- Pomohla AI? Jak?
- Řekla AI něco špatně?
- Co bys příště zeptal jinak?

---

## Variace

!!! example "Pro pokročilé (SŠ/VŠ)"
    Žáci sami vytvoří chybný kód pro spolužáka. Pak ho ladí společně s AI.

!!! example "Pro začátečníky (ZŠ)"
    Zjednodušit na 1 chybu, pracovat ve dvojicích, učitel moderuje dialog s AI společně.

---

## Hodnocení

Žáci odevzdají krátkou reflexi (5–10 vět):

1. Jaké chyby jsi v kódu našel/a?
2. Jak jsi formuloval/a dotaz na AI?
3. Byla odpověď AI správná? Jak jsi to ověřil/a?

---

*[Další aktivita: AI jako recenzent kódu →](recenzent-kodu.md)*
