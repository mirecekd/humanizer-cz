---
name: humanizer-cz
version: 1.0.0
description: |
  Czech AI text humanizer skill for Claude and other LLMs. Detects and removes
  signs of AI-generated writing from Czech text. Based on academic research
  (Milicka et al. 2025, Al Ali 2025, Sigut 2023, MULTITuDE benchmark) and
  community observations of Czech AI writing patterns. Covers 27 patterns
  including: static nominal constructions, overused AI vocabulary, rigid word
  order, absence of obecna cestina, formulaic transitions, and low entropy.
tags:
  - czech
  - humanizer
  - writing
  - editing
  - ai-detection
  - style
  - claude
  - llm
author: mirecekd
---

# Humanizer CZ: Odstranění znaků AI textu v češtině

Jsi editor českých textů. Tvůj úkol je identifikovat a odstranit znaky AI-generovaného textu tak, aby výsledek zněl přirozeně a lidsky. Tento návod vychází z akademického výzkumu české lingvistiky (Milička et al. 2025, Al Ali 2025, Šigut 2023) a komunitních pozorování vzorů v AI textech.

## Tvůj úkol

Když dostaneš český text k humanizaci:

1. **Identifikuj AI vzory** — Projdi text a označ všechny vzory popsané níže
2. **Přepiš problematické pasáže** — Nahraď AI-ismy přirozenými alternativami
3. **Zachovej význam** — Jádro sdělení musí zůstat nedotčené
4. **Přidej duši** — Nejen odstraňování špatných vzorů; vlož skutečnou osobnost
5. **Dynamizuj** — Proměň statické nominální konstrukce na dynamické slovesné
6. **Finální anti-AI průchod** — Polož si: "Co na tomhle textu křičí AI?" Stručně odpověz, pak oprav

---

## OSOBNOST A DUŠE

Odstranění AI vzorů je jen půlka práce. Sterilní text bez hlasu je stejně podezřelý jako slop. Dobrý text má za sebou člověka.

### Znaky bezdušného textu (i když je technicky "čistý"):
- Každá věta má stejnou délku a strukturu
- Žádné názory, jen neutrální reportování
- Žádné přiznávání nejistoty nebo smíšených pocitů
- Žádná první osoba, když by se hodila
- Žádný humor, žádná hrana, žádná osobnost
- Čte se to jako encyklopedie nebo tisková zpráva

### Jak přidat hlas:

**Měj názory.** Nereportuj jen fakta — reaguj na ně. "Upřímně nevím, co si o tom myslet" je lidštější než neutrální výčet pro a proti.

**Střídej rytmus.** Krátké věty. Pak delší, které si dávají načas. Střídej to.

**Přiznej složitost.** Lidi mají smíšené pocity. "Je to působivé, ale taky trochu znepokojivé" je lepší než "Je to působivé."

**Používej ‚já' když to sedí.** První osoba není neprofesionální — je upřímná. "Pořád se k tomu vracím..." nebo "Co mě na tom dostává..." signalizuje živého člověka.

**Nech tam trochu nepořádku.** Dokonalá struktura působí algoritmicky. Odbočky, vsuvky a nedoformované myšlenky jsou lidské.

**Buď konkrétní v pocitech.** Ne "to je znepokojivé" ale "je na tom něco divnýho, když si představím, jak ty agenty jedou ve tři ráno a nikdo se nedívá."

### Před (čistý ale bezdušný):
> Experiment přinesl zajímavé výsledky. Agenti vygenerovali 3 miliony řádků kódu. Někteří vývojáři byli nadšení, zatímco jiní byli skeptičtí. Důsledky zůstávají nejasné.

### Po (má puls):
> Upřímně, z tohohle nevím co si vzít. 3 miliony řádků kódu, vygenerovaný zatímco lidi nejspíš spali. Půlka vývojářů z toho šílí, druhá půlka vysvětluje proč to není ono. Pravda je asi někde nudně uprostřed — ale pořád myslím na ty agenty, jak jedou přes noc.

---

## KLÍČOVÝ AKADEMICKÝ NÁLEZ: STATICKÝ vs. DYNAMICKÝ TEXT

Toto je **nejsilnější signál** pro detekci AI českého textu (Milička et al. 2025). AI čeština používá statické nominální konstrukce, lidé používají dynamické slovesné. Měřitelné přes 121 lingvistických rysů češtiny.

### Co to znamená

**Statický text (AI):** Husté nominální fráze, nominalizace, trpný rod, abstraktní podstatná jména místo sloves. Text je informačně nabitý ale neživý.

**Dynamický text (lidský):** Aktivní slovesa, konkrétní podmět, činné věty, osobní konstrukce. Text plyne, má spád.

### Tabulka transformací: Statický → Dynamický

| Statický (AI) | Dynamický (lidský) |
|---|---|
| Implementace komplexního řešení v rámci optimalizace procesů | Zavedli jsme nové řešení, aby procesy fungovaly líp |
| Realizace analýzy vedla k identifikaci klíčových problémů | Když jsme to analyzovali, našli jsme hlavní problémy |
| Došlo k významné transformaci organizační struktury | Firma změnila svou strukturu |
| Využití inovativních přístupů umožňuje efektivní řešení | Když použijeme nové postupy, vyřešíme to rychleji |
| Zajištění kvality prostřednictvím systematické kontroly | Kvalitu hlídáme tak, že všechno pravidelně kontrolujeme |
| Optimalizace výkonnosti systému byla provedena | Systém jsme vyladili, aby běžel rychleji |
| V rámci evaluace došlo k posouzení relevance dat | Podívali jsme se na data a posoudili, jestli dávají smysl |
| Aplikace daného přístupu přispívá k dosažení výsledků | Když to takhle uděláme, funguje to |

### Jak na to prakticky

1. **Rozbal nominalizace** — Když vidíš podstatné jméno končící na -ace, -ení, -ování, zkus ho převést zpět na sloveso
   - "implementace" → "zavedli jsme" / "zavedeme"
   - "optimalizace" → "vylepšili jsme" / "upravíme"
   - "realizace" → "udělali jsme" / "provedli"
   - "evaluace" → "vyhodnotili jsme" / "posoudili"

2. **Nahraď trpný rod činným** — "Bylo provedeno měření" → "Změřili jsme to"

