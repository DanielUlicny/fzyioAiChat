# Chat: Fyzio App – Príprava na prezentáciu pre fyzioterapeuta

**Dátum:** 15.–18. júna 2026

---

## Kontext

Príprava na videohovor s 26-ročným fyzioterapeutom, ktorý prejavil záujem o fyzioterapeutickú aplikáciu. Cieľom bolo pripraviť zrozumiteľné zhrnutie aplikácie a osnovu pre prezentáciu.

---

## O čom bol tento chat

Tento chat slúžil ako prípravný nástroj pred videohovorom s fyzioterapeutom. Prebehlo v ňom niekoľko kľúčových krokov:

1. **Popis aplikácie hlasom/textom** – autor podrobne popísal všetky funkcie webovej časti pre fyzioterapeuta aj mobilnej aplikácie pre pacienta, vrátane správy pacientov, programov, cvikov, fáz, hodnotiacich nástrojov a nastavení.
2. **Štruktúrovanie obsahu** – AI z dlhého, neformálneho opisu vytvorila prehľadné a zrozumiteľné zhrnutie aplikácie vhodné pre externého odborníka.
3. **Príprava hovorenej osnovy** – vytvorená osnova prezentácie (~3–5 minút), ktorú môže autor použiť priamo na videohovore.
4. **Identifikácia kľúčových otázok** – chat pomohol určiť, čo je podstatné pýtať sa fyzioterapeuta a aký feedback by bol pre vývoj najcennejší.

---

## Aplikácia – Prehľad

Dvojdielna platforma:
- **Web pre fyzioterapeuta** – správa pacientov, programov, cvikov, sledovanie progresu, hodnotiace nástroje
- **Mobilná appka pre pacienta** – cvičenie podľa videí, sledovanie plánu, záznam bolesti, dotazníky

---

## WEB PRE FYZIOTERAPEUTA – Detailný popis

### 1. Pacienti

#### Vytvorenie pacienta
- Fyzioterapeut zadá **meno** a **e-mail** pacienta.
- Systém automaticky vygeneruje **prístupový kód**, ktorý fyzioterapeut nadiktuje pacientovi.
- Pacient tento kód použije na prihlásenie do mobilnej aplikácie.

#### Detail pacienta – Karta „Pokrok" (Progres)
- Po otvorení pacienta vidí terapeut kartu s jeho pokrokom.
- **Sledované obdobia** (terapeut si môže prepínať): 7 dní, 30 dní, 3 mesiace, 12 mesiacov, celý čas
- **Adherence** – koľko dní za dané obdobie pacient cvičil a ako dodržiaval plán v percentách
- **Priebeh bolesti** – graf úrovne bolesti, ktorú pacient zadával každý deň (škála 0–10)
- **Hodnotiace nástroje (Outcome Measures)** – ak má program priradený hodnotiaci nástroj, zobrazí sa:
  - Posledné skóre
  - Predchádzajúce skóre
  - Zmena oproti poslednému meraniu
  - Interpretácia výsledku (napr. mierne obmedzenie / vážnejšie obmedzenie)
  - Tlačidlo na zobrazenie konkrétnych odpovedí pacienta na jednotlivé otázky dotazníka

#### Detail pacienta – Karta „Program"
- Terapeut vidí všetky programy priradené danému pacientovi.
- Pri každom programe je zobrazené: názov, fázy, trvanie, hodnotiaci nástroj, tvorca.
- **Rozvrh programu**: nastavenie minimálneho počtu tréningových dní za týždeň (rozsah 2–7) a odporúčaných dní (napr. pondelok, streda, piatok).
- Terapeut môže rozkliknúť jednotlivé fázy programu.

---

### 2. Programy

