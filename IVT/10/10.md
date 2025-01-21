# 10. Strukturované programování

***Obsah otázky:*** návrh programu, základní datové typy, rozšířené datové typy, základní  programové konstrukce (podmínky, cykly, funkce), konstrukce složitějších programů. 

## K čemu slouží programovací jazyk?

Programovací jazyk slouží k psaní instrukcí pro počítač, které mu říkají, co má dělat.

1. **Vytváření softwaru**: Programovací jazyky umožňují vývojářům vytvářet různé druhy softwaru, jako jsou aplikace, hry, webové stránky, mobilní aplikace a další.

2. **Automatizace úloh**: Pomocí programování lze vytvořit skripty nebo programy, které automatizují opakující se úkoly nebo procesy, což může ušetřit čas a snížit chybovost.

3. **Manipulace s daty**: Programování umožňuje práci s daty, jako je jejich zpracování, analýza, vizualizace a ukládání. To je důležité v oblastech jako jsou data science, business intelligence a analýza.

4. **Rozvoj systémů a infrastruktury**: Programovací jazyky se používají k vývoji operačních systémů, síťových aplikací, databází a další infrastruktury, která umožňuje fungování moderních informačních technologií.

6. **Rozvoj hardware**: Programovací jazyky se také používají pro vývoj vestavěných systémů a ovládacího software pro hardware, jako jsou mikrokontroléry, senzory a další zařízení.

## Některé programovací jazyky a jejich vlastnosti

### Python:
- **Základní vlastnosti:**
  1. **Snadná syntaxe:** Python má čistou a jednoduchou syntaxi, což ho činí snadno čitelným a pochopitelným.
  2. **Dynamické typování:** Nemusíte explicitně definovat typy proměnných, což zjednodušuje psaní kódu.
  3. **Rozsáhlá knihovna:** Python má rozsáhlou knihovnu standardních modulů, které pokrývají mnoho různých úloh, jako je práce se soubory, síťové komunikace, web development a další.
  
- **Použití:**
  1. **Web development:** Python je populární pro vývoj webových aplikací díky frameworkům jako Django a Flask.
  2. **Data science:** Python je často používán pro analýzu dat a strojové učení díky knihovnám jako Pandas, NumPy, a scikit-learn.
  3. **Automatizace:** Díky své jednoduché syntaxi se Python často používá pro automatizaci opakujících se úloh.

### JavaScript:
- **Základní vlastnosti:**
  1. **Interpretovaný:** JavaScript je interpretovaný jazyk, který běží ve webovém prohlížeči klienta.
  2. **Funkcionální i objektově orientovaný:** Podporuje různé programovací paradigma, což umožňuje psát kód v různých stylech.
  3. **Asynchronní programování:** Podporuje asynchronní operace, což je užitečné pro interaktivní webové aplikace.

- **Použití:**
  1. **Webový vývoj:** JavaScript je základem pro vývoj interaktivních webových stránek a aplikací.
  2. **Node.js:** JavaScript může běžet na serverové straně díky platformě Node.js, což umožňuje psát kompletní webové aplikace v JavaScriptu.
  3. **Mobilní vývoj:** S frameworky jako React Native lze psát mobilní aplikace pro iOS a Android v JavaScriptu.

### C:
- **Základní vlastnosti:**
  1. **Nízkoúrovňový:** C je nízkoúrovňový jazyk, který poskytuje přímý přístup k paměti a hardwaru.
  2. **Efektivní:** C je velmi efektivní jazyk s malým režií paměti a výkonu.
  3. **Přenositelný:** Kód napsaný v C je často přenositelný mezi různými platformami s minimálními úpravami.

- **Použití:**
  1. **Systémový a embedded programming:** C je často používán pro vývoj operačních systémů, ovladačů zařízení a embedded systémů.
  2. **Výkonově náročné aplikace:** Kvůli své efektivitě je C často používán pro vývoj aplikací s vysokým výkonem, jako jsou herní enginy.
  3. **Programování hardware:** Díky své nízkoúrovňové povaze je C často používán pro programování hardware, jako jsou mikrokontroléry a FPGA.


## Rozdělení programovacích jazyků

1. **Podle úrovně abstrakce:**
   - Nízkoúrovňové jazyky (např. jazyk symbolických adres (assembler))
   - Středněúrovňové jazyky (např. C)
   - Vysokoúrovňové jazyky (např. Python)

2. **Podle typu paradigmatu:**
   - Procedurální jazyky (např. C, Pascal)
	- Objektově orientované jazyky (např. Java, C++)
	- Strukturované (C, Pascal)
   - Deklarativní jazyky (např. SQL)
	- Funkcionální jazyky (např. Haskell)
	- Logické jazyky (např. Prolog)

3. **Podle použití:**
   - Obecné programovací jazyky (např. Java, Python)
   - Webové jazyky (např. JavaScript, PHP)
   - Vědecké výpočetní jazyky (např. MATLAB, R)
   - Jazyky pro vestavěné systémy (např. C, Assembly)

4. **Podle platformy:**
   - Jazyky pro web (např. JavaScript, Ruby)
   - Jazyky pro mobilní aplikace (např. Swift pro iOS, Kotlin pro Android)
   - Jazyky pro desktopové aplikace (např. C#, Java)

5. **Podle kompilace vs. interpretace:**
   - Kompilované jazyky (např. C, C++)
   - Interpretované jazyky (např. Python, Ruby)
  
   - Kompilace překládá zdrojový kód do strojového kódu, který je poté spustielný, zatímco interpretace překládá a vykonává kód postupně během jeho spuštění řádek po řádku.

## Datové typy v jazyce Python

Základní datové typy:

- int: celá čísla
- float: desetinná čísla (jejich kódování viz [1. Základní pojmy informatiky](01.md))
- str: textové řetězce
- bool: pravdivostní hodnoty (boolean)
- None: typ "bez hodnoty"

Rozšířené datové typy:

- list: uspořádaný seznam/dynamické pole prvků (`l = [1, 2, 3]`)
- tuple: N-tice, na rozdíl od listu nelze upravovat po vytvoření (`t = ('a', 'b', 'c')`)
- set: neuspořádaná množina, prvky se nemohou opakovat (`s = {"a", "b", "c"}`)
- dict: slovník; páry klíč-hodnota (`d = {"spz": 1234, "model": "Mustang"}`)
- range: rozsah (`range(1, 5)`)

## Základní programové konstrukce
- podmínky
- cykly 
- funkce