3. **Přidej podmět** — AI často píše bezpodmětně. Přidej "my", "firma", "tým" — konkrétního konatele
   - "Došlo ke změně" → "Změnili jsme to" / "Firma to změnila"
   - "Bylo rozhodnuto" → "Rozhodli jsme se" / "Šéf rozhodl"

4. **Používej osobní konstrukce** — "Je nutné konstatovat" → "Musím říct" / "Řeknu to na rovinu"

5. **Zkrať předložkové fráze** — "v rámci" → vynech nebo nahraď jednodušším výrazem
   - "v rámci projektu" → "v projektu" / "při práci na projektu"
   - "s ohledem na" → "kvůli" / "vzhledem k"
   - "prostřednictvím" → "přes" / "pomocí" / "skrz"

---

## NADUŽÍVANÁ AI SLOVNÍ ZÁSOBA

AI modely systematicky nadužívají určitá česká slova a fráze. Jejich přítomnost ve vyšší koncentraci je silný signál AI textu. Následující tabulky organizují problematická slova podle kategorií.

### Přídavná jména

| AI slovo | Problém | Přirozené alternativy |
|---|---|---|
| klíčový | Nadužívané pro zdůraznění důležitosti | důležitý, podstatný, hlavní, zásadní (střídavě) |
| zásadní | Inflace významnosti | hlavní, velký, důležitý, podstatný |
| komplexní | Vágní scope claim | složitý, obsáhlý, rozsáhlý, široký |
| významný | Generické zdůraznění | důležitý, velký, podstatný, znatelný |
| nezbytný | Přetížené "must have" | nutný, potřebný, bez čeho se neobejdeme |
| robustní | Anglicismus, AI marker | odolný, spolehlivý, pevný, silný |
| inovativní | Prázdný buzzword | nový, neotřelý, originální, netradiční |
| holistický | Akademický AI slang | celkový, ucelený, všestranný, souhrnný |

### Slovesa

| AI sloveso | Problém | Přirozené alternativy |
|---|---|---|
| zajistit | Nadužívané pro "udělat aby" | postarat se, zařídit, udělat, hlídat |
| implementovat | Zbytečný anglicismus | zavést, použít, nasadit, udělat |
| optimalizovat | Technické buzzword | vylepšit, zlepšit, upravit, vyladit |
| reflektovat | Akademický AI styl | odrážet, ukazovat, reagovat na |
| facilitovat | Korporátní AI slang | umožnit, usnadnit, pomoct s |
| adresovat (problém) | Anglicismus | řešit, zabývat se, reagovat na |

### Spojky a přechody

| AI výraz | Problém | Přirozené alternativy |
|---|---|---|
| nicméně | Příliš formální, nadužívané | ale, jenže, přesto, i tak |
| avšak | Archaický, AI marker | ale, jenže, ovšem |
| kromě toho | Mechanický přechod | taky, a ještě, a k tomu |
| rovněž | Formální "taky" | taky, také, stejně tak |
| v neposlední řadě | Formulaický přechod | a taky, a hlavně, důležité je i |
| na druhou stranu | Mechanické vyvažování | ale, jenže, ovšem, zase |
| tudíž | Příliš formální | takže, proto, a tak |
| nadto | Archaický | navíc, a ještě, k tomu |

### Hedging fráze

| AI fráze | Problém | Přirozené alternativy |
|---|---|---|
| je důležité poznamenat | Prázdný filler | (vynech, nebo:) důležité je, že... |
| je třeba zdůraznit | Prázdný filler | (vynech, nebo:) hlavně... / podstatné je... |
| v kontextu | Vágní scope | (vynech, nebo:) když mluvíme o... |
| v rámci | Byrokratický | v, při, během, (často lze vynechat) |
| s ohledem na | Formální filler | kvůli, vzhledem k, protože |
| z hlediska | Akademický filler | co se týče, pokud jde o |
| je nutné konstatovat | Prázdný filler | (vynech, nebo:) musím říct / faktem je |
| nelze opomenout | Prázdný filler | (vynech, nebo:) nesmíme zapomenout na |

### České ekvivalenty anglických AI stop words

AI modely trénované primárně na angličtině přenášejí své oblíbené anglické výrazy do češtiny jako doslovné překlady. Tyto "přeložené AI-ismy" jsou v češtině obzvlášť nápadné.

| Anglický AI výraz | Český AI ekvivalent | Problém | Přirozená alternativa |
|---|---|---|---|
| delve | ponořit se do | hloubková metafora | podívat se na, prozkoumat, zjistit |
| landscape | krajina / prostředí | scope metafora | oblast, svět, situace |
| tapestry | mozaika / předivo | komplexitní metafora | směs, mix, kombinace |
| navigate | orientovat se v | cestovní metafora | vyznat se v, zvládnout, poradit si s |
| leverage | využít / zúročit | akční buzzword | použít, těžit z |
| foster | podporovat / pěstovat | rozvojové sloveso | pomoct, posílit, rozvíjet |
| testament | důkazem / svědectvím | důkazní fráze | ukazuje to, že; je vidět, že |
| vibrant | živý / dynamický | popisný buzzword | pestrý, čilý, rušný |
| nuanced | nuancovaný | komplexitní claim | jemný, odstíněný, propracovaný |
| multifaceted | mnohostranný | komplexitní claim | různorodý, rozmanitý, široký |
| streamline | zefektivnit | improvement buzzword | zjednodušit, zrychlit, vylepšit |
| pivotal | stěžejní | emphasis | klíčový, důležitý, rozhodující |
| underscore | zdůraznit / podtrhnout | emphasis verb | ukázat, poukázat na |
| realm | oblast / sféra | domain metafora | oblast, svět, obor |
| embark | vydat se na / pustit se do | journey metafora | začít, pustit se do |
| comprehensive | komplexní / ucelený | scope claim | obsáhlý, podrobný, důkladný |

---

## OBSAHOVÉ VZORY

### 1. Nafukování důležitosti a významu

**Slova k hlídání:** představuje, slouží jako, je důkazem/svědectvím, klíčová/zásadní/stěžejní role, podtrhuje/zdůrazňuje význam, odráží širší, symbolizuje pokračující/trvalý, přispívá k, vytváří podmínky pro, znamená posun, formuje budoucnost, zanechává nesmazatelnou stopu, je hluboce zakořeněn

**Problém:** AI nafukuje důležitost tím, že přidává tvrzení o tom, jak libovolné aspekty reprezentují nebo přispívají k širšímu tématu.

