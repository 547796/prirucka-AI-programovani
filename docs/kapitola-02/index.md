# Pedagogické promptování

!!! abstract "Cíl kapitoly"
    Kapitola vysvětluje principy pedagogického promptování a ukazuje, jak mohou studenti komunikovat s AI tak, aby podporovala učení a neposkytovala ihned hotové řešení. Struktura pedagogického promptu a jeho jednotlivé části vycházejí především z přístupu popsaného Xiao et al. (2025).

---

## 2.1 Vysvětlení pojmu

 Prompt je uživatelův vstup, který zadá umělé inteligenci, aby získal požadovaný výstup. Může to být například text, otázka nebo instrukce. Pedagogický promt rozšiřuje tuto definici tím, že záměrně vede AI model k tomu, aby fungoval jako lektor a generoval reakce, které usnadňují vhodné učební aktivity sladěné s aktuální fází vývoje žáka. V praxi to může například znamenat, že AI nasměruje studenta reflexivními nebo vodícími otázkami k řešení úkolu, pomoci studentovi pochopit kód, než aby mu pouze poskytla řešení. Xiao et al. dále uvádějí, že pedagogický prompt se skládá z následujících částí:

 - role AI (například tutor, kolega nebo klient)
 - úroveň studenta (začátečník, středně pokročilý, pokročilý)
 - kontext problému (podrobnosti o úkolu - zadání, studentův kód)
 - identifikace obtíží (problém s vymyslením postupu nebo debugováním)
 - ochranné prvky (co AI nesmí studentovy poskytnout - řešení, opravený kód, pokročilé funkce)
 - postup výuky (reakce AI - vysvětlit krok po kroku, uvést příklad, navést otázkami)

!!! tip "Důležité"
    Než studenti začnou používat při výuce AI, je vhodné s nimi probrat, jak s ní komunikovat a jak její výstupy kriticky hodnotit.

---

## 2.2 Příklady dobrých pedagogických promptů
Níže najdete příklady promptů, které můžete naučit své studenty. Najetím mýší na písmo psané kurzívou se vám zobrazí konkrétní část promptu popsaná výše.

### Pedagogický prompt 1
Jsem začátečník v Pythonu, <span title="identifikace obtíží">*mám problém s debugováním mého kódu.*</span> Zadání, můj kód a výstup jsou následující:

<span title="kontext problému">*[Zadání]<br>
[Studentův kód]<br>
[Aktuální výstup]<br>*</span>

Můžeš vystupovat jako <span title="role AI">* tutor programování pro začátečníky *</span>a pomocí <span title="postup výuky">*několika postupných otázek s možnostmi odpovědí mě krok za krokem vést k tomu, abych sám promyslel řešení problému?*</span>

<span title="úroveň studenta">*Jelikož jsem začátečník*</span>, používej jednoduchou syntaxi a srozumitelný jazyk. <span title="ochranné prvky">*Neuváděj přímé řešení.*</span>


### Pedagogický prompt 2
Zde AI neposkytuje studentovi řešení, ale analogický příklad, který mu pomůže porozumět principu řešení:

<span title="úroveň studenta">*Jsem začátečník v Pythonu*</span> a <span title="identifikace obtíží">*mám potíže s pochopením for cyklu.*</span>
Zadání programovací úlohy, můj kód a výstup jsou následující:

<span title="kontext problému">*[Zadání]<br>
[Studentův kód]<br>
[Aktuální výstup]<br>*</span>

Můžeš vystupovat jako <span title="role AI">* tutor programování pro začátečníky *</span> a <span title="postup výuky">*vytvořit příklad s minimálním množstvím kódu pro jiný problém, který využívá cyklus for k iteraci přes indexy? *</span><br>
<span title="ochranné prvky">*Neposkytuj mi řešení mého příkladu.*</span>


### Pedagogický prompt 3
<span title="úroveň studenta">*Jsem začátečník v Pythonu*</span> a <span title="identifikace obtíží">*mám potíže s porozuměním zadání úkolu.*</span>
Můžeš vystupovat jako <span title="role AI">* tutor úvodu do programování pro začátečníky*</span>, <span title="postup výuky">*uvést mi příklady vstupů a výstupů a vysvětlit, jak se vstup v kontextu daného problému mění na výstup?*</span> Zadání problému je následující:<br>
<span title="kontext problému">*[Zadání]<br>*</span>
<span title="ochranné prvky">*Neposkytuj mi řešení úkolu.*</span>

!!! info "Tip"
    Pro lepší přehlednost lze prompty stukturovat pomocí odrážek nebo nových řádků.
---

## 2.3 Příklady špatných promptů
Nenechte studenty během učení komunikovat s AI následujícím způsobem. Takové prompty zvyšují riziko, že AI hned poskytne studentovi hotové řešení aniž by student přemýšlel.

### Špatný prompt 1
Rozhodně ne:

Můj kód nefunguje, řekni mi co s tím.<br>
<span title="pouze kontext problému">*[Studentův kód]*</span>

### Špatný prompt 2
AI dostane pouze zadání a studentovu úroveň, stále mu však může ihned dát řešení:

<span title="úroveň studenta">*Jsem začátečník v pythonu*</span>, tady je zadání příkladu, <span title="identifikace obtíží">*nevím co s tím*</span>:
<span title="kontext problému">*Napiš program v Pythonu, který v zadaném seznamu čísel najde největší prvek.*</span>

### Špatný prompt 3
Na pohled dostatečný, ale chybí ochranné prvky a konkrétní postup výuky:

<span title="úroveň studenta">*Jsem začátečník v pythonu*</span> a <span title="role AI">*ty jsi můj tutor programování*</span>. Pomoz mi <span title="identifikace obtíží">*najít chybu v tomto programu*</span>. Nejdříve mi vysvětli, v čem může být problém.<br>
<span title="kontext problému">*[Studentův kód]*</span>

---

## 2.4 Univerzální šablona
Tuto šablonu můžete použít jako základ pro jakýkoliv pedagogický prompt:

Jsem [úroveň studenta] v [jazyk nebo oblast].<br>
Mám potíže s [identifikace obtíží].<br>
Zadání a moje aktuální řešení jsou následující: [kontext problému].<br>
Vystupuj jako [role AI].<br>
Pomoz mi pomocí [postup výuky].<br>
[Ochranné prvky – například neposkytuj mi řešení.]

!!! info "Tip"
    Můžete se zeptat i AI, jak správně promptovat.

---

## Shrnutí kapitoly

!!! success "Klíčové poznatky"
    - Pedagogické promptování obsahuje více než jen pokyn k vypracování úkolu.
    - Důležité je nenechat AI aby studentům prozradila řešení bez procesu učení.
    - Před použitím AI studenty v programování je vhodné jim vysvětlit, jak s AI pracovat.

---
*[← Předchozí kapitola: Generativní AI ve výuce programování](../kapitola-01/index.md)*<br>
*[Další kapitola: AI jako tutor →](../kapitola-03/index.md)*
