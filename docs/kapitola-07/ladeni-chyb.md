# Aktivita: Debugování kódu

**Časový odhad:** 15-30 minut (podle znalostí studentů)

---

## Cíl aktivity

Procvičení identifikace a opravy logických chyb v programu s podporou AI. Aktivita se zaměřuje na logické chyby a porozumění algoritmu. Zdůrazněte studentům, že je potřeba s AI komunikovat *[stylem podporující jejich přemýšlení](../kapitola-02/index.md)*. Aktivita je vhodná pro žáky, kteří znají princip bubble sortu.

---

# Zadání

Opravte následující bubble sort kód. Postupujte podle následujících instrukcí:
- identifikujte možné chyby v kódu (bez použití AI),
- u každé chyby zkuste vysvětlit, proč může způsobit nesprávné chování programu,
- navrhněte opravu (bez použití AI),
- konzultujte svůj návrh s AI pomocí pedagogického promptování,
- pokud si s něčím nevíte rady, nechte se od AI navést,
- ověřte fungování po opravě chyby.

Při komunikaci s AI popište svůj návrh opravy a zamyslete se, zda výstupy od AI dávají logicky smysl. Zakažte AI vytvořit hotové řešení.

```python title="bubblewrong.py"
mylist = [7, 3, 9, 12, 11]

n = len(mylist)
swapped = False
for i in range(n-1):
  for j in range(n-i-1):
    if mylist[j] > mylist[i]:
      mylist[j], mylist[i] = mylist[i], mylist[j]
      swapped = True
  if swapped:
    break

print(mylist)
```

Očekávaný výstup je [3, 7, 9, 11, 12].

---

# Vzorové řešení
??? example "Vzorové řešení"

```python title="bubblesort.py"
    mylist = [7, 3, 9, 12, 11]

    n = len(mylist)
    for i in range(n-1):
    swapped = False # přesunuto do cyklu
    for j in range(n-i-1):
        if mylist[j] > mylist[j+1]: # i nahrazeno za j+1
        mylist[j], mylist[j+1] = mylist[j+1], mylist[j] # i nahrazeno za j+1
        swapped = True
    if not swapped: # přidána negace
        break

    print(mylist)
```

Kód vychází z příkladu na stránce [W3Schools](https://www.w3schools.com/python/python_dsa_bubblesort.asp).

---

# Reflexe

!!! example "Na konci aktivity se zamyslete nad otázkami:"
    - Kde vznikly chyby a jaký měly dopad na program?
    - Proč mnou opravený kód (ne)funguje? Jak jsem ověřil funkčnost?
    - Poradila mi AI dobře? Proč jsem návrh od AI přijal nebo zamítl?

*[← Zpět na přehled aktivit](index.md)*