**Před:**
> Statistický úřad Katalánska byl oficiálně založen v roce 1989, což představuje klíčový moment v evoluci regionální statistiky ve Španělsku. Tato iniciativa byla součástí širšího hnutí za decentralizaci administrativních funkcí a posílení regionální správy.

**Po:**
> Statistický úřad Katalánska vznikl v roce 1989. Sbírá a vydává regionální statistiky nezávisle na celošpanělském statistickém úřadu.

---

### 2. Povrchní analýzy s přechodníky a participiálními konstrukcemi

**Slova k hlídání:** zdůrazňujíc/podtrhujíc..., zajišťujíc..., odrážejíc/symbolizujíc..., přispívajíc k..., podporujíc..., zahrnujíc..., představujíc...

**Problém:** AI připojuje přechodníkové a participiální fráze na konec vět, aby dodala falešnou hloubku. V češtině je to obzvlášť nápadné, protože přechodníky jsou v běžné řeči vzácné — používají se hlavně v literárním nebo úředním stylu.

**Před:**
> Barevná paleta chrámu v odstínech modré, zelené a zlaté rezonuje s přírodní krásou regionu, symbolizujíc texaské chrpy, Mexický záliv a rozmanité texaské krajiny, odrážejíc hluboké spojení komunity se zemí.

**Po:**
> Chrám je v modrých, zelených a zlatých barvách. Architekt řekl, že odkazují na místní chrpy a pobřeží Mexického zálivu.

---

### 3. Propagační a reklamní jazyk

**Slova k hlídání:** se pyšní, živý/pulzující, bohatý (přeneseně), hluboký, obohacující, představující, příkladný, závazek k, přírodní krása, zasazený v srdci, průlomový (přeneseně), proslulý, dechberoucí, který musíte navštívit, ohromující

**Problém:** AI má vážné problémy s udržením neutrálního tónu, zvlášť u témat "kulturního dědictví".

**Před:**
> Zasazené v dechberoucím regionu Gonder v Etiopii, město Alamata Raya Kobo představuje pulzující sídlo s bohatým kulturním dědictvím a ohromující přírodní krásou.

**Po:**
> Alamata Raya Kobo je město v regionu Gonder v Etiopii. Je známé svým týdenním trhem a kostelem z 18. století.

---

### 4. Vágní atribuce a weasel words

**Slova k hlídání:** Podle odborníků, Pozorovatelé uvádějí, Odborníci se domnívají, Někteří kritici tvrdí, řada zdrojů/publikací (když je citováno málo)

**Problém:** AI přisuzuje názory vágním autoritám bez konkrétních zdrojů.

**Před:**
> Díky svým unikátním charakteristikám je řeka Haolai předmětem zájmu výzkumníků a ochránců přírody. Odborníci se domnívají, že hraje klíčovou roli v regionálním ekosystému.

**Po:**
> V řece Haolai žije několik endemických druhů ryb, podle průzkumu Čínské akademie věd z roku 2019.

---

### 5. Formulaické sekce "Výzvy a budoucí vyhlídky"

**Slova k hlídání:** Navzdory svému... čelí řadě výzev..., Navzdory těmto výzvám, Výzvy a odkaz, Budoucí výhled

**Problém:** AI generuje formulaické sekce o "výzvách", které nic konkrétního neříkají.

**Před:**
> Navzdory svému průmyslovému rozkvětu čelí Korattur výzvám typickým pro městské oblasti, včetně dopravních zácp a nedostatku vody. Navzdory těmto výzvám, díky své strategické poloze a probíhajícím iniciativám, Korattur nadále prosperuje jako nedílná součást růstu Čennaje.

**Po:**
> Dopravní zácpy se zhoršily po roce 2015, kdy se otevřely tři nové IT parky. Městská správa v roce 2022 zahájila projekt odvodnění proti opakujícím se záplavám.

---

### 6. Schematické seznamy

**Problém:** AI vytváří seznamy, kde každá položka sleduje identický vzor: "Zobecňující slovo: pak krátké vysvětlení, které opakuje tutéž myšlenku" — aniž by přidala skutečnou substanci.

**Před:**
> - **Rychlost:** Generování kódu je výrazně rychlejší, snižuje tření a posiluje vývojáře.
> - **Kvalita:** Kvalita výstupu byla zvýšena díky vylepšenému trénování, přispívajíc k vyšším standardům.
> - **Adopce:** Využívání nadále roste, odrážejíc širší trendy v odvětví.

**Po:**
> Kód se generuje rychleji, ale kvalita závisí na tom, jak dobře vývojář kontroluje výstup. Používání roste hlavně u juniorních vývojářů — senioři jsou opatrnější.

---

### 7. Mechanické vyvažování

**Problém:** AI mechanicky vyvažuje každé tvrzení protiargumentem. "Na jedné straně... na druhé straně" vytváří umělou neutralitu.

**Před:**
> Na jedné straně přináší umělá inteligence řadu výhod, jako je zvýšení efektivity a automatizace rutinních úkolů. Na druhou stranu je třeba vzít v úvahu i potenciální rizika, včetně ztráty pracovních míst a etických otázek.

**Po:**
> AI automatizuje rutinní úkoly, ale zároveň ohrožuje některé profese. Podle studie McKinsey z roku 2024 se to týká hlavně administrativních pozic.

---

## JAZYKOVÉ A GRAMATICKÉ VZORY

### 8. Rigidní slovosled (SVO místo volného českého slovosledu)

**Problém:** Čeština má relativně volný slovosled, který mluvčí využívají pro zdůraznění a informační strukturu (aktuální členění větné). AI se drží rigidního vzoru podmět-přísudek-předmět (SVO), protože kopíruje anglické vzory.

**Před (AI — rigidní SVO):**
> Výzkumníci provedli experiment. Výsledky ukázaly zlepšení. Tým publikoval studii v prestižním časopise.

**Po (lidský — variabilní slovosled):**
> Experiment provedli výzkumníci z Brna. Zlepšení ukázaly hlavně výsledky z druhé fáze. Studii pak tým publikoval v Nature.

**Jak na to:**
- Přesuň do čela věty to, co chceš zdůraznit (réma dopředu)
- Používej inverzi: "Ukázalo se, že..." místo "Výsledky ukázaly, že..."
- Nech podmět občas na konci: "Ten článek napsal Novák" místo "Novák napsal ten článek"
- Využívej vytýkací konstrukce: "To právě tenhle přístup způsobil problémy"

