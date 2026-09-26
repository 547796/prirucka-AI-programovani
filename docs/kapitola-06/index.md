# AI jako nástroj pro přípravu učitele

!!! abstract "Cíl kapitoly"
    Kapitola ukazuje možnosti využití umělé inteligence při přípravě učitele na hodinu, zejména v generování úloh a nápadů do výuky.

---

Umělá inteligence může učiteli pomoci i mimo hodinu. Pokud učitel potřebuji nápady, aktivity nebo příklady kódu, může se obrátit na AI. AI však nedokáže nahradit práci učitele, který musí doporučení a nápady od AI kriticky posoudit.

---

## 6.1 Generování úloh

AI lze využít pro generování programovacích úloh pro studenty a to včetně jejich ukázkového řešení a testů. U generování úloh lze jednoduše měnit kontext a nechat AI vygenerovat více variant jedné úlohy, což může být přínosné například při testování znalostí žáků, kde studenti budou mít zdánlivě odlišná zadání a tedy méně příležitostí od sebe opisovat. Pokud chcete aby úlohy byly lépe přizpůsobené úrovni znalostí žáků, dejte nejprve AI nějaké vzorové úlohy na požadované úrovni. V systémovém nastavení AI (popsáno níže) si uložte pro každou obtížnost (lehká, střední, těžká) kontext úloh, který AI bude při generování používat. Například větvení, cykly nebo seznamy pro lehkou obtížnost, dále například vnořené cykly, rekurzi nebo třídění uložené jako náročnější.

Úlohy je nutné před použitím do výuky zkontrolovat. Novější modely dělají méně chyb, avšak není zaručená 100% správnost. Problematičtější může být zejména generování testů, které ověřují, zda kód funguje. Testy lze využít jako odrazový můstek. Snadné úlohy AI zvládá dobře, ale čím více je úloha náročnější, tím se zvyšuje pravděpodobnost chyby při generování vzorového řešení. Nesprávně vygenerované úlohy lze využít jako debugingové cvičení pro studenty, jak je popsno v kapitole [Debugování kódu s AI](../kapitola-04/index.md).


!!! info "Tip"
    Při generování úloh je užitečné nedělat vše přes 1 prompt. Nejprve požádejte AI o zadání, v dalším promptu o vzorové řešení a potom úlohu můžete upravovat.

---

## 6.2 AI jako pomocník při plánování výuky

Kromě generování konkrétních úloh může učitel požádat AI, aby mu dala nápady do výuky. AI učiteli navrhne například jak výuku zpestřit, ukáže praktické aplikace, navrhne postupy jak látku učit, nebo časové rozložení hodiny. Umělá inteligence ale nenahrazuje práci učitele, slouží jen jako pomocník do výuky, proto by učitelé měli vždy zhodnotit nápad, který jim AI dá. Není přínosné ani nechat AI nahrazovat přípravu učitele, vhodnější může být využívat ji jako zdroj nápadů, které je potřeba protřídit a případně upravit.

Některé nástroje AI umožňují uživateli nastavit trvalé informace a preference, které mohou být zohledněny v další komunikaci. Sdělte AI, že jste učitelé programování pro studenty na střední škole, dále AI nastavte aby při programování používala jednodušší konstrukce odpovídající úrovni studentů. Dále můžete AI dát podrobnější informace o svém předmětu, počtu žáků apod. Požádejte o radu AI, aby vám pomohla vybrat podstatné informace pro její nastavení. V průběhu roku můžete informace aktualizovat, podle toho co se žáci naučili nového. Ne všechny informace je nutné dávat AI do nastavení, informace o postupech výuky můžete vždy upřesnit až přímo v chatu. Podobně si AI mohou nastavit i studenti, ale je potřeba je seznámit s bezpečností, zejména nesdělujte AI své osobní údaje, hesla a jiné citlivé (školní) informace.

---

## 6.3 Příklad promptu pro učitele

Následuje příklad promptu pro generování úloh, principy vychází z *[Pedagogického promptování](../kapitola-02/index.md)*. Prompt obsahuje informace o učiteli, úrovni žáků a jejich dosavadních znalostech. Zároveň poskytuje AI vzorové zadání a zaručuje postupné generování ochranými prvky.

Jsem učitel programování na střední škole / gymnáziu. Právě probíráme seznamy. Používáme Python jako programovací jazyk. Pomoz mi vygenerovat zadání jednodušších úloh pro studenty, kteří mají programování teprve 2. měsíc. Vzorová zadání na požadované úrovni jsou následující:<br>
[Zadání]<br>
Vygeneruj mi zadání pro 5 úloh na podobné úrovni tak, aby při řešení úlohy studenti museli použít seznam, dále studenti znají práci s proměnnými, podmínky a cykly. Způsob použití seznamu se v každé úloze bude lišit. Řešení úloh zatím negeneruj.

*AI dá učiteli úlohy a následuje další prompt:*<br>
Teď mi pro první úlohu dej vzorové řešení v jazyce Python. Stručně popiš co může být pro studenty při řešení nejnáročnější a zdůvodni proč. Používej základní syntax bez pokročilých knihovních funkcí.

*AI poskytne řešení, následuje další prompt:*<br>
Nakonec pro úlohu vytvoř pomocí funkcí assert testování správnosti kódu. Vytvoř i příklady vstupů a výstupů.

## Shrnutí kapitoly

!!! success "Klíčové poznatky"
    - AI může pomoci při generování úloh a vzorových řešení.
    - AI lze využít také jako zdroj nápadů při plánování výuky a tvorbě aktivit.
    - Výstupy AI je vždy nutné zkontrolovat a přizpůsobit potřebám učitele.
---

*[← Předchozí kapitola: AI párové programování](../kapitola-05/index.md)*<br>
*[Další kapitola: Praktické aktivity →](../kapitola-07/index.md)*