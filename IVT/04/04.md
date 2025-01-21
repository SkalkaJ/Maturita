# 4. Instalace OS unixového typu

***Obsah otázky:*** ukázka virtualizace OS Unixového typu na PC. Instalace systému, popis systému. Souborové systémy, organizace souborového systému. CLI, GUI 

## Virtualizační software
- VirtualBox
	- multiplatoformový, open-source nástroj pro virtualizaci
	- **virtualizace** je proces, kdy se vytváří virtuální výpočetní prostředí namísto fyzického, často vytváří virtuální hardware, OS, atd
	- jeden PC/server může být rozdělen na několik virtuálních počítačů - snižuje počet využívaných serverů, spotřebu energie, náklady na infrastrukturu
	- Postup: Nový --> nastavení --> úložiště --> cd ikonka --> cd ikonka napravo --> choose/create a VOD --> vybrat .iso soubor --> run --> install

## OS unixového typu
- víceuživatelský multitasking OS s modulovým designem (= dělí systém do menších částí, "modulů", mohou být tvořeny, vyměňovány a upravovány)
- unixová filozofie = autor Ken Thompson, prosazuje minimalistický a modulový software development ("Do one thing and do it well")
- od svých předchůdců se liší tím, že byl jako první přenosný (napsán v C)
- hierarchický souborový systém (stromová str.), data ukládá jako "plain text"
- malé programy, které plní specifické úkoly - jejich propojení v shellu použitím "pipe" (|)
	- output jednoho programu je automaticky používán jako input druhého
- **výhody**: multitasking (proto využíván ve větších institucích, např. servery), efektivní využití paměti, sjednocený souborový systém (zařízení, programy a data se stávají soubory), vysoce přenosný
- **nevýhody**: ne-přátelské rozhraní pro nové uživatele, nutnost znát a rozumět hlavním vlastnostem, nutnost psát příkazy přesně a kontrolovat je
- **použití**: nejčastěji pro webové servery (multitasking, bezpečnost), databáze, cloud aplikace, zabezpečení cloudu (servery přístupné přes internet)
- unixový souborový systém: nejmenší jednotkou je **soubor** (obsahuje data) - soubory jsou ve **složkách** - složky jsou ve **stromové struktuře**
- Příkaz lze automaticky dokončit tabulátorem

| Příkaz  | Co to dělá         |
| ------- | ------------------ |
| ls (-l) | list files         |
| cd      | change directory   |
| mkdir   | make directory     |
| clear   | vyčistí cmd line   |
| cp      | kopírování souborů |
| mv      | přesun souborů     |
| rm      | mazání souborů     |

## Souborové systémy na OS unixového typu
- používá se pro ukládání dat na disk, je to specifický způsob, ve kterém jsou data ukládána a umožňuje např. pojmenovávat soubory či stromovou strukturu
- FS na Linuxových systémech:
	- Extended File System (ext) - dnes verze ext4
	- Btrfs - snapshoty a copy-on-write (při vytvoření kopie se hned nevytvoří nová data, zkopírují se až když dojde k zápisu)
	- ZFS - podpora enormně velikých disků
- často podpora pro FAT32, NTFS, HFS+

## Organizace souborového systému
- na unixových systémech **je vše soubor nebo složka**

![](./UnixFS.png)
- souborové systémy se "mountují" do nějaké složky - hlavní disk se mountuje jako `/`, odnímatelné disky buď do `/mnt` nebo `/run/media`
- `/bin` obsahuje základní programy/příkazy OS jako /ls /pwd atd.
- `/boot` obsahuje soubory potřebné pro start počítače
	- často na jiném oddílu než zbytek systému