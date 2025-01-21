# 11. Objektově orientované a událostmi řízené programování

***Obsah otázky:*** Základní pojmy OOP – atributy, metody, dědičnost, zapouzdření. Událostmi řízené programování – událost, obsluha události.  

## Objektově orientované programování
- je programovací paradigma, kde kód je přidružen k datům (metody jsou zapouzdřeny v objektech), což umožňuje snadnější přenos kódu mezi různými projekty (abstrakce a zapouzdření)
- **DRY** (Don't Repeat Yourself) - důraz na znovupoužitelnost
- jednodušší oprava softwaru
- spíše z pohledu programátora - objekt často odpovídá věci z reálného světa 
- základní jednotkou je **objekt**

### Základní pojmy
- **Třída (class)** 
	- předpis objektu (ten kód, který napíšeme)
	- předpisy metod, atributů
	- třídu samotnou nelze používat, musíme vytvořit *instanci*
	- továrna (factory method) - vytváří konkrétní objekt
- **Objekt (object)** - koncepčně ucelená jednotka daná těmito součástmi:
	- vnitřní stav (vlastnosti) - soubor proměnných, tzv. **atributy** - mohou to být i další objekty
	- vnitřní chování (schopnosti) - soubor procedur, tzv. **metody**
- **Instance třídy** - konkrétní objekt
	- jeden konkrétní jedinec z příslušné třídy

### "Pilíře" OOP
- **Zapouzdření**
	- "zabalení" dat a metod, co s daty pracují, do jednoho objektu
	- přímý přístup k datům můžeme omezit (`private` atribut/metoda v Javě, C#, PHP...)
- **Dědičnost**
	- třídy můžou zároveň dědit své vlastnosti
	- např. Třída `Zvire` s atributem `maHlad` a metodou `jist()` a třída `Ptak` dědící `Zvire` s metodou `letat()`
- **Polymorfismus**
	- "více forem"
	- např. Třída `Zvire` s metodou `mluvit()`, `Ptak` dědící `Zvire` s metodou `mluvit()` která vypíše "Kokodák" a třída `Prase` s metodou `mluvit()` která vypíše "Chrocht"
		- jedna metoda může vyvolat různé funkce
- **Abstrakce**

## Událostmi řízené programování
= programovací paradigma, kde tok programu řídí události
- události nastávají obvykle určitou uživatelskou akcí - klik či pohyb myši, stisk tlačítka...
- program běží v tzv. smyčce událostí (event loop), která sleduje, jestli se nestalo něco, na co by měl program zareagovat, a v případě potřeby "obslouží" událost zavoláním příslušné funkce
- klíčové např. ve webovém vývoji, JavaScript nabízí mnoho událostí