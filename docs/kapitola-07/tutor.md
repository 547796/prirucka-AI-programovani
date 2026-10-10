# Aktivita: AI tutor

**Časový odhad:** 25-35 minut

---

## Cíl aktivity
Praktické seznámení použití AI jako tutora ve výuce programování, žáci si vyzkouší analyzovat kód a upravit jej. Aktivita předpokládá, že jste žáky seznámili s *[Pedagogickým promptováním](../kapitola-02/index.md)*, můžete využít i šablonu, která se nachází na konci odkazované kapitoly. Programovací úloha je zaměřena na hledání duplicit v seznamu, avšak lze použít jakoukoliv jinou úlohu podle potřeby učitele.

Kód v Pythonu byl vygenerován pomocí AI.

---

## Zadání
Vysvětlete co zadaný program dělá. Předpokládejte, že na vstupu je seznam celých čísel. Postupujte podle následujících instrukcí:

- sami kód analyzujte, odhadněte co dělá (můžete si kód spustit),
- po vlastní analýze svůj návrh konzultujte s AI. Pokud si nejste jisti, co program dělá, nechte se od AI navést pomocí naváděcích otázek (zakažte AI vám poskytnout přímé řešení),
- stručně učiteli popište co program dělá (podle pokynů učitele zapište jako text, nebo konzultujte ústně),
- přepište kód do lépe čitelné podoby, zaměřte se na názvy proměnných, strukturu programu a srozumitelnost jeho logiky. Nejdříve zkuste sami, pokud si nebudete jisti, nebo si chcete výsledek zkontrolovat, poraďte se s AI (zakažte AI vám poskytnout přímé řešení),
- výsledný kód odevzdejte učiteli.

```python title="kod.py"
def funkce_a(x):
    q = 0
    while q < len(x):
        w = 0
        while w < len(x):
            if q - w != 0:
                if str(x[q]) == str(x[w]):
                    return True
            w += 1
        q += 1
    return False

# Příklad volání:
vysledek = funkce_a([1, 5, 8, 3, 5])
print(vysledek)
```

---

??? success "Vzorové řešení"
    Řešení je voleno s ohledem na to, že ne na každé SŠ se probírají množiny (set) jako datová struktura.
    ```python title="citelnykod.py"
    def obsahuje_duplicity(x):
        videne = []
        for polozka in x:
            if polozka in videne:
                return True
            videne.append(polozka)
        return False

    # Příklad volání:
    vysledek = obsahuje_duplicity([1, 5, 8, 3, 5])
    print(vysledek)
    ```

---

# Reflexe

!!! example "Na konci aktivity se zamyslete nad otázkami:"
    - Proč je potřeba kód přepsat do lépe čitelné podoby?
    - Jak dobře mi AI pomohla? Dokázala mě navést na řešení pomocí otázek?
    - Jak jste ověřili, že váš upravený program funguje správně?

*[← Zpět na přehled aktivit](index.md)*