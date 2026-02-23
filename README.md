# 🇨🇿 humanizer-cz

> Skill pro Claude AI — detekce a humanizace AI-generovaného textu v češtině

[![Claude](https://img.shields.io/badge/Claude-Skill-blueviolet?style=flat-square&logo=anthropic)](https://claude.ai)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)
<div align="center">

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/mirecekdg)

</div>

---

## Co to je?

**humanizer-cz** je specializovaný skill pro **Claude AI** (Anthropic) a další LLM, který slouží k detekci a odstranění znaků AI-generovaného textu v češtině. Na rozdíl od běžných anglických humanizerů je tento nástroj postavený na akademickém výzkumu českých univerzit a zohledňuje specifika českého jazyka.

Skill obsahuje komplexní příručku s **27 vzory AI psaní** rozdělenými do **14 strukturovaných sekcí**, včetně tabulek nadužívané AI slovní zásoby, příkladů před/po a 14krokového editačního procesu.

Skill funguje s:
- **Claude Project** — nahrajte `SKILL.md` jako knowledge soubor nebo vložte do Project Instructions
- **Claude API** — použijte jako system prompt
- **Agent Zero** — plně kompatibilní jako Agent Zero skill
- **Jakýkoli LLM** — funguje s každým LLM, který podporuje systémové instrukce

Klíčovým akademickým nálezem, na kterém skill staví, je rozlišení **statického vs. dynamického textu** (Milička et al., 2025) — AI texty jsou výrazně nominálnější (více podstatných jmen, méně sloves), což je nejsilnější signál pro detekci.

## Proč to vzniklo?

Existující humanizační nástroje jsou navrženy pro angličtinu a na češtinu nefungují. Čeština má unikátní vlastnosti, které AI systémy nedokážou správně napodobit: **volný slovosled** (ne rigidní SVO), **7 pádů** se složitou deklinací, **obecnou češtinu** jako neformální registr a bohatou morfologii. AI texty v češtině jsou proto rozpoznatelné podle specifických vzorů, které tento skill systematicky pokrývá.

## Hlavní funkce

### SKILL.md — Humanizační příručka

- **27 vzorů AI psaní** specifických pro češtinu
- **14 strukturovaných sekcí** od obsahových po jazykové, stylové a komunikační vzory
- **Klíčový akademický nález**: statický vs. dynamický text (nejsilnější detekční signál)
- **35+ českých AI stop words** + 15 anglických leaků s českými ekvivalenty
- **Kompletní příklady před/po** — celý text od AI verze po humanizovanou
- **14krokový editační proces** pro systematickou humanizaci
- **Sekce o entropii** — jak zvýšit nepředvídatelnost textu
- **Reference na akademické práce** (Masarykova univerzita, Univerzita Karlova, KInIT)

## Použití

### S Claude AI

#### Jako Claude Project

1. Vytvořte nový **Claude Project** na [claude.ai](https://claude.ai)
2. Nahrajte `SKILL.md` jako knowledge soubor (nebo vložte jeho obsah do **Project Instructions**)
3. Pošlete text k humanizaci:

```
Zhumanizuj tento text:

Implementace komplexního řešení vyžaduje zásadní transformaci stávajících
processů. Nicméně je důležité poznamenat, že klíčové aspekty tohoto přístupu...
```

Claude automaticky použije příručku a provede 14krokový editační proces.

#### Jako system prompt (API)

Vložte obsah `SKILL.md` jako system prompt a text k humanizaci jako user message:

```python
import anthropic

client = anthropic.Anthropic()

with open("SKILL.md", "r") as f:
    skill_content = f.read()

message = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=4096,
    system=skill_content,
    messages=[{"role": "user", "content": "Zhumanizuj tento text:\n\n..."}]
)
```

### S Agent Zero

Skill je plně kompatibilní s frameworkem [Agent Zero](https://github.com/frdel/agent-zero):

```bash
# Zkopírujte složku do skills adresáře Agent Zero
cp -r humanizer-cz /path/to/agent-zero/skills/
```

Po restartování Agent Zero se skill automaticky načte a bude dostupný pro humanizaci českých textů.

### S jiným LLM

`SKILL.md` funguje jako system prompt pro jakýkoli LLM, který podporuje systémové instrukce (GPT-4, Gemini, Llama, Mistral aj.). Stačí vložit obsah souboru jako system prompt a poslat text k humanizaci jako uživatelskou zprávu.

## Pokryté vzory AI psaní

Skill pokrývá **27 vzorů** rozdělených do 6 kategorií:

### Obsahové vzory (1–7)

1. Nafukování důležitosti a významu
2. Povrchní analýzy s přechodníky a participiálními konstrukcemi
3. Propagační a reklamní jazyk
4. Vágní atribuce a weasel words
5. Formulaické sekce "Výzvy a budoucí vyhlídky"
6. Schematické seznamy
7. Mechanické vyvažování

### Jazykové a gramatické vzory (8–17)

8. Rigidní slovosled (SVO místo volného českého slovosledu)
9. Problémy s registrem (absence obecné češtiny)
10. Dokonalá interpunkce jako signál AI
11. Uniformita délky vět
12. Předvídatelné začátky vět
13. Vyhýbání se složité morfologii
14. Vyhýbání se sponě "je/jsou" (copula avoidance)
15. Nadužívání pravidla tří
16. Negativní paralelismy
17. Elegantní variace (cyklování synonym)

### Stylové vzory (18–21)

18. Nadužívání pomlček (em dash)
19. Nadměrné tučné písmo
20. Vertikální seznamy s inline hlavičkami
21. Emoji dekorace

### Komunikační vzory (22–24)

22. Artefakty chatbotové komunikace v češtině
23. Disclaimery o knowledge cutoff
24. Servilní/sycophantický tón

### Filler a hedging (25–27)

25. České filler fráze
26. Nadměrný hedging
27. Generické pozitivní závěry

## Akademické zdroje

Skill staví na výzkumu českých a slovenských univerzit:

| Autor | Rok | Téma | Instituce |
|-------|-----|-------|-----------|
| Milička et al. | 2025 | Statický vs. dynamický text — nejsilnější detekční signál | PMC / Masarykova univerzita |
| Al Ali | 2025 | Detekce AI textu, entropie, větné začátky | Univerzita Karlova |
| Šigut | 2023 | Diplomová práce — detekce AI v češtině | Masarykova univerzita |
| Macko et al. | 2023 | MULTITuDE — multilingvální detekce (vč. češtiny) | KInIT / EMNLP 2023 |

Kompletní seznam referencí včetně odkazů najdete v souboru [SKILL.md](SKILL.md#reference).

## Jak to funguje?

Když LLM dostane text k humanizaci a má načtený `SKILL.md`, řídí se 14krokovým procesem:

1. **Analýza** — identifikuje AI vzory v textu
2. **Slovní zásoba** — nahradí AI stop words přirozenými alternativami
3. **Syntax** — převede nominální konstrukce na slovesné (statický → dynamický)
4. **Slovosled** — zavede volný český slovosled místo rigidního SVO
5. **Registr** — přidá prvky obecné češtiny kde je to vhodné
6. **Entropie** — zvýší nepředvídatelnost textu
7. **Verifikace** — ověří výsledek

## Struktura projektu

```
humanizer-cz/
├── README.md              # Tento soubor
├── SKILL.md               # Humanizační příručka pro Claude a další LLM
├── LICENSE                # MIT licence
└── .github/
    └── FUNDING.yml        # GitHub Sponsors / Buy Me a Coffee
```

## Licence

MIT — viz [LICENSE](LICENSE)

## Podpořte projekt

Pokud vám tento projekt pomohl, zvažte podporu přes Buy Me a Coffee.

<div align="center">

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/mirecekdg)

</div>

---

*Vytvořeno s ❤️ pro českou AI komunitu*
