# AI jako tutor

!!! abstract "Cíl kapitoly"
    Kapitola popisuje, jak AI používat, aby studenty vedla k přemýšlení při učení programování.

---

AI lze vhodně zapojit do výuky nejen jako generátor kódu. Se správným promptem může AI studenta navádět ke správnému řešení pomocí naváděcích otázek, usnadnit pochopení daného kódu nebo algoritmu, vysvětlit kód řádek po řádku a odpověď přizpůsobit jeho úrovni. Níže najdete vhodné příklady na konkrétní použití. 

---

## 3.1 Vysvětlování kódu
Pokud si studenti neví rady s různými částmi kódu, nebo mají různé příklady, je pro učitele náročné věnovat se každému. S tímto problémem učiteli pomůže AI tutor, který dokáže interagovat se studenty individuálně. Pomocí [pedagogického promptu](../kapitola-02/index.md) AI tutor může studentům pomáhat pochopit kód následovně:

Student poskytne AI kód nebo jeho část, které nerozumí. AI dostane specifické instrukce, jak má studentovi pomoci. Pokud se jedná o kratší kód, AI jej může studentovi vysvětlit řádek po řádku. V případě komplexnějšího kódu je vhodné AI říci, aby nevysvětlovala celý kód naráz, ale po logických částech. AI v jedné odpovědi může vysvětlit jen jednu funkci, rekurzi nebo cyklus.

Je vhodnější nepožadovat pouze vysvětlení kódu po řádcích. AI může nejprve stručně shrnout, jak program funguje, a potom **pomocí naváděcích otázek** se studenta zeptat, proč co konkrétní část kódu dělá a proč je pro daný program důležitá. Student bude AI odpovídat a pokud udělá chybu nebo si pořád nebude jistý, může požádat AI o podrobnější vysvětlení, například po řádcích. Tato metoda vede studenta k přemýšlení nad problémem namísto pasivního čtení výstupu AI.

**Příklad**<br>
Prompt: Jsem začátečník v Pythonu, učím se pracovat se seznamy, ale mám problém s porozuměním následujícího kódu:<br>
[Kód (nebo jeho problematická část)]<br>
[Výstup (pokud nějaký je)]<br>
Jsi můj tutor programování pro začátečníky a pomocí naváděcích otázek mě naváděj k pochopení problému a jeho řešení, nejprve si ověř, jak tomu rozumím a přizpůsob se mé úrovni. Řešení mi neprozrazuj.

AI může pomocí otázek zjistit, jak dobře student problému rozumí a podle jeho odpovědí se pokusit přizpůsobit. AI se pokusí pomocí dalších otázek studenta navést, ten pochopí část, ale pořád mu dělá problém pochopení cyklu.

Prompt: Už chápu většinu, ale pořád nerozumím tomu cyklu. Teď mi řádek po řádku vysvětli, jak ten cyklus funguje a jak se mění proměnná *i* při každém průchodu.

Po další interakci může AI dát studentovi podobný příklad na procvičení. Student si tak může ověřit své pochopení, což pro něj může být přínosné, případně požádat o dodatečné vysvětlení AI nebo učitele.

!!! warning "Pozor"
    To, že si student přečte vysvětlení od AI neznamená, že tomu už rozumí, proto jsou vhodné naváděcí otázky, které podporují aktivní přemýšlení studenta nad problémem.

## 3.2 Kritické reflektování AI odpovědí
Může se stát, že AI bude během učení halucinovat (vymyslí si nesprávnou nebo zcela smyšlenou odpověď). V oblasti vzdělávání je toto problematické, protože student může uvěřit nepravdivé informaci, která zní přesvědčivě. Navíc AI nemusí poskytnout vždy totožné odpovědi, u generování kódu byl pozorován nedeterminismus. Proto není vhodné považovat odpověď za správnou pouze na základě jejího přesvědčivého vysvětlení. Je proto nutné, aby se studenti nad AI odpovědí zamysleli, zda dává v daném kontextu smysl nebo ne. V oblasti programování si například mohou ověřit funkčnost AI kódu jeho spuštěním a otestováním, zejména na krajních případech. Pokud si student není jistý odpovědí od AI, může s ní o tom vést dialog, nebo se zeptat učitele. Další možnost je se na stejnou otázku zeptat AI znovu v jiném chatu, a to klidně i vícekrát, ale stále to neznamená jednoznačné ověření pravdivosti. Kritické reflektování platí pro **každou** AI odpověď, nejen v případě vysvětlování kódu.

Při řešení úkolu s AI by studenti měli postupovat způsobem, který kromě podporování přemýšlení studentů a kritické reflexe AI odpovědí navíc omezuje pasivní spoléhání se na AI:

- Nejdřív o úkolu přemýšlejte sami. Zkuste se zamyslet, jak byste problém řešili, navrhnout postup řešení nebo jeho začátek, případně pojmenujte to, s čím máte problém.
- Pokud si nevíte rady, požádejte AI o pomoc, ne o hotové řešení.
- Zamyslete se nad AI výstupem, zda dává smysl, případně s AI veďte dialog, nebo se obraťte na učitele.
- Otestujte své řešení, jestli funguje. AI může pomoci s generováním vstupů pro program, nebo navrhnout testy.
- Ověřte si své porozumění. Například diskusí o fungování řešení se spolužákem, učitelem nebo AI, případně zkuste vypracovat podobný úkol.

---

## Shrnutí kapitoly

!!! success "Klíčové poznatky"
    - AI jako tutor může navést studenty ke správné odpovědi pomocí naváděcích otázek, které vedou studenty k přemýšlení.
    - AI tutor by se měl snažit o aktivní zapojení studenta.
    - Každou odpověď od AI by si studenti měli kriticky zhodnotit, zda dává smysl.

---

*[← Předchozí kapitola: Pedagogické promptování](../kapitola-02/index.md)*<br>
*[Další kapitola: Debugování kódu pomocí AI →](../kapitola-04/index.md)*
