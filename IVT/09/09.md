# 9. Počítačové jazyky

***Obsah otázky:*** reprezentace algoritmu pomocí programovacího jazyka; druhy počítačové jazyků; spojitost strojového kódu a programovacího jazyka, např. JSA v reálné či teoretické architektuře (LMC); příklady zápisu algoritmu v programovacím jazyku různé úrovně

# K čemu slouží programovací jazyk?
- Programovací jazyk = prostředek pro zápis algoritmů, jež mohou být provedeny na počítači
- Zápis algoritmu ve zvoleném programovacím jazyce se nazývá *program*
- Programovací jazyk je komunikačním nástrojem mezi programátorem, který v programovacím jazyce formuluje postup řešení daného problému, a počítačem, který program interpretuje technickými prostředky. Programovací jazyk je vlastně soubor pravidel pro zápis algoritmu, odborně řečeno se jedná o formální jazyk.

# Strojový kód x Programovací jazyk
- Počítač "rozumí" pouze jednomu "jazyku", který je navržen pro zpracování procesorem
- Programy v programovacích jazycích jsou na ně překládány tzv. kompilátorem
- Jazyk symbolických adres - První úroveň abstrakce nad strojovým kódem, umožňuje do strojového kódu vkládat např. značky a data a na ty se pak odkazovat, tento jazyk musí poté tzv. assembler sestavit do čistého strojového kódu
    - JSA si můžete vyzkoušet v teoretické architektuře LMC (little man computer) [zde](https://www.peterhigginson.co.uk/lmc/). Používá dekadickou soustavu a je tím jednodušší pro učení

# Dělení programovacích jazyků
Dle míry abstrakce:
- *nízkoúrovňový* - svojí syntaxí se blíží stroji
- *vysokoúrovňový* - svojí syntaxí se blíží člověku

Dle způsobu překladu a spuštění:
- *kompilované* - před spuštěním jsou přeloženy kompilátorem, omezeny na jeden OS/architekturu
- *interpretované* - nepřekládají se, ztrácí kvůli tomu rychlost
- tyto přístupy kombinuje např. Java, která kód kompiluje do Java Virtual Machine - pro spuštění potřebujeme JVM, ale interpretace tohoto kódu je rychlejší než interpretace zdrojového kódu

# Příklady programovacích jazyků
- **C** - nízkoúrovňový strukturovaný jazyk, primárně se v něm vytváří software jako operační systémy, kompilátory, databáze nebo také programy pro hardware a embedded zařízení, např. v autech, a vychází z něj další jazyky; je velmi rychlý, ale složitý pro komplikovanější účely
- **C ++** - multiparadigmatický (jak strukturovaný, tak i objektově orientovaný) jazyk, vychází z jazyka C, používá se k programování výkonných programů jako např. her/herních enginů 
- **Python** - multiparadigmatický vysokoúrovňový interpretovaný jazyk, má jednoduchou syntaxi která značně urychluje a usnadňuje vývoj, vhodný pro začátečníky i pro profesionály, ztrácí ale kvůli interpretovanosti rychlost, proto se nevyužívá pro programy ve kterých záleží na výkonu; kvůli obrovskému množství knihoven (rozšíření) je velmi flexibilní a není v podstatě oblast, se kterou by si Python a jeho knihovny neporadily (např. TensorFlow, PyTorch pro AI, pandas pro tabulky, numpy pro výpočty...)

*Vyber si jeden programovací jazyk a vyjmenuj základní datové typy, které se v tomto jazyce používají*

Python:
- `int` - integer neboli celé číslo
- `float` - float neboli desetinné číslo
- `str` - string neboli textový řetězec
- `bool` - boolean neboli pravdivostní hodnoty
- `list` - list neboli seznam
- `dict` - dictionary neboli slovníky
- `tuple` - tuple neboli n-tice