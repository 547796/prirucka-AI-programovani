# Aktivita: Párové programování s AI

**Časový odhad:** 35-45 minut

---

## Cíl aktivity
Cílem je praktické vyzkoušení párového programování s AI asistentem. Studenti v párech navrhnou a vytvoří program, rozdělí si práci a budou průběžne svůj postup konzultovat s AI. Aktivita předpokládá, že jste žáky seznámili s *[Pedagogickým promptováním](../kapitola-02/index.md)*. Aktivita je vhodná rovněž jako procvičení práce se seznamy. Žáci dále musí umět pracovat s podmínkami a cykly.

---

## Zadání
Vytvořte program, který vyhodnotí výsledek testu. Na vstupu dostane neprázdný seznam bodů z testu jednotlivých studentů. Seznam obsahuje celá čísla v rozsahu 0-100, nebo znak "N", pokud nějaký student test nepsal. Můžete předpokládat, že alespoň jeden student test vždy psal.<br>
Příklad vstupu: [45, 78, 50, 91, 38, 67, "N", 21];<br>

Program musí umět vypočítat a vypsat:

- průměr všech získaných bodů (studenti, kteří test nepsali se nepočítají)
- nejvyšší dosažený počet bodů
- nejnižší dosažený počet bodů
- počet jedniček z testu (90-100 bodů)
- počet neúspěšných studentů (do 0-44 bodů)
- počet studentů, kteří test nepsali

Pokud je na vstupním seznamu číslo mimo požadovaný interval, program vypíše chybovou hlášku a skončí neúspěšne.

Postupujte podle následujících instrukcí:

1. Společne navrhněte řešení a rozdělte program do funkcí (bez AI).
2. Zkonzultujte svůj návrh s AI. Požádejte o zpětnou vazbu nebo radu. Zakažte AI vypsat hotové řešení.
3. Rozdělte si párové role a domluvte se, kdy si je vystřídáte. Můžete požádat AI o pomoc.
4. Programujte. Jeden student píše kód, druhý na něj dohlíží a radí mu. Můžete se radit s AI, pokud se zaseknete, nebo máte problem se syntaxí.
5. Role si průběžně střídejte.
6. Svoje řešení otestujte na alespoň 3 seznamech. Opravte případné chyby, můžete se poradit s AI.

---

??? success "Vzorový prompt pro párové programátory"
    Jsme dva studenti, kteří párově programují. Jsme začátečníci v pythonu, umíme větvení, cykly a právě probíráme seznamy. Potřebujeme ohodnotit, zda jsme správně rozdělili program do jednotlivých funkcí. Máme za úkol následující:<br>
    [Zadání]<br>
    Vystupuj v roli učitele programování a pomocí zpětné vazby nám ohodnoť, zda jsme na dobré cestě v rozdělení úkolu na jednotlivé funkce. Nedávej nám hotový kód, ani správné rozdělení programu na funkce. Na řešení jsme se domluvili následovně:<br>
    [Rozdělení programu na funkce]

---

# Reflexe

!!! example "Na konci aktivity se zamyslete nad otázkami:"
    - Jak dobře se nám podařila práce bez AI? Dokázali jsme sami program rozdělit do funkcí?
    - Jakým způsobem nám AI radila? Byly její rady a připomínky užitečné?
    - Jak se nám společně pracovalo? Dokázali jsme si rozdělit práci tak, abychom oba aktivně příspívali k řešení?

*[← Zpět na přehled aktivit](index.md)*