# Aktivita: Debugování kódu

**Časový odhad:** 10-30 minut (podle znalostí studentů)

---

## Cíl aktivity

Procvičení identifikace a opravy logických chyb v programu s podporou AI. Žáci nemusí řešit příliš syntax a mohou se zaměřit více na logiku kódu. Zdůrazněte studentům, že je potřeba s AI komunikovat stylem podporující jejich přemýšlení.

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

---

# Vzorové řešení

```python title="bubblesort.py"
řešení # (1)!

```
1. proměnná swapped patří na začátek vnějšího cyklu; v podmínce má být i všude nahrazeno za j+1; poslední podmínku je potřeba znegovat

---

# Reflexe

!!! example "Na konci aktivity se zamyslete nad otázkami:"
    - Kde vznikly chyby a jaký měly dopad na program?
    - Proč mnou opravený kód (ne)funguje?
    - Poradila mi AI dobře? Proč jsem návrh od AI přijal nebo zamítl?

*[← Zpět na přehled aktivit](index.md)*