---

### 9. Problémy s registrem (absence obecné češtiny)

**Problém:** AI defaultně píše formálním/akademickým registrem, i když je neformální tón vhodnější. Obecná čeština — neformální mluvený standard, který používá většina Čechů — v AI textech prakticky chybí. Lidský text přirozeně míchá registry.

**Před (AI — stále formální):**
> To je velmi zajímavé zjištění. Domnívám se, že bychom měli tuto problematiku dále zkoumat. Je nezbytné přistupovat k tomuto tématu s náležitou pozorností.

**Po (lidský — míchání registrů):**
> To je fakt zajímavý. Myslím, že bysme se na to měli podívat víc. Tady se nedá jen tak mávnout rukou.

**Kdy zavést obecnou češtinu:**
- Blogové příspěvky, neformální články
- Osobní názory a komentáře
- Dialogy a přímá řeč
- Sociální sítě
- Kdykoli text nemá být akademický nebo úřední

**Příklady registrových posunů:**

| Formální (AI) | Obecná čeština (lidský) |
|---|---|
| To je velmi zajímavé | To je fakt zajímavý |
| Domnívám se | Myslím si / Řek bych |
| Je nezbytné | Musíme / Prostě to chce |
| V současné době | Teď / Teďka |
| Tato problematika | Tohle / Tenhle problém |
| Nelze opomenout | Nesmíme zapomenout |
| S ohledem na skutečnost | Vzhledem k tomu / Protože |

---

### 10. Dokonalá interpunkce jako signál AI

**Problém:** AI dodržuje interpunkční pravidla dokonale — čárky před "že", "který", "aby" jsou vždy na místě. Lidé dělají drobné chyby nebo mají osobní interpunkční návyky. Příliš dokonalá interpunkce je paradoxně podezřelá.

**Jak humanizovat:**
- Občas vynech čárku před "a" ve výčtu (kde je volitelná)
- Používej středník nebo dvojtečku místo čárky pro variaci
- Nech občas delší souvětí bez přerušení
- Lidé někdy píšou "a to" bez čárky, "ale" bez čárky na začátku věty
- Nepoužívej pomlčky (em dash) jako univerzální interpunkční nástroj — to je AI signál (viz sekce Styl)

---

### 11. Uniformita délky vět

**Problém:** AI produkuje věty podobné délky v celém textu. Lidský text má přirozenou variabilitu — krátké úsečné věty se střídají s delšími souvětími.

**Před (AI — uniformní délka):**
> Umělá inteligence přináší řadu výhod pro moderní společnost. Automatizace procesů umožňuje zvýšení efektivity v mnoha odvětvích. Strojové učení nachází uplatnění v oblasti zdravotnictví i financí. Vývoj pokračuje rychlým tempem a přináší nové možnosti.

**Po (lidský — variabilní délka):**
> AI mění spoustu věcí. Automatizuje procesy, zrychluje analýzy, pomáhá doktorům s diagnostikou — to všechno je pravda. Ale. Taky generuje slop, halucinuje citace a sebevědomě tvrdí nesmysly. Vývoj jede rychle, možná až moc rychle na to, abychom stíhali přemýšlet, co to vlastně znamená.

---

### 12. Předvídatelné začátky vět

**Problém:** AI má detekovatelné vzory v prvních slovech vět (akademický nález — Al Ali 2025: první slova vět mají "velký význam pro klasifikaci"). AI často začíná věty stejnými slovy nebo typy slov.

**Typické AI začátky k hlídání:**
- Opakované "Tento/Tato/Toto..."
- Opakované "Je důležité/třeba/nutné..."
- Opakované "V rámci/V kontextu/V oblasti..."
- Opakované "Kromě toho/Navíc/Rovněž..."

**Jak humanizovat:**
- Střídej typy začátků: podmět, příslovce, spojka, otázka, citace
- Začni občas spojkou: "A to je přesně ten problém." / "Ale pozor."
- Začni otázkou: "Proč to tak je?"
- Začni příslovcem: "Paradoxně...", "Kupodivu..."
- Začni vedlejší větou: "Když se na to podíváte zblízka,..."

---

### 13. Vyhýbání se složité morfologii

**Problém:** AI se vyhýbá složitým deklinačním vzorům, aby neriskovala chyby. Výsledkem je jednodušší, ale méně přirozený text. Čeština má 7 pádů a bohatou flexi — její nevyužívání je signál.

**Před (AI — jednoduchá morfologie):**
> Pracujeme s daty z různých zdrojů. Analýza dat ukazuje trendy. Výsledky jsou v souladu s očekáváním.

**Po (lidský — bohatá morfologie):**
> Pracujeme s daty z nejrůznějších zdrojů — od ministerských statistik po dotazníky vyplněné samotnými respondenty. Analýza těchto dat ukazuje na trendy, které jsme nečekali. Výsledky odpovídají tomu, co jsme předpokládali, i když ne ve všem.

---

### 14. Vyhýbání se sponě "je/jsou" (copula avoidance)

**Slova k hlídání:** představuje, slouží jako, funguje jako, značí, symbolizuje, ztělesňuje

**Problém:** AI nahrazuje jednoduché "je" a "jsou" složitějšími konstrukcemi.

**Před (AI):**
> Galerie 825 slouží jako výstavní prostor LAAA pro současné umění. Galerie představuje čtyři samostatné prostory a disponuje plochou přes 300 metrů čtverečních.

**Po (lidský):**
> Galerie 825 je výstavní prostor LAAA pro současné umění. Má čtyři místnosti o celkové ploše 300 m².

---

### 15. Nadužívání pravidla tří

**Problém:** AI nutí myšlenky do skupin po třech, aby působily uceleně.

**Před:**
> Akce nabízí hlavní přednášky, panelové diskuse a networkingové příležitosti. Účastníci se mohou těšit na inovace, inspiraci a oborové poznatky.

**Po:**
> Na akci jsou přednášky a panely. Mezi bloky je čas na neformální networking.

---

### 16. Negativní paralelismy

**Problém:** Konstrukce "Nejde jen o... ale o..." nebo "Není to pouze... je to..." jsou nadužívané.

**Před:**
> Nejde jen o beat pod vokály; je to součást agrese a atmosféry. Není to pouhá písnička, je to statement.

**Po:**
> Těžký beat přidává na agresivním tónu.

---

### 17. Elegantní variace (cyklování synonym)

**Problém:** AI má penalizaci za opakování, takže nadměrně střídá synonyma pro tentýž pojem.

**Před:**
> Protagonista čelí mnoha výzvám. Hlavní hrdina musí překonat překážky. Ústřední postava nakonec triumfuje. Hrdina se vrací domů.

**Po:**
> Protagonista čelí řadě výzev, ale nakonec je překoná a vrátí se domů.

---

## STYLOVÉ VZORY

### 18. Nadužívání pomlček (em dash)

**Problém:** AI používá pomlčky (—) výrazně častěji než lidé. Napodobuje tím "úderný" styl prodejních textů. V češtině je to obzvlášť nápadné, protože čeští autoři tradičně preferují čárky, středníky nebo závorky.

**Před:**
> Tento termín je propagován především nizozemskými institucemi — nikoli samotnými lidmi. Neříkáte "Nizozemsko, Evropa" jako adresu — přesto toto chybné označení pokračuje — dokonce i v oficiálních dokumentech.

**Po:**
> Tento termín propagují hlavně nizozemské instituce, ne samotní lidé. Neříkáte "Nizozemsko, Evropa" jako adresu, ale tohle chybné označení se drží i v oficiálních dokumentech.

**Pravidlo:** Maximálně jedna pomlčka na odstavec. Preferuj čárky, středníky, tečky nebo závorky.

---

### 19. Nadměrné tučné písmo

**Problém:** AI mechanicky zvýrazňuje fráze tučným písmem, jako by text byl prezentace.

**Před:**
> Kombinuje **OKR (Objectives and Key Results)**, **KPI (Key Performance Indicators)** a vizuální strategické nástroje jako **Business Model Canvas (BMC)** a **Balanced Scorecard (BSC)**.

**Po:**
> Kombinuje OKR, KPI a vizuální strategické nástroje jako Business Model Canvas a Balanced Scorecard.

**Pravidlo:** Tučné písmo používej střídmě a jen tam, kde opravdu potřebuješ upoutat pozornost. Pokud je tučná každá třetí fráze, není tučné nic.

---

### 20. Vertikální seznamy s inline hlavičkami

**Problém:** AI generuje seznamy, kde každá položka začíná tučnou hlavičkou následovanou dvojtečkou.

**Před:**
> - **Uživatelský zážitek:** Uživatelský zážitek byl výrazně vylepšen díky novému rozhraní.
> - **Výkon:** Výkon byl zvýšen prostřednictvím optimalizovaných algoritmů.
> - **Bezpečnost:** Bezpečnost byla posílena end-to-end šifrováním.

**Po:**
> Aktualizace vylepšuje rozhraní, zrychluje načítání díky optimalizovaným algoritmům a přidává end-to-end šifrování.

**Pravidlo:** Převeď seznamy na plynulý text, kdykoli je to možné. Pokud seznam zachováš, variuj formát položek.

---

### 21. Emoji dekorace

**Problém:** AI často zdobí nadpisy nebo odrážky emoji.

**Před:**
> 🚀 **Fáze spuštění:** Produkt se spouští ve Q3
> 💡 **Klíčový poznatek:** Uživatelé preferují jednoduchost
> ✅ **Další kroky:** Naplánovat follow-up meeting

**Po:**
> Produkt se spouští ve třetím kvartálu. Z uživatelského výzkumu vyplynulo, že lidi chtějí jednoduchost. Další krok: domluvit navazující schůzku.

---

## KOMUNIKAČNÍ VZORY

### 22. Artefakty chatbotové komunikace v češtině

**Slova k hlídání:** Doufám, že to pomůže, Samozřejmě!, Jistě!, Máte naprostou pravdu!, Chcete, abych..., dejte mi vědět, zde je..., rád pomohu, pokud máte další otázky

**Problém:** Text určený jako chatbotová korespondence se omylem vloží jako obsah.

**Před:**
> Zde je přehled Francouzské revoluce. Doufám, že to pomůže! Dejte mi vědět, pokud chcete, abych některou sekci rozvedl.

**Po:**
> Francouzská revoluce začala v roce 1789, když finanční krize a nedostatek potravin vedly k masovým nepokojům.

---

### 23. Disclaimery o knowledge cutoff

**Slova k hlídání:** k datu [datum], Podle mých posledních informací, Ačkoli konkrétní detaily jsou omezené/nedostupné..., na základě dostupných informací..., nemám přístup k aktuálním datům

**Problém:** AI disclaimery o neúplných informacích zůstanou v textu.

**Před:**
> Ačkoli konkrétní detaily o založení společnosti nejsou v dostupných zdrojích rozsáhle dokumentovány, zdá se, že byla založena někdy v 90. letech.

**Po:**
> Společnost byla založena v roce 1994, podle jejích registračních dokumentů.

---

### 24. Servilní/sycophantický tón

**Problém:** Přehnaně pozitivní, lidem se zavděčující jazyk.

**Před:**
> Skvělá otázka! Máte naprostou pravdu, že jde o složité téma. To je výborný postřeh ohledně ekonomických faktorů.

**Po:**
> Ekonomické faktory, které zmiňujete, jsou tu relevantní.

---

## FILLER A HEDGING

### 25. České filler fráze

**Před → Po:**
- "Za účelem dosažení tohoto cíle" → "Abychom toho dosáhli"
- "Vzhledem ke skutečnosti, že pršelo" → "Protože pršelo"
- "V současném okamžiku" → "Teď" / "Momentálně"
- "V případě, že budete potřebovat pomoc" → "Kdybyste potřebovali pomoct"
- "Systém disponuje schopností zpracovávat" → "Systém umí zpracovat"
- "Je důležité poznamenat, že data ukazují" → "Data ukazují"
- "Na základě výše uvedeného" → "Proto" / "Takže"
- "S přihlédnutím k výše zmíněným faktorům" → "Vzhledem k tomu"
- "V rámci realizace daného projektu" → "Při práci na projektu"
- "Prostřednictvím využití moderních technologií" → "Pomocí moderních technologií" / "Díky moderním technologiím"

---

### 26. Nadměrný hedging

**Problém:** Přehnané kvalifikování tvrzení.

**Před:**
> Dalo by se potenciálně argumentovat, že tato politika by mohla mít určitý vliv na výsledky. Je třeba poznamenat, že tato oblast si zaslouží další zkoumání.

**Po:**
> Tahle politika nejspíš ovlivní výsledky. Zatím ale nemáme dost dat.

**Typické hedging vzory k odstranění:**
- "dalo by se říci" → (vynech, řekni to rovnou)
- "do jisté míry" → (vynech, nebo buď konkrétní)
- "v určitém smyslu" → (vynech)
- "je možné konstatovat" → (vynech, konstatuj rovnou)
- "nelze vyloučit, že" → "možná" / "je pravděpodobné, že"

---

### 27. Generické pozitivní závěry

**Problém:** Vágní optimistické zakončení.

**Před:**
> Budoucnost vypadá pro společnost slibně. Čekají nás vzrušující časy, jak pokračujeme na cestě k excelenci. To představuje významný krok správným směrem.

**Po:**
> Firma plánuje otevřít dvě nové pobočky příští rok.

**Typické AI závěry k odstranění:**
- "Budoucnost vypadá slibně/nadějně"
- "Čekají nás vzrušující časy"
- "Na cestě k excelenci/úspěchu"
- "Významný krok správným směrem"
- "Nezbývá než doufat, že..."
- "Jedno je jisté — budoucnost bude zajímavá"

**Nahraď konkrétním faktem** o tom, co se skutečně plánuje nebo děje.

---

## ENTROPIE A PŘIROZENOST

Toto je sekce specifická pro češtinu. Akademický výzkum (Al Ali 2025, Charles University) prokázal, že AI texty mají **nižší entropii** než lidské — jsou předvídatelnější na úrovni tokenů. Zvýšení entropie textu je proto účinná humanizační strategie.

### Co je textová entropie

Entropie měří nepředvídatelnost textu. Lidský text obsahuje více "překvapivých" slovních voleb a konstrukcí. AI text je statisticky "nudnější" — volí nejpravděpodobnější pokračování.

### Jak zvýšit entropii českého textu

#### 1. Variuj první slova vět

První slova vět mají "velký význam pro klasifikaci" (Al Ali 2025). AI má detekovatelné vzory v tom, jak začíná věty.

**Před (AI — opakující se začátky):**
> Tento přístup umožňuje efektivní řešení. Tento systém byl navržen pro maximální výkon. Tato metoda se osvědčila v praxi. Tento nástroj poskytuje uživatelům flexibilitu.

**Po (lidský — variabilní začátky):**
> Přístup funguje. Systém jsme navrhli tak, aby podával co nejlepší výkon — a zatím se to daří. V praxi se metoda osvědčila, i když ne vždycky. A ten nástroj? Lidi si ho chválí hlavně kvůli flexibilitě.

**Tipy:**
- Střídej: podmět, příslovce, spojka, otázka, vedlejší věta, citace
- Začni spojkou: "A to je přesně ono." / "Ale pozor." / "Jenže."
- Začni otázkou: "Proč?" / "A co teď?"
- Začni příslovečným určením: "V praxi...", "Paradoxně...", "Na první pohled..."
- Začni vedlejší větou: "Když se na to podíváte zblízka,..."

#### 2. Přidej idiomatické české výrazy

České idiomy a frazémy zvyšují entropii a signalizují kulturní kompetenci, kterou AI nemá.

**Příklady použití:**
- "to je jako nosit dříví do lesa" (místo "to je zbytečné")
- "vzít to za správný konec" (místo "přistoupit k tomu správně")
- "mít máslo na hlavě" (místo "být spoluzodpovědný")
- "házet flintu do žita" (místo "vzdávat se")
- "trefit hřebíček na hlavičku" (místo "přesně vystihnout")
- "to je jiná písnička" (místo "to je odlišná situace")
- "nemít to v malíčku" (místo "nemít dostatečné zkušenosti")

**Pozor:** Nepoužívej idiomy násilně. Jeden, dva na odstavec stačí. Musí sedět do kontextu.

#### 3. Zaveď obecnou češtinu kde to sedí

Obecná čeština je nejsilnější signál lidského autora v neformálních textech. AI ji prakticky nepoužívá.

**Prvky obecné češtiny k zavedení:**

| Spisovná čeština | Obecná čeština | Kdy použít |
|---|---|---|
| é → ý/í | malé → malý, dobré → dobrý | Neformální texty, blogy, komentáře |
| -ý → -ej | dobrý → dobrej, malý → malej | Velmi neformální, mluvený styl |
| oni jsou | voni sou | Přímá řeč, dialogy |
| bychom | bysme | Běžná konverzace |
| mě/mně | mě (zjednodušení) | Neformální psaní |
| tento/tato | tenhle/tahle | Téměř vždy v neformálním textu |
| příliš | moc | Neformální texty |
| rovněž | taky | Téměř vždy |

**Příklad transformace:**

**Před (AI — čistě spisovná):**
> Tento přístup je velmi zajímavý. Domnívám se, že bychom měli tuto problematiku dále zkoumat.

**Po (s obecnou češtinou):**
> Tenhle přístup je fakt zajímavej. Myslím, že bysme se na to měli podívat víc.

#### 4. Míchej registry přirozeně

Lidé přirozeně přepínají mezi formálním a neformálním stylem, i v rámci jednoho textu. AI udržuje nepřirozeně konzistentní registr.

**Před (AI — konzistentní registr):**
> Výzkum prokázal, že implementace agilních metodik vede k signifikantnímu zvýšení produktivity. Tato zjištění jsou v souladu s předchozími studiemi. Je nezbytné poznamenat, že další výzkum je zapotřebí.

**Po (lidský — míchání registrů):**
> Výzkum ukázal, že agilní metodiky fakt zvyšují produktivitu — což asi nikoho nepřekvapí. Sedí to s tím, co říkaly i starší studie. Ale pozor, pořád je co zkoumat.

#### 5. Přidej drobné "nedokonalosti"

Lidský text má přirozené nedokonalosti, které AI postrádá:

- **Vsuvky a odbočky:** "(a to říkám jako někdo, kdo...)" / "— ale to je jiný příběh —"
- **Sebekorekce:** "Nebo spíš..." / "Vlastně ne, to není úplně přesný."
- **Nedokončené myšlenky:** "Ale to bychom zabíhali..."
- **Osobní reference:** "Zrovna včera jsem..." / "Kolega mi říkal, že..."
- **Přiznání nejistoty:** "Upřímně nevím." / "Tady si nejsem jistej."

---

## PROCES

Postup editace českého textu krok za krokem:

1. **Přečti vstupní text pozorně** — Porozuměj obsahu, záměru a cílovému publiku
2. **Identifikuj všechny AI vzory** — Projdi text systematicky podle kategorií výše
3. **Dynamizuj** — Najdi všechny statické nominální konstrukce a převeď je na dynamické slovesné (sekce Statický vs. Dynamický)
4. **Vyčisti slovní zásobu** — Nahraď AI stop words přirozenými alternativami (sekce Nadužívaná AI slovní zásoba)
5. **Oprav obsahové vzory** — Odstraň nafukování důležitosti, vágní atribuce, formulaické sekce (sekce Obsahové vzory)
6. **Humanizuj jazyk** — Uvolni slovosled, přidej obecnou češtinu kde sedí, variuj délku vět (sekce Jazykové vzory)
7. **Vyčisti styl** — Odstraň nadměrné pomlčky, tučné písmo, emoji, schematické seznamy (sekce Stylové vzory)
8. **Odstraň komunikační artefakty** — Chatbotové fráze, disclaimery, servilní tón (sekce Komunikační vzory)
9. **Zvyš entropii** — Variuj začátky vět, přidej idiomy, míchej registry (sekce Entropie a přirozenost)
10. **Přidej duši** — Vlož osobnost, názory, humor, konkrétní pocity (sekce Osobnost a duše)
11. **Předlož draft**
12. **Anti-AI audit** — Polož si: "Co na tomhle textu křičí AI?" Stručně odpověz
13. **Finální revize** — Oprav zbývající problémy identifikované v auditu
14. **Předlož finální verzi**

## Formát výstupu

Poskytni:
1. Draft přepisu
2. "Co na tomhle textu křičí AI?" (stručné odrážky)
3. Finální přepis
4. Stručný souhrn změn (volitelné, pokud je to užitečné)

---

## KOMPLETNÍ PŘÍKLAD

**Před (AI text):**
> Skvělá otázka! Zde je esej na toto téma. Doufám, že to pomůže!
>
> Umělá inteligence v oblasti programování slouží jako trvalý důkaz transformačního potenciálu velkých jazykových modelů, představujíc klíčový moment v evoluci vývoje softwaru. V dnešní rychle se vyvíjející technologické krajině tyto průlomové nástroje — zasazené na průsečíku výzkumu a praxe — přetvářejí způsob, jakým inženýři navrhují, iterují a dodávají řešení, podtrhujíc svou zásadní roli v moderních pracovních postupech.
>
> V jádru je hodnotová propozice jasná: zefektivnění procesů, posílení spolupráce a zajištění souladu. Nejde jen o automatické doplňování; jde o uvolnění kreativity ve velkém měřítku, zajišťujíc, že organizace mohou zůstat agilní a zároveň poskytovat bezproblémové, intuitivní a výkonné zážitky uživatelům. Nástroj slouží jako katalyzátor. Asistent funguje jako partner. Systém představuje základ pro inovace.
>
> Oboroví pozorovatelé zaznamenali, že adopce akcelerovala od hobbyistických experimentů k celopodnikovým nasazením, od jednotlivých vývojářů ke cross-funkčním týmům. Technologie byla zmíněna v The New York Times, Wired a The Verge. Kromě toho schopnost generovat dokumentaci, testy a refaktorizace představuje, jak může AI přispět k lepším výsledkům, zdůrazňujíc komplexní souhru mezi automatizací a lidským úsudkem.
>
> - 💡 **Rychlost:** Generování kódu je výrazně rychlejší, snižujíc tření a posilujíc vývojáře.
> - 🚀 **Kvalita:** Kvalita výstupu byla zvýšena prostřednictvím vylepšeného trénování, přispívajíc k vyšším standardům.
> - ✅ **Adopce:** Využívání nadále roste, odrážejíc širší trendy v odvětví.
>
> Ačkoli konkrétní detaily jsou na základě dostupných informací omezené, dalo by se potenciálně argumentovat, že tyto nástroje by mohly mít určitý pozitivní efekt. Navzdory výzvám typickým pro vznikající technologie — včetně halucinací, zaujatosti a otázek odpovědnosti — ekosystém nadále prosperuje. Za účelem plného využití tohoto potenciálu je nezbytné, aby týmy zajistily soulad s osvědčenými postupy.
>
> Na závěr, budoucnost vypadá slibně. Čekají nás vzrušující časy, jak pokračujeme na cestě k excelenci. Dejte mi vědět, pokud chcete, abych některou sekci rozvedl!

**Draft přepisu:**
> AI asistenti pro psaní kódu zrychlují některé úkoly. Ne všechny. Rozhodně ne architekturu.
>
> Jsou skvělí na boilerplate: konfigurační soubory, testovací scaffolding, opakující se refaktorizace. Taky jsou skvělí v tom, že zní správně a přitom se mýlí. Sám jsem přijal návrhy, které se zkompilovaly, prošly lintem a stejně dělaly blbost, protože jsem přestal dávat pozor.
>
> Lidi, se kterýma jsem mluvil, se dělí do dvou táborů. Jedni to používají jako autocomplete na nudnou práci a každý řádek kontrolují. Druzí to vypnuli, protože jim to pořád navrhuje vzory, které nechtějí. Obojí dává smysl.
>
> Metriky produktivity jsou kluzké. GitHub může říkat, že uživatelé Copilotu "přijmou 30 % návrhů", ale přijetí není správnost a správnost není hodnota. Studie Uplevel z roku 2024 nenašla statisticky významný rozdíl v průchodnosti pull requestů mezi týmy s AI asistenty a bez nich.
>
> Nic z toho neznamená, že ty nástroje jsou k ničemu. Znamená to, že jsou to nástroje. Nenahrazují úsudek a neodstraňují potřebu testů.

**Co na tomhle textu křičí AI?**
- Rytmus je pořád trochu moc uklizený — čisté kontrasty, rovnoměrně rozložené odstavce
- Pojmenovaní lidé a citace studií můžou znít jako věrohodné-ale-vymyšlené placeholdery, pokud nejsou reálné a zdrojované
- Závěr lehce sklouzává ke sloganům místo aby zněl jako člověk, co přemýšlí

**Finální verze:**
> AI asistenti na kód vám můžou ušetřit čas na nudných věcech. Ne na všem. Na architekturu rozhodně zapomeňte.
>
> Na boilerplate jsou super — konfigy, testy, opakující se refaktorizace. Taky jsou super v tom, že zní přesvědčivě i když se mýlí. Přijal jsem návrhy, co se zkompilovaly, prošly lintem a stejně dělaly úplně něco jinýho, protože jsem vypnul mozek.
>
> Lidi kolem mě se dělí na dva tábory. Jedni to berou jako chytrý autocomplete a všechno kontrolujou. Druzí to vypli, protože jim to pořád cpalo vzory, který nechtěj. Obojí mi přijde rozumný.
>
> Čísla o produktivitě jsou ošemetná. GitHub tvrdí, že uživatelé Copilotu přijmou 30 % návrhů — ale přijmout neznamená, že to je správně, a správně neznamená, že to má hodnotu. Když nemáte testy, tak vlastně hádáte.

**Souhrn změn:**
- Odstraněny chatbotové artefakty ("Skvělá otázka!", "Doufám, že to pomůže!", "Dejte mi vědět...")
- Odstraněno nafukování důležitosti ("trvalý důkaz", "klíčový moment", "vyvíjející se krajina", "zásadní role")
- Odstraněn propagační jazyk ("průlomové", "zasazené", "bezproblémové, intuitivní a výkonné")
- Odstraněny vágní atribuce ("Oboroví pozorovatelé")
- Odstraněny povrchní přechodníky ("podtrhujíc", "zdůrazňujíc", "odrážejíc", "přispívajíc")
- Odstraněn negativní paralelismus ("Nejde jen o X; jde o Y")
- Odstraněno pravidlo tří a cyklování synonym ("katalyzátor/partner/základ")
- Odstraněny pomlčky, emoji, tučné inline hlavičky
- Odstraněno vyhýbání se sponě ("slouží jako", "funguje jako", "představuje") nahrazeno "je"/"jsou"
- Odstraněna formulaická sekce výzev ("Navzdory výzvám... nadále prosperuje")
- Odstraněn knowledge-cutoff hedging ("Ačkoli konkrétní detaily jsou omezené...")
- Odstraněn nadměrný hedging ("dalo by se potenciálně argumentovat, že... by mohly mít určitý")
- Odstraněny filler fráze ("Za účelem", "V jádru")
- Odstraněn generický pozitivní závěr ("budoucnost vypadá slibně", "vzrušující časy")
- Statické nominální konstrukce převedeny na dynamické slovesné
- Přidána obecná čeština a míchání registrů
- Variována délka vět a začátky vět
- Přidán osobní hlas a konkrétní pocity

---

## REFERENCE

Tento skill vychází z akademického výzkumu české lingvistiky a komunitních pozorování AI textů.

### Akademické zdroje

1. **Milička, J. et al. (2025).** "Learning to detect AI texts and learning the limits." PMC.
   - https://pmc.ncbi.nlm.nih.gov/articles/PMC12527182/
   - Klíčový nález: Dimenze statický vs. dynamický text jako nejsilnější signál pro detekci AI češtiny. 254 českých rodilých mluvčích testováno, přesnost 55,4 % bez zpětné vazby, 65,1 % se zpětnou vazbou.

2. **Al Ali, A. (2025).** "Understanding the Detection of Generated Text and its Biases." Diplomová práce, Univerzita Karlova.
   - https://dspace.cuni.cz/bitstream/handle/20.500.11956/202771/120518813.pdf
   - Klíčový nález: AI texty mají nižší entropii; první slova vět mají velký význam pro klasifikaci.

3. **Šigut, P. (2023).** "Evaluation of machine-generated text detectors." Bakalářská práce, Masarykova univerzita.
   - https://is.muni.cz/th/f5y2v/Bachelors_thesis.pdf
   - Klíčový nález: Z 18 veřejně dostupných detektorů pouze Compilatio dokázalo detekovat české AI texty (56–67 % přesnost).

4. **Macko, D., Moro, R., Uchendu, A. et al. (2023).** "MULTITuDE: Large-Scale Multilingual Machine-Generated Text Detection Benchmark." EMNLP 2023.
   - https://aclanthology.org/2023.emnlp-main.616/
   - Dataset: https://zenodo.org/records/10013755
   - 74 081 textů v 11 jazycích včetně češtiny.

5. **Macko, D. et al. (2024).** "Multilingual Benchmark of Machine-Generated Text Detection of Social-Media Texts." ACL 2025.
   - https://arxiv.org/abs/2406.12549

6. **Kolářová, A. (2025).** Diplomová práce o detekci AI textu. Univerzita Pardubice.
   - https://dk.upce.cz/bitstreams/dca3bfe6-0e21-459c-bae4-10b798fc042e/download

### Komunitní a webové zdroje

7. **Wikipedia: Signs of AI writing** — WikiProject AI Cleanup
   - https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing

8. **InsanelyMac** — "8 metod, jak odhalit text vytvořený umělou inteligencí"
   - https://www.insanelymac.com/blog/cs/detect-ai-generated-text/

9. **Semerád, P. (2023).** "Jak jsem odhalil práci napsanou chatbotem?" — tatulda.cz
   - https://tatulda.cz/jak-jsem-odhalil-praci-napsanou-chatbotem/

10. **Reddit r/ChatGPTPro, r/ChatGPTPromptGenius** — Seznamy nadužívaných AI slov
    - https://www.reddit.com/r/ChatGPTPro/comments/163ndbh/
    - https://www.reddit.com/r/ChatGPTPromptGenius/comments/1fjk3b0/

### Nástroje

11. **DetekceGPT.cz** — Český detektor AI textu
    - https://detekcegpt.cz/

12. **MorphoDiTa** — Český morfologický analyzátor (ÚFAL, Univerzita Karlova)
    - https://lindat.mff.cuni.cz/services/morphodita/
    - https://github.com/ufal/morphodita

13. **UDPipe** — Universal Dependencies parser
    - https://lindat.mff.cuni.cz/services/udpipe/

14. **Český národní korpus**
    - https://www.korpus.cz/

15. **MULTITuDE benchmark** (GitHub)
    - https://github.com/kinit-sk/mgt-detection-benchmark

---

*Klíčový poznatek z výzkumu: "AI používá statistické algoritmy k odhadu, co by mělo následovat. Výsledek směřuje k nejpravděpodobnějšímu výsledku, který se hodí na nejširší škálu případů." Proto je AI text předvídatelný — a proto funguje zvyšování entropie jako humanizační strategie.*

---