#### Knižnica programov
- Zobrazenie všetkých dostupných programov (vlastných aj firemných šablón).
- **Filtrovanie podľa stavu pacienta** (tzv. „condition"): napr. ACL tear, Achilles tendinopathy, Lateral ankle sprain, Rotator cuff repair a ďalšie.
- Každý program v zozname zobrazuje: názov, počet fáz, celkové trvanie, hodnotiaci nástroj, tvorca.
- Rovnako je tu tlačidlo **„Vytvoriť program"** – tvorba nového programu od nuly.

#### Priradenie programu pacientovi
- Terapeut môže pacientovi priradiť jeden alebo viacero programov.
- Pri pridaní programu sa ho systém opýta, ktorý program chce priradiť (výber z knižnice).
- Ak chce, môže ho pred priradením upraviť.

#### Úprava programu
Po kliknutí na „Upraviť program" má terapeut tieto možnosti:

**a) Hodnotiaci nástroj:**
- Výber alebo zmena outcome measure pre daný program.
- Nastavenie frekvencie – ako často sa má pacient dotazník pýtať (napr. raz za 2 týždne, raz za týždeň).
- Možnosť pridať viacero hodnotiacich nástrojov.

**b) Správa fáz:**
- Terapeut vidí jednotlivé fázy programu.
- Každá fáza má nastaviteľnú dĺžku: od 1 dňa po 13 (zobrazuje sa v dňoch), od 13 vyššie zobrazuje v týždňoch.
- **Opakovanie dní v rámci fázy**: dni v rámci fázy sa automaticky opakujú. Príklad: fáza má 2 dni cvičenia a trvá 1 týždeň → poradie bude Deň 1, Deň 2, Deň 1, Deň 2, Deň 1, Deň 2, Deň 1.
- Terapeut môže **posúvať poradie fáz** (napr. fázu 1 dať za fázu 2).
- Môže **pridávať nové fázy**.

**c) Správa dní a cvikov vo fáze:**
- Terapeut klikne na fázu a uvidí jednotlivé dni.
- Pri každom dni vidí priradené cviky.
- Akcie pri cvik v dni:
  - **Prehranie videa cviku** (hover nad cvikom = automatické prehrávanie náhľadu videa)
  - **Odstránenie cviku** (ikona koša)
  - **Pridanie cviku** – otvorí sa panel knižnice cvikov (viď sekcia Cviky)
  - **Klik na cvik** → otvorí detail, kde sa dá upraviť: počet sérií, počet opakovaní, čas, váha; uloženie zmien

#### Uloženie upraveného programu ako nový program
- Keď terapeut dokončí úpravu, môže program uložiť.
- Systém si vyžiada: **názov programu**, **variácia** (napr. stupeň závažnosti), **stav/diagnóza pacienta** (napr. Rotator cuff repair, Achilles tendinopathy – toto pole ešte môže byť upravené).
- Program sa uloží do knižnice ako nový záznam.

#### Vytvorenie programu od nuly
- Terapeut klikne na „Vytvoriť program" v knižnici programov.
- Zadá základné informácie: názov, stav pacienta (diagnóza/kondícia).
- Potom ho rovno môže upravovať rovnakým spôsobom ako existujúci program (fázy, dni, cviky).
- Po dokončení uloží → uloží sa ako nový program v knižnici.

---

### 3. Cviky

#### Knižnica cvikov
- Celkový počet: **700+ cvikov** (videá budú natočené postupne).
- Zobrazenie zoznamu cvikov s možnosťou:
  - **Hľadanie podľa názvu**
  - **Filtrovanie podľa**:
    - **Oblasť tela**: chodidlo a členok, koleno, bedrový kĺb, panvové dno, jadro, drieková chrbtica, hrudná chrbtica, krk, rameno, lakeť, zápästie a ruka
    - **Typ cviku**: sila, mobilita, uvoľnenie, rovnováha, skákanie, kardio
    - **Vybavenie**: žiadne, odporová guma, masážna loptička, činka, stroj, penový valec, gymnastická lopta, tyč, lavička
    - **Tvorca**: vlastné / firemné
    - **Obľúbené**: áno/nie
  - Po výbere filtra môže terapeut filtre vyčistiť jedným tlačidlom.

#### Interakcia s cvikom v knižnici
- **Hover nad cvikom** → automaticky sa prehrá náhľad videa cviku (bez kliknutia).
- **Klik na cvik (v karte)** → rozbalí sa detailný pohľad priamo v karte (bez nového okna):
  - Ukáže: počet sérií, počet opakovaní, čas trvania, váha
  - Popis cviku
  - Atribúty cviku (oblasť tela, typ, vybavenie)
- **Otvorenie plného detailu cviku**: pozrieť video, všetky parametre, pridať do obľúbených.

#### Tvorba vlastného cviku
- Terapeut klikne na „Vytvoriť cvik".
- Vyplní:
  - **Názov cviku**
  - **Variácia** (napr. s odporovou gumou, bez pomôcky)
  - **Stručný popis**
  - **Série** (počet)
  - **Opakovania** (počet)
  - **Čas** (trvanie cviku alebo série)
  - **Váha** (ak je relevantná)
  - **Pokyny pre pacienta** (textové inštrukcie)
  - **Typ cviku**: sila / mobilita / uvoľnenie / rovnováha / skákanie / kardio
  - **Oblasť tela**: chodidlo a členok / koleno / bedrový kĺb / panvové dno / jadro / drieková chrbtica / hrudná chrbtica / krk / rameno / lakeť / zápästie a ruka
  - **Vybavenie**: žiadne / odporová guma / masážna loptička / činka / stroj / penový valec / gymnastická lopta / tyč / lavička
  - **Nahranie videa** *(zatiaľ vo fáze rozhodovania – možno bude, možno nie)*

---

### 4. Hodnotiace nástroje (Outcome Measures)

#### Prehľad nástrojov
- Zoznam všetkých dostupných hodnotiacich nástrojov.
- Filtrovanie podľa kategórie.
- Každý nástroj v zozname: **názov**, **skratka**, **jazyk**.
- Aktuálne dostupné nástroje (príklady):
  - CSI – Dotazník centrálnej senzitizácie (SK)
  - PGQ – Pelvic Girdle Questionnaire (dotazník panvového pletenca)
  - (ďalšie budú pribúdať)

#### Detail hodnotiaceho nástroja
Po kliknutí na nástroj terapeut vidí:
- **Celý názov** (napr. Dotazník centrálnej senzitizácie) + **tag so skratkou** (napr. CSI)
- **Anglický názov** (napr. Central Sensitization Inventory)
- **Trvanie vyplnenia**: napr. 3–5 minút
- **Počet sekcií**: napr. 2
- **Tag** s interpretáciou smeru: napr. „Nižšie skóre = lepší zdravotný stav"
- **Informatívny text**: „Tento dotazník vyplní pacient vo svojej aplikácii. Skóre sa vypočíta automaticky. Táto obrazovka slúži len na náhľad štruktúry otázok a možností odpovede."
- **Popis nástroja**: napr. „Dotazník centrálnej senzitizácie pomáha zachytiť príznaky spojené s centrálnou senzitizáciou a súvisiacimi zdravotnými ťažkosťami. Celkové skóre sa udáva na škále od 0 do 100."
- **Štruktúra dotazníka** (rozbaľovacia):
  - Príklad – CSI:
    - **Časť A** (výber jednej odpovede): 25 otázok, zadanie „Vyberte prosím odpoveď, ktorá najlepšie vystihuje každé z nasledujúcich tvrdení."
      - Možnosti odpovede: Nikdy / Zriedka / Niekedy / Často / Vždy
      - Príklad otázky: „Cítim sa unavený/á a neoddýchnutý/á, keď sa zobudím."
    - **Časť B**: odlišný formát otázok (napr. áno/nie)
  - Pri každej časti je viditeľný počet otázok.

#### Výsledky hodnotiaceho nástroja pri pacientovi
- Fyzioterapeut vidí v detaile pacienta (karta Pokrok → sekcia Hodnotiace nástroje):
  - **Posledné skóre** (napr. 42 bodov alebo %)
  - **Predchádzajúce skóre**
  - **Zmena oproti poslednému meraniu** (napr. −8 bodov)
  - **Interpretačná stupnica** (napr. mierne obmedzenie / stredné / vážne)
  - **Zobrazenie odpovedí pacienta** – terapeut si môže pozrieť, na ktorú otázku pacient odpovedal ako, aby vedel, na čo sa zamerať pri ďalšej kontrole.

---

### 5. Spätná väzba

- Umiestnenie: rozbaľovacie menu v ľavom dolnom rohu aplikácie.
- Terapeut môže pridať:
  - **Screenshot alebo obrázok** (vloženie cez Ctrl+V alebo iný spôsob)
  - **Textový komentár** – čo by mohlo byť lepšie, čo nefunguje

---

### 6. Nastavenia profilu

- **Profilová fotka**
- **Celé meno**
- **E-mail**
- **Heslo** (zmena)

---

## MOBILNÁ APPKA PRE PACIENTA – Detailný popis

### 1. Prihlásenie

- Pacient zadá **prístupový kód** (vygenerovaný systémom, nadiktovaný fyzioterapeutom).
- Prihlási sa aj **e-mailom** a vytvorí si **heslo**.
- E-mail je priradený ku kódu → pri ďalšom prihlásení stačí e-mail + heslo (kód nie je potrebný opakovane).

---

### 2. Výber aktívneho programu

- Pri vstupe do appky vidí pacient všetky **aktívne programy**.
- Klikne na program, ktorý chce práve cvičiť.
- Systém ho zavedie na kartu **Domov** s daným programom.

---

### 3. Karta Domov

#### Horná lišta
- **Názov programu** (napr. Zlomenina zápästia) – kliknutím si pacient môže pozrieť prehľad svojich programov.
- **Fáza a postup**: napr. „Fáza 1 – 3. týždeň z 8"
- **Kruhový indikátor** (vpravo): zobrazuje, koľko cvičení za daný deň pacient splnil (napr. 2/4 cviky splnené → krúžok je z 50 % vyplnený).

#### Kalendár dní
- Horizontálny pás dní (napr. So, Ne, Po, Ut, St – s dátumami).
- Pri dňoch, kedy má pacient cvičiť podľa plánu, je **malá modrá bodka**.
- Kliknutím na deň sa zobrazí plán pre daný deň.

#### Dnešný plán
- Zobrazuje všetky cviky na daný deň.
- Hore je počítadlo splnených cvikov: napr. „1 zo 4".
- Každý cvik v zozname obsahuje:
  - **Miniatura videa** (malý obdĺžnik s ikonkou videa)
  - **Názov cviku** (napr. Pohyb zápästia do strán)
  - **Stručný popis** *(zatiaľ vo fáze rozhodovania – možno nebude)*
  - **Počet splnených sérií** (napr. 0/2)
  - **Trvanie** (napr. každá séria 30 sekúnd)
  - **Fajfka v štvorčeku** (vpravo) – klik = splní 1 sériu; ďalší klik = splní ďalšiu sériu; po splnení všetkých sérií = cvik sa označí ako odcvičený a počítadlo sa aktualizuje.

#### Odcvičené cviky
- Úplne dole pod aktívnymi cvikmi je sekcia **„Odcvičené"**.
- Pacient si môže zobraziť alebo skryť odcvičené cviky.
- Zobrazujú sa rovnaké informácie ako pri aktívnych cvikoch.

#### Skrytie cviku (Swipe doprava)
- Ak pacient potáhne cvik doprava, môže ho **skryť** (napr. keď ho bolí a nechce ho robiť).
- *Alternatíva vo vývoji*: možno sa toto nechá a pacient jednoducho cvik nerobí a nahlási to terapeutovi na kontrole.

---

### 4. Detail cviku

- Kliknutím na cvik sa otvorí celá karta s detailom.
- **Video na celú obrazovku** (alebo takmer celú) – je možné dať na fullscreen.
- Pod videom: **názov cviku**.
- **Fajfka** – označenie splnenia série.
- **Časovač** – ak je cvik na čas (napr. 30 sekúnd), zobrazí sa odpočítavač.
- **Zobrazenie úplného popisu cviku** – možnosť rozbaliť/zobraziť detailný popis a pokyny.

---

### 5. Karta Pokrok

#### Obdobia
- Prepínanie: **7 dní / 30 dní / 3 mesiace**

#### Štatistiky
- **Dodržiavanie plánu** v % (koľko dní pacient cvičil z plánovaných)
- **Počet dní cvičenia** (celkový počet dní, kedy pacient cvičil)
- **Počet splnených cvičení** (celkový počet odcvičených cvikov)
- **Graf priebehu bolesti** – vizualizácia denných záznamov pain level (0–10) za zvolené obdobie
- **Výsledky hodnotiacich nástrojov** – vývoj skóre v čase za zvolené obdobie

#### Denný záznam bolesti
- Pacient každý deň dostane otázku: **„Aká je tvoja bolesť?"** (hodnotí na škále 0–10).
- Tieto dáta sa zobrazujú v grafe pokroku.

#### Dotazníky (Outcome Measures)
- Pacient dostane dotazník v intervale nastavenom fyzioterapeutom (napr. raz za 2 týždne).
- Vypĺňa ho priamo v appke.
- Skóre sa vypočíta automaticky a odošle fyzioterapeutovi.

---

### 6. Karta Nastavenia

- **Informácie o fyzioterapeutovi**: meno, profilová fotka (ak je nastavená)
- **Aktívne programy**: zoznam momentálne priradených programov
- **Ukončené programy**: história programov, ktoré pacient absolvoval
- **Tréningové dni**:
  - Pacient si môže upraviť, ktoré dni chce cvičiť.
  - Vidí **minimum nastavené fyzioterapeutom** (napr. min. 4 dni/týždeň) – ak zadá menej, zobrazí sa upozornenie: „Váš fyzioterapeut stanovil minimálne 4 tréningové dni."
- **Čas pripomienky**: nastavenie, kedy chce pacient dostávať notifikáciu, že má cvičiť
- **Oznámenia**: správa notifikácií

---

## Čo od fyzioterapeuta potrebujeme

1. Či sú navrhnuté funkcie reálne užitočné v každodennej fyzioterapeutickej praxi
2. Či dáva zmysel rozsah knižnice cvikov a ich rozdelenie podľa oblasti tela, typu a vybavenia
3. Či sú predpripravené programy praktickejšie než tvorba vlastných plánov od nuly
4. Či sú outcome measures, sledovanie bolesti a adherence dostatočne hodnotné pre terapeuta
5. Čo v systéme chýba, aby bol naozaj použiteľný v reálnej ambulancii
6. Či by takýto systém šetril čas a pomáhal pri práci s pacientmi

---

## Osnova pre prezentáciu (hovorená)

### 1. Otvorenie (~30 sek)
> Dobrý deň, chcel by som vám stručne ukázať náš návrh digitálnej fyzioterapeutickej platformy. Ide o systém, ktorý má dve časti: webovú aplikáciu pre fyzioterapeuta a mobilnú aplikáciu pre pacienta. Cieľom je zjednodušiť domácu terapiu, zlepšiť prehľad o tom, čo pacient reálne robí, a umožniť lepšie sledovanie progresu. A od vás by sme privítali hlavne praktický pohľad z ambulancie – nie len pochvalu, ale aj kritiku.

### 2. Problém (~30 sek)
> Pacienti doma často necvičia pravidelne alebo nevedia presne, čo robiť. Fyzioterapeut potom nevidí, ako pacient dodržiava plán, akú má bolesť, ani ako sa mení jeho stav medzi kontrolami. Naše riešenie je platforma, kde terapeut nastaví plán a pacient ho v mobile jednoducho sleduje, cvičí podľa videí a zapisuje plnenie.

### 3. Web pre terapeuta (~1 min)
- Terapeut si vytvorí pacienta a priradí mu program.
- K dispozícii bude 700+ cvikov s videami – dajú sa filtrovať podľa oblasti tela, typu cviku a vybavenia.
- Programy budú predpripravené, takže nemusí všetko vytvárať od nuly, ale vie ich prispôsobiť konkrétnemu pacientovi.
- V detaile pacienta vidí: adherence, priebeh bolesti a výsledky hodnotiacich dotazníkov.

### 4. Mobil pre pacienta (~30 sek)
- Pacient dostane kód, prihlási sa do appky.
- Vidí dnešný plán, cvičí podľa videí, označuje splnenie každej série.
- Každý deň zadáva úroveň bolesti, v nastavených intervaloch vypĺňa dotazníky.
- Terapeut dostáva späť reálne údaje o tom, čo pacient robí.

### 5. Záver + otázky (~30 sek)
> Najviac by nás zaujímalo, či by vám takýto systém reálne šetril čas a pomáhal pri práci s pacientmi. Máte nejaké otázky alebo nápady, čo by malo byť inak, čo vám tam chýba alebo čo je naopak zbytočné?

---

Dátum: 23. júna 2026
Kontext

Systematické získavanie povolení na použitie validovaných hodnotiacich nástrojov (outcome measures) pre digitálnu fyzioterapeutickú platformu. Kontaktovanie autorov jednotlivých dotazníkov s cieľom zabezpečiť právne a eticky správne používanie nástrojov vrátane slovenských prekladov.

O čom bol tento chat

Chat slúžil na prípravu a odoslanie žiadostí o povolenie pre každý outcome measure a na spracovanie prichádzajúcich odpovedí.

Príprava mailov – Pre každý nástroj bol pripravený individuálny mail s konzistentnou štruktúrou: predstavenie projektu SOČ, konkrétna žiadosť o povolenie na použitie a preklad, záväzky voči autorom, otázky k licencii.

Riešenie nedoručených mailov – Pri viacerých nástrojoch boli staré kontaktné adresy nefunkčné (LEFS, PGQ, RMDQ) a boli vyhľadané aktuálne kontakty.

Spracovanie odpovedí – Prišli odpovede od Dr. Martina Rolanda (RMDQ) a Dr. Britt Stugeovej (PGQ); obe boli zodpovedané.

Identifikácia nástrojov nevyžadujúcich povolenie – RMDQ a RAND-36 sú verejná doména; pre oba boli identifikované správne citácie.

Prehľad kontaktovaných autorov

Nástroj	Autor	Kontakt	Stav
HOOS-JR / KOOS-JR	HOOS/KOOS Research Team (HSS)	hooskoos@hss.edu	✉️ odoslané
LEFS	Jill M. Binkley	jill@jmbinkley.com	✉️ odoslané (2 z 3 adries nedoručené)
UEFI-15	Jill M. Binkley	jill@jmbinkley.com	✉️ odoslané (follow-up)
PGQ	Britt Stuge	britt.stuge@outlook.com	✅ odpoveď – kontaktovať Magdalenu Hagovskú (UPJŠ)
PGQ – SK preklad	Magdalena Hagovská	magdalena.hagovska@upjs.sk	✉️ odoslané
RMDQ	Martin Roland	mr108@cam.ac.uk	✅ odpoveď – verejná doména, prekladaj voľne
SPADI	Kathryn Roach	keroach@miami.edu	✉️ odoslané
VISA-A	Victorian Institute of Sport	research@vis.org.au	✉️ odoslané
RAND-36	RAND Corporation	–	✅ verejná doména – povolenie nie je potrebné
RAND-36	RAND Corporation	–	✅ citácia: Hays et al., 1993
Kľúčové zistenia

RMDQ aj RAND-36 sú verejná doména — nevyžadujú povolenie ani na preklad.

Preklad každého nástroja je potrebné robiť štandardizovaným postupom (forward → back-translation → expert review → pilotný test), bez ohľadu na to, či je nástroj chránený alebo verejný.

Pilotné testovanie zrozumiteľnosti (kognitívny pilotný test) stačí na 5–10 ľuďoch celkovo pre všetky nástroje; psychometrická validácia je odložená na budúci výskum.

UEFI-15 (Rasch-validovaná 15-položková verzia) je odporúčaná pre platformu oproti staršej UEFI-20.

Rehabot (slovenská konkurenčná platforma) bol kontaktovaný a ochotne poskytne screenshoty a video ukážky pre teoretickú časť SOČ.

Generované a doplnené pomocou Perplexity AI
