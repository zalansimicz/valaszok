
Tesztelési alapok (ISTQB-hez kapcsolódó)
✅ Mi a tesztelés célja? Mi nem az?
Célja:
Hibák felderítése a szoftverben.
Annak ellenőrzése, hogy a szoftver megfelel-e a követelményeknek.
Információ szolgáltatása a szoftver minőségéről a döntéshozók számára.
Bizalom növelése a szoftver minőségében.
Hibák megelőzése (a tesztelési folyamat és a tapasztalatok révén).
Nem célja:
Annak bizonyítása, hogy a szoftver hibátlan (ez gyakorlatilag lehetetlen, kivéve nagyon egyszerű eseteket).
A szoftver minőségének javítása (a tesztelés hibákat tár fel, de a javítás a fejlesztők feladata).
A fejlesztés helyettesítése.
✅ Mik a tesztelési alapelvek?
Az ISTQB (International Software Testing Qualifications Board) szerint a tesztelés hét alapelve van:

A tesztelés hibákat tár fel, nem a hiányukat bizonyítja: A tesztelés csökkentheti a szoftverben maradó felderítetlen hibák valószínűségét, de még ha nem is találunk hibát, az nem bizonyítja a hibátlanságot.
A kimerítő tesztelés lehetetlen: Minden lehetséges bemeneti kombináció és előfeltétel tesztelése (kivéve a triviális eseteket) nem valósítható meg. Ehelyett kockázatelemzést és prioritásokat kell alkalmazni a tesztelési erőfeszítések összpontosításához.
Korai tesztelés időt és pénzt takarít meg: A szoftverfejlesztési életciklusban minél korábban kezdődik a tesztelés (és a hibajavítás), annál olcsóbb.
A hibák csoportosulnak: A hibák jellemzően nem egyenletesen oszlanak el a szoftverben, hanem bizonyos modulokban vagy területeken koncentrálódnak (Pareto-elv, 80/20 szabály).
Pesticid-paradoxon: Ha ugyanazokat a teszteket ismételten futtatjuk, egy idő után ezek a tesztek már nem találnak új hibákat. A teszteseteket rendszeresen felül kell vizsgálni és frissíteni kell, valamint új teszteket kell írni.
A tesztelés kontextusfüggő: Különböző kontextusokban (pl. biztonságkritikus szoftver vs. e-kereskedelmi weboldal) eltérő módon kell tesztelni.
A hibamentesség téveszméje: Attól, hogy egy szoftver hibamentes, még nem biztos, hogy használható vagy megfelel a felhasználói igényeknek. A hibák felderítése és javítása haszontalan, ha a rendszer a rossz követelmények alapján épült.
✅ Mi az egységtesztelés (unit testing)? Ki felelős az egységtesztek írásáért?
Egységtesztelés: A szoftver legkisebb tesztelhető részeit, azaz egységeit (modulok, osztályok, függvények) izoláltan teszteli. Célja annak ellenőrzése, hogy az adott egység a specifikációnak megfelelően működik-e.
Felelős: Általában maguk a fejlesztők felelősek az egységtesztek megírásáért, mivel ők ismerik legjobban a kód belső működését. Ez gyakran a "tesztvezérelt fejlesztés" (TDD) része.
✅ Mik a tesztszintek, és mi a különbség köztük?
A tesztelés különböző szinteken történik a szoftverfejlesztési életciklus során:

Egységtesztelés (Unit Testing):
Fókusz: Egyedi komponensek, modulok, osztályok vagy függvények.
Cél: Annak ellenőrzése, hogy minden egyes kódrészlet helyesen működik-e önmagában.
Végzi: Általában fejlesztők.
Integrációs tesztelés (Integration Testing):
Fókusz: Az egységek közötti interfészek és interakciók.
Cél: Annak ellenőrzése, hogy a különböző komponensek megfelelően együttműködnek-e, miután integrálták őket. Lehet komponensintegrációs (egységek közötti) vagy rendszerintegrációs (rendszerek közötti) tesztelés.
Végzi: Fejlesztők vagy tesztelők.
Rendszertesztelés (System Testing):
Fókusz: A teljes, integrált rendszer viselkedése.
Cél: Annak ellenőrzése, hogy a teljes rendszer megfelel-e a specifikált követelményeknek. Ez egy fekete dobozos tesztelési technika.
Végzi: Általában független tesztelő csapat.
Elfogadási tesztelés (Acceptance Testing):
Fókusz: A rendszer megfelel-e a felhasználói igényeknek és az üzleti követelményeknek.
Cél: Annak eldöntése, hogy a szoftver elfogadható-e a kibocsátásra vagy használatba vételre.
Végzi: Végfelhasználók, ügyfelek vagy a terméktulajdonos. Típusai:
Felhasználói elfogadási teszt (UAT)
Üzleti elfogadási teszt (BAT)
Alfa tesztelés (fejlesztői környezetben, belső csapat által)
Béta tesztelés (valós felhasználói környezetben, külső felhasználók által)
Különbségek: A szintek az ellenőrzés hatókörében, céljában, a tesztkörnyezetben és a végrehajtókban térnek el. Ahogy haladunk felfelé a szinteken, a tesztelés fókusza az egyedi komponensektől a teljes rendszerig és annak üzleti megfelelőségéig terjed.

✅ Mi a különbség a verifikáció és a validáció között?
Verifikáció (Verification): "Jól építjük a terméket?"
Annak ellenőrzése, hogy a szoftver megfelel-e a specifikációknak és a tervezési dokumentumoknak.
Fókuszban a belső konzisztencia és a helyes implementáció.
Tipikus kérdés: "A szoftver a specifikáció szerint működik?"
Általában statikus tesztelési technikákat (pl. kódellenőrzés, walkthrough) és dinamikus tesztelést is magában foglal a fejlesztési fázisok során (pl. egységtesztek, integrációs tesztek).
Validáció (Validation): "A jó terméket építjük?"
Annak ellenőrzése, hogy a szoftver megfelel-e a felhasználói igényeknek és az elvárásoknak.
Fókuszban a külső megfelelőség és a használhatóság.
Tipikus kérdés: "Ez az, amit a felhasználó akart?"
Általában a fejlesztési ciklus későbbi szakaszaiban történik (pl. rendszertesztelés, elfogadási tesztelés).
Röviden: a verifikáció arról szól, hogy a szoftvert helyesen építjük-e, míg a validáció arról, hogy a helyes szoftvert építjük-e.

✅ Mik a tesztelési típusok, és mi a különbség köztük?
A tesztelési típusok a tesztelés konkrét céljai vagy jellemzői alapján csoportosíthatók. A fő kategóriák:

Funkcionális tesztelés:
Cél: Annak ellenőrzése, hogy a szoftver funkciói a specifikációknak megfelelően működnek-e ("mit csinál a rendszer").
Példák: Egységtesztelés, integrációs tesztelés, rendszertesztelés, elfogadási tesztelés (bizonyos részei), regressziós tesztelés, füsttesztelés.
Nem-funkcionális tesztelés:
Cél: A szoftver minőségi jellemzőinek tesztelése ("hogyan működik a rendszer").
Példák:
Teljesítménytesztelés: Sebesség, válaszidő, stabilitás, skálázhatóság terhelés alatt (terheléses tesztelés, stressztesztelés, tartóssági tesztelés).
Használhatósági tesztelés: Mennyire könnyen használható, intuitív a rendszer a végfelhasználó számára.
Biztonsági tesztelés: Sebezhetőségek, adatintegritás, hozzáférés-szabályozás vizsgálata.
Megbízhatósági tesztelés: A szoftver képessége a hibamentes működésre adott időtartamon keresztül.
Karbantarthatósági tesztelés: Mennyire könnyen módosítható, javítható a szoftver.
Hordozhatósági tesztelés: Mennyire könnyen vihető át a szoftver egyik környezetből a másikba.
Strukturális (fehér dobozos) tesztelés:
Cél: A szoftver belső szerkezetének, kódjának vizsgálata. Lásd a fehér dobozos tesztelésnél.
Változásokhoz kapcsolódó tesztelés:
Cél: Annak biztosítása, hogy a kód módosításai (hibajavítások, új funkciók) nem okoztak-e új hibákat, vagy nem rontották-e el a meglévő funkciókat.
Példák: Újratesztelés (re-testing), regressziós tesztelés.
Különbségek: A típusok abban különböznek, hogy a szoftver melyik aspektusát vizsgálják (funkció, teljesítmény, biztonság stb.), és milyen céllal tesznek (hibakeresés, minőségbiztosítás, megfelelőség ellenőrzése).

✅ Mi a különbség a fehér doboz, szürke doboz és fekete doboz tesztelés között?
Ezek a tesztelési technikák a tesztelő tudásszintje alapján különböznek a rendszer belső működéséről:

Fekete doboz tesztelés (Black-box testing):
Ismeret: A tesztelő nem ismeri a rendszer belső szerkezetét, kódját, architektúráját. Csak a bemeneteket és a várt kimeneteket ismeri.
Fókusz: A szoftver funkcionalitásának ellenőrzése a felhasználói felületen vagy API-n keresztül, a specifikációk alapján.
Előnyök: Felhasználói szemszögből tesztel, a tesztesetek függetlenek a kódtól.
Hátrányok: Nem minden kódrészlet kerülhet lefedésre, bizonyos hibatípusok nehezebben találhatók meg.
Példák: Ekvivalencia particionálás, határérték-elemzés, döntési tábla tesztelés.
Fehér doboz tesztelés (White-box testing / Glass-box testing):
Ismeret: A tesztelő teljes mértékben ismeri a rendszer belső szerkezetét, kódját, logikáját, architektúráját.
Fókusz: A kód útvonalainak, elágazásainak, ciklusainak és belső logikájának tesztelése.
Előnyök: Magas kódfedettség érhető el, optimalizálható a kód, rejtett hibák is feltárhatók.
Hátrányok: A tesztesetek erősen kötődnek a kódhoz (módosítás esetén frissíteni kell), a hiányzó funkcionalitást nem tárja fel.
Példák: Utasításfedettség, elágazásfedettség, útvonalfedettség. Tipikusan egységtesztelésnél használatos.
Szürke doboz tesztelés (Grey-box testing):
Ismeret: A tesztelő részleges ismeretekkel rendelkezik a rendszer belső működéséről (pl. adatbázis séma, algoritmusok alapelvei), de nem ismeri a forráskódot teljes mélységében.
Fókusz: Funkcionális tesztelés, de a belső ismeretek birtokában hatékonyabb tesztesetek tervezhetők. Ötvözi a fekete és fehér dobozos tesztelés előnyeit.
Előnyök: Jobb tesztlefedettség, mint a fekete doboznál, anélkül, hogy a kód minden részletét ismerni kellene.
Hátrányok: A tesztelőnek rendelkeznie kell bizonyos szintű belső ismeretekkel.
Példák: API tesztelés, adatbázis integritásának ellenőrzése a funkciók tesztelése során.
✅ Mi a különbség a felhasználói elfogadási teszt (UAT) és a rendszerteszt között?
Jellemző	Rendszertesztelés (System Testing)	Felhasználói Elfogadási Teszt (UAT)
Cél	Annak ellenőrzése, hogy a teljes integrált rendszer megfelel-e a specifikált követelményeknek.	Annak ellenőrzése, hogy a rendszer megfelel-e a felhasználói igényeknek és üzleti követelményeknek, és használatra kész-e.
Ki végzi?	Általában független tesztelő csapat (a fejlesztőktől elkülönülve).	Végfelhasználók, ügyfelek, terméktulajdonosok, üzleti elemzők.
Mikor?	Az integrációs tesztelés után, de az elfogadási tesztelés előtt.	A rendszertesztelés után, közvetlenül a szoftver kiadása előtt.
Fókusz	Funkcionális és nem-funkcionális követelmények teljesítése.	Üzleti folyamatok, valós felhasználási esetek, használhatóság.
Környezet	Tesztkörnyezet, amely a lehető legjobban hasonlít az éles környezetre.	Gyakran éleshez közeli vagy éles környezet (pl. béta tesztelésnél).
Alapja	Rendszerkövetelmények, specifikációk, tervezési dokumentumok.	Felhasználói történetek, üzleti követelmények, valós forgatókönyvek.
Tesztelési típus	Főként fekete dobozos tesztelés.	Fekete dobozos tesztelés.

Exportálás Táblázatok-fájlba
Röviden: a rendszertesztelés azt vizsgálja, hogy a rendszer a specifikációknak megfelelően épült-e, míg az UAT azt, hogy a rendszer megfelel-e a felhasználó céljainak és használható-e a valós világban.

✅ Sorolj fel különbségeket a regressziós tesztelés, a füsttesztelés és az újratesztelés között!
Jellemző	Regressziós tesztelés (Regression Testing)	Füsttesztelés (Smoke Testing / Build Verification Test)	Újratesztelés (Re-testing / Confirmation Testing)
Cél	Annak ellenőrzése, hogy a kód módosításai (új funkciók, hibajavítások) nem rontották-e el a meglévő, korábban működő funkciókat.	Annak gyors ellenőrzése, hogy a szoftver legkritikusabb funkciói működnek-e egy új build telepítése után, és a build elég stabil-e a további, részletesebb teszteléshez.	Annak ellenőrzése, hogy egy korábban jelentett és kijavított hiba valóban megjavult-e.
Mikor?	Kódmódosítások (új funkciók, hibajavítások, konfigurációváltozások) után.	Minden új build/verzió telepítésekor, a részletesebb tesztek előtt.	Egy konkrét hiba javítása után.
Hatókör	A teljes alkalmazás vagy annak érintett részei. Lehet teljes vagy részleges.	A szoftver alapvető, legfontosabb funkcióira korlátozódik. Széles, de sekély.	Csak a korábban hibásan működő funkcióra vagy komponensre fókuszál.
Ki végzi?	Tesztelők, automatizált tesztek.	Tesztelők, fejlesztők, automatizált szkriptek.	Tesztelők.
Tesztkészlet	Előre definiált regressziós tesztkészlet (manuális vagy automatizált).	Kis, gyorsan futtatható tesztkészlet a kritikus útvonalakra.	A hibát eredetileg reprodukáló teszteset(ek).
Eredmény	Biztosítja, hogy a meglévő funkcionalitás továbbra is működik.	Eldönti, hogy a build elfogadható-e a további tesztelésre.	Megerősíti a hibajavítás sikerességét.

Exportálás Táblázatok-fájlba
✅ Mi a különbség a statikus és dinamikus tesztelés között?
Jellemző	Statikus tesztelés (Static Testing)	Dinamikus tesztelés (Dynamic Testing)
Definíció	A szoftvertermék vizsgálata a kód futtatása nélkül.	A szoftvertermék vizsgálata a kód futtatása közben.
Cél	Hibák korai felderítése a dokumentumokban (követelmények, design) és a kódban, a minőség javítása.	Hibák felderítése a szoftver futása során, a viselkedés ellenőrzése.
Mikor?	A fejlesztési ciklus korai szakaszaitól kezdve, a kódolás előtt és alatt is.	A kód elkészülte után, a tesztelési fázisokban.
Mit vizsgál?	Forráskód, tervezési dokumentumok, követelményspecifikációk, teszttervek, felhasználói útmutatók stb.	A szoftver bemeneteit, kimeneteit, teljesítményét, viselkedését.
Technikák	Kódellenőrzés (review), walkthrough, inspekció, statikus kódelemzés (automatizált eszközökkel).	Egységtesztelés, integrációs tesztelés, rendszertesztelés, UAT, funkcionális és nem-funkcionális tesztek.
Hibák típusa	Szintaktikai hibák, kódolási szabványok megsértése, tervezési hibák, követelménybeli hiányosságok, karbantarthatósági problémák.	Futásidejű hibák, teljesítményproblémák, helytelen kimenetek, biztonsági rések, memória szivárgás.
Előnyök	Korai hibafelismerés (olcsóbb javítás), hibamegelőzés, jobb dokumentáció.	Valós működés közbeni hibák feltárása, a rendszer egészének vizsgálata.
Korlátok	Nem talál futásidejű hibákat, a tesztelő szubjektivitása befolyásolhatja.	Későbbi fázisban talál hibákat (drágább javítás), időigényes lehet.

Exportálás Táblázatok-fájlba
✅ Hasonlítsd össze a V-modellt, a vízesés modellt és az Agile megközelítést a tesztelés szempontjából!
Jellemző	Vízesés modell	V-modell	Agile megközelítés
Tesztelés kezdete	A fejlesztési fázisok befejezése után, a ciklus végén kezdődik a dedikált tesztelési fázis.	Minden fejlesztési fázishoz párhuzamosan hozzárendel egy tesztelési szintet. A tesztelés tervezése korán kezdődik, a végrehajtás később.	A tesztelés a fejlesztéssel párhuzamosan, folyamatosan zajlik minden iterációban (sprintben).
Tesztelési szintek	Általában a végén van egy nagyobb rendszertesztelési és elfogadási tesztelési fázis.	Egyértelműen definiálja a tesztelési szinteket (egység, integráció, rendszer, elfogadás) és összekapcsolja őket a megfelelő fejlesztési fázisokkal.	Minden szintű tesztelés (egység, integráció, rendszer, elfogadás) jelen van az iterációk során, gyakran automatizáltan.
Visszacsatolás	Késői visszacsatolás, a hibák felfedezése és javítása költséges lehet.	Korábbi visszacsatolás a verifikációs és validációs tevékenységek révén minden fázisban, de a tényleges tesztelés még szekvenciális.	Gyors és folyamatos visszacsatolás az iterációk során, ami lehetővé teszi a korai hibajavítást.
Rugalmasság a változásokra	Kevésbé rugalmas, a követelmények változása nehezen kezelhető a késői fázisokban.	Kevésbé rugalmas, mint az Agile, mivel a fázisok szekvenciálisak, de a korai teszttervezés segít.	Nagyon rugalmas, jól kezeli a változó követelményeket az iteratív fejlesztésnek köszönhetően.
Tesztelők bevonása	A tesztelők általában a fejlesztés vége felé kapcsolódnak be.	A tesztelők korábban bevonódnak a teszttervezési és előkészítési tevékenységekbe.	A tesztelők a kezdetektől fogva szerves részei a fejlesztői csapatnak (cross-functional team).
Dokumentáció	Általában részletes, átfogó dokumentációra támaszkodik.	Részletes dokumentációt igényel, különösen a tesztterveket és specifikációkat.	Kevesebb hangsúly a formális dokumentáción, inkább a működő szoftver és a közvetlen kommunikáció a fontos.
Hibajavítás	A hibák javítása a tesztelési fázisban történik, ami költséges lehet, ha alapvető tervezési hibákról van szó.	A hibák korábban azonosíthatók a verifikáció során, de a javításuk még mindig a későbbi fázisokra maradhat.	A hibákat az adott iteráción belül vagy a következőben gyorsan javítják.
Fókusz	A teljes projekt egyben történő leszállítására fókuszál.	A verifikációra és validációra helyezi a hangsúlyt minden fejlesztési lépésnél.	Működő szoftver inkrementális szállítása, folyamatos fejlesztés és tesztelés.

Exportálás Táblázatok-fájlba
Reporting, Bugs
✅ Milyen lépéseket követnél egy hiba megtalálásakor?
Reprodukálás: Próbáld meg többször előidézni a hibát, hogy biztos legyél benne, és megértsd a körülményeket. Jegyezd fel a pontos lépéseket.
Izolálás: Szűkítsd le a hiba okát. Változtass egy dolgot egyszerre, hogy kiderüljön, mi váltja ki a hibát (pl. más böngésző, más adatok, más felhasználói fiók).
Dokumentálás (Hibajelentés készítése): Készíts részletes hibajelentést. (Lásd a következő kérdést a tartalmáról.)
Ellenőrzés (létezik-e már): Nézd meg a hibakövető rendszerben, hogy nem jelentették-e már ezt a hibát korábban.
Jelentés: Rögzítsd a hibát a használt hibakövető rendszerben (pl. Jira, Bugzilla).
Súlyosság és prioritás meghatározása (ha ez a te feladatod): Javaslatot tehetsz a hiba súlyosságára és prioritására. Ezt általában a terméktulajdonos vagy a projektmenedzser véglegesíti.
Kommunikáció: Értesítsd a releváns személyeket (pl. fejlesztő, projektmenedzser) a hibáról, ha szükséges.
Nyomon követés: Kövesd nyomon a hiba állapotát a hibakövető rendszerben, és végezd el az újratesztelést, miután a fejlesztők jelezték, hogy javították.
✅ Beszélj a gyakori tesztjelentésekről és részleteikről!
A tesztjelentések célja, hogy tájékoztatást adjanak a tesztelési folyamat állapotáról, eredményeiről és a szoftver minőségéről. Néhány gyakori típus:

Tesztelési Összefoglaló Jelentés (Test Summary Report):
Cél: Átfogó képet ad egy tesztelési ciklus vagy projekt végén.
Tartalma:
Projekt neve, tesztelt verzió.
Tesztelési időszak.
Összes futtatott teszteset száma.
Sikeres tesztesetek száma és aránya.
Sikertelen tesztesetek száma és aránya.
Blokkolt tesztesetek száma.
Nyitott, javított, lezárt hibák száma (súlyosság szerint bontva).
Tesztfedettség (ha mérhető).
Felmerült kockázatok és problémák.
Következtetések és javaslatok (pl. kiadásra javasolt-e a szoftver).
Tesztelési környezet részletei.
Napi/Heti Tesztelési Státusz Jelentés (Daily/Weekly Test Status Report):
Cél: Rendszeres frissítést ad a tesztelés előrehaladásáról.
Tartalma:
Jelentési időszak.
Elvégzett feladatok az adott időszakban.
Tervezett feladatok a következő időszakra.
Futtatott tesztesetek száma (sikeres/sikertelen).
Újonnan talált hibák.
Akadályok, problémák.
Hibajelentés (Bug Report / Defect Report):
Cél: Egy konkrét hiba részletes leírása. (Lásd következő kérdés.)
Tesztfedettségi Jelentés (Test Coverage Report):
Cél: Megmutatja, hogy a követelmények, funkciók vagy kódrészletek mekkora részét fedték le a tesztesetek.
Tartalma:
Követelmények/funkciók listája.
Hozzájuk rendelt tesztesetek.
Lefedett/nem lefedett elemek aránya.
Automatizált eszközök által generált kódfedettségi mutatók (pl. utasítás-, elágazásfedettség).
Automatizált Tesztfuttatási Jelentés (Automated Test Execution Report):
Cél: Az automatizált tesztek futtatásának eredményeit mutatja be.
Tartalma:
Futtatás időpontja, időtartama.
Futtatott tesztek listája.
Sikeres/sikertelen tesztek.
Hibaüzenetek, logok, képernyőképek sikertelenség esetén.
Teljesítménymutatók (pl. futási idők).
✅ Mit tartalmaz egy hibajelentés?
Egy jó hibajelentés egyértelmű, tömör, reprodukálható és teljes. Alapvető elemei:

Egyedi Azonosító (ID): Automatikusan generálja a hibakövető rendszer.
Összegzés/Cím (Summary/Title): Rövid, lényegre törő leírás a hibáról (pl. "Bejelentkezés gomb nem működik Firefox böngészőben").
Leírás (Description): Részletesebb leírás a hibáról, mi történt.
Reprodukálás Lépései (Steps to Reproduce): Pontos, sorszámozott lépések, amelyekkel a hiba előidézhető.
Tényleges Eredmény (Actual Result): Mi történt a lépések végrehajtása után.
Várt Eredmény (Expected Result): Minek kellett volna történnie a specifikáció vagy a józan ész alapján.
Súlyosság (Severity): A hiba hatása a szoftver működésére (pl. Kritikus, Magas, Közepes, Alacsony, Kozmetikai).
Kritikus: A rendszer használhatatlan, adatvesztés történik, nincs kerülőút.
Magas: Egy fontos funkció nem működik, vagy jelentősen akadályozza a használatot, de van kerülőút.
Közepes: Kisebb funkció nem működik megfelelően, vagy a felhasználói élményt rontja, de a fő funkciók használhatók.
Alacsony: Kisebb hiba, ami nem befolyásolja a funkcionalitást jelentősen (pl. elírás a felületen).
Prioritás (Priority): A hiba javításának sürgőssége üzleti szempontból (pl. Magas, Közepes, Alacsony). Ezt gyakran a terméktulajdonos vagy projektmenedzser határozza meg.
Környezet (Environment): A rendszer és a környezet részletei, ahol a hibát észlelték (pl. operációs rendszer, böngésző verziója, eszköz típusa, szerver környezet, szoftver verziója).
Csatolmányok (Attachments): Képernyőképek, videók, log fájlok, amelyek segítenek a hiba megértésében és reprodukálásában.
Jelentő (Reported by): Ki jelentette a hibát.
Dátum (Date Reported): Mikor jelentették a hibát.
Státusz (Status): A hiba aktuális állapota (pl. Új, Megnyitva, Folyamatban, Javítva, Újratesztelésre vár, Lezárva, Elutasítva).
✅ Hogyan rangsorolnál egy hibát?
A hibák rangsorolása általában két dimenzió mentén történik: súlyosság (severity) és prioritás (priority).

Súlyosság (Severity):
Meghatározása: A tesztelő vagy a QA csapat határozza meg.
Szempont: A hiba technikai hatása a szoftver működésére. Mennyire akadályozza a funkcionalitást, okoz-e adatvesztést, rendszerösszeomlást stb.
Szintek (példák):
Kritikus (Critical/Blocker): A szoftver fő funkcionalitása használhatatlan, a rendszer összeomlik, adatvesztés történik, nincs kerülőút.
Magas (High/Major): Egy fontos funkció nem működik, vagy jelentősen akadályozza a használatot, de esetleg van kerülőút.
Közepes (Medium/Moderate): Kisebb funkció nem működik megfelelően, vagy a felhasználói élményt rontja, de a fő funkciók használhatók. Kellemetlenséget okoz.
Alacsony (Low/Minor): Kisebb hiba, ami nem befolyásolja a funkcionalitást jelentősen (pl. elírás a felületen, kisebb UI/UX probléma).
Kozmetikai (Cosmetic/Trivial): Nagyon apró esztétikai hiba, ami alig észrevehető.
Prioritás (Priority):
Meghatározása: Általában a terméktulajdonos (Product Owner), projektmenedzser vagy üzleti elemző határozza meg, gyakran a tesztelő javaslata alapján.
Szempont: A hiba javításának üzleti sürgőssége. Milyen gyorsan kell kijavítani a hibát az üzleti célok, a felhasználói hatás, a határidők stb. figyelembevételével.
Szintek (példák):
Azonnali (Urgent/Highest): Azonnal javítani kell, mert blokkolja a fejlesztést, tesztelést, vagy súlyos üzleti kárt okoz.
Magas (High): A lehető leghamarabb javítani kell, általában a következő release ciklusban.
Közepes (Medium): A normál fejlesztési ütemterv szerint javítandó.
Alacsony (Low): Akkor javítandó, ha van rá idő és erőforrás, nem sürgős.
A rangsorolás folyamata:

Súlyosság megállapítása: A tesztelő a technikai impakt alapján besorolja a hibát.
Prioritás megállapítása: A felelős személy (pl. PO) a súlyosságot, az üzleti hatást, a felhasználói visszajelzéseket, a javítás költségét/idejét és a projekt céljait figyelembe véve meghatározza a prioritást.
Fontos megjegyezni, hogy a magas súlyosság nem mindig jelent magas prioritást, és fordítva:

Magas súlyosság, alacsony prioritás: Pl. egy ritkán használt funkcióban van egy kritikus hiba, ami összeomlasztja a rendszert, de mivel alig használják, a javítása nem sürgős.
Alacsony súlyosság, magas prioritás: Pl. egy elírás a cég logójában a főoldalon. Technikailag alacsony súlyosságú, de üzletileg kínos, ezért magas prioritással kell javítani.
Test Automation, Selenium
✅ Melyik teszteseteket érdemes automatizálni és melyiket nem?
Érdemes automatizálni:

Ismétlődő tesztek: Amelyeket minden build, release vagy kódmódosítás után futtatni kell (pl. regressziós tesztek, füsttesztek).
Nagy adatmennyiséggel dolgozó tesztek (Data-Driven Tests): Amikor ugyanazt a tesztlogikát sok különböző adatbeállítással kell futtatni.
Kritikus útvonalak (Critical Path Tests): A szoftver legfontosabb funkcióit ellenőrző tesztek, amelyeknek mindig működniük kell.
Időigényes manuális tesztek: Amelyek manuálisan sokáig tartanak, de automatizálva gyorsan lefutnak.
Stabil funkciók tesztjei: Olyan funkciók, amelyek ritkán változnak, így az automatizált szkriptek karbantartási igénye alacsony.
Párhuzamosan futtatható tesztek: Különböző böngészőkön, eszközökön, operációs rendszereken (cross-browser, cross-platform testing).
Nem-funkcionális tesztek: Teljesítménytesztek, terheléses tesztek, stressztesztek.
API tesztek: Gyorsak, stabilak és korai visszajelzést adnak a rendszer állapotáról a UI réteg nélkül.
Matematikai számításokat, adatellenőrzést végző tesztek: Ahol a pontosság kritikus és az emberi hiba lehetősége magas.
Nem (vagy kevésbé) érdemes automatizálni:

Ritkán futtatandó tesztek: Amelyeket csak egyszer vagy nagyon ritkán kell végrehajtani (pl. exploratív tesztelés egy része).
Használhatósági tesztek (Usability Tests): Ezek emberi interakciót, megfigyelést és szubjektív értékelést igényelnek.
Exploratív tesztelés (Exploratory Testing): Ahol a tesztelő kreativitása, tudása és intuíciója alapján "felfedezi" a szoftvert, előre nem definiált forgatókönyvek szerint.
Gyakran változó funkciók tesztjei: Ha egy funkció UI-ja vagy logikája sűrűn változik, az automatizált szkriptek folyamatos és költséges karbantartást igényelnek.
Szubjektív értékelést igénylő tesztek: Pl. vizuális megjelenés, esztétika (bár vannak eszközök vizuális regressziós tesztelésre, de a végső döntés gyakran emberi).
Nagyon bonyolult, nehezen automatizálható forgatókönyvek: Ha az automatizálás költsége és ideje aránytalanul magas a várható haszonhoz képest.
CAPTCHA és hasonló biztonsági mechanizmusok tesztelése: Ezeket direkt úgy tervezték, hogy automatizált szkriptek ne tudják kikerülni. (Tesztkörnyezetben ezeket ki szokták kapcsolni vagy mockolni.)
✅ Írj le egy jó automatizált tesztet!
Egy jó automatizált tesztnek a következő jellemzőkkel kell rendelkeznie (gyakran az FIRST mozaikszóval hivatkoznak rájuk, bár ez inkább az egységtesztekre specifikus, de általánosan is alkalmazható elveket tartalmaz):

F (Fast - Gyors): A teszteknek gyorsan le kell futniuk. A lassú tesztek rontják a visszacsatolási ciklust és csökkentik a fejlesztők hajlandóságát a futtatásukra.
I (Independent/Isolated - Független/Izolált): Minden tesztnek függetlennek kell lennie a többitől. Egy teszt eredménye nem befolyásolhatja egy másik teszt eredményét, és a tesztek bármilyen sorrendben futtathatóak kell legyenek. Nem szabad közös állapoton osztozniuk, vagy ha igen, azt minden teszt előtt/után megfelelően kell kezelni (setup/teardown).
R (Repeatable - Megismételhető): A tesztnek konzisztensen ugyanazt az eredményt kell adnia minden futtatáskor, ha a kód és a környezet nem változik. A "pelyhes" (flaky) tesztek, amelyek néha sikeresek, néha sikertelenek azonos körülmények között, aláássák a tesztkészletbe vetett bizalmat.
S (Self-Validating - Önellenőrző): A tesztnek egyértelműen meg kell tudnia állapítani, hogy sikeres volt-e vagy sem, anélkül, hogy manuális beavatkozásra vagy eredményértelmezésre lenne szükség. Tartalmaznia kell az asserciókat (assertions), amelyek ellenőrzik a várt eredményt.
T (Timely/Thorough - Időszerű/Alapos):
Időszerű: A teszteket a fejlesztéssel párhuzamosan, vagy röviddel azután kell megírni (TDD/BDD esetén még előtte).
Alapos (de nem túlzóan): Megfelelő mértékben kell lefednie a tesztelendő funkcionalitást, de nem kell minden lehetséges esetet lefednie (kimerítő tesztelés lehetetlen). Koncentráljon a fontos esetekre.
További jellemzők egy jó automatizált (UI) tesztre:

Olvasható és karbantartható: A tesztkódnak tisztának, jól strukturáltnak és könnyen érthetőnek kell lennie. Használjon beszédes változó- és függvénneveket, kommenteket, ahol szükséges. Kövessen tervezési mintákat (pl. Page Object Model).
Robusztus: Ellenálljon a kisebb UI változásoknak (pl. stabil lokátorok használata).
Determinisztikus: Adott bemenetre mindig ugyanazt a kimenetet produkálja.
Jó hibajelentés: Hiba esetén egyértelmű információt adjon arról, hogy mi és hol hibásodott meg (pl. képernyőképek, logok).
Megfelelő absztrakciós szint: A teszt a "mit" teszteljen, ne a "hogyan"-t részletezze túlságosan.
Fókuszált: Egy teszt egy konkrét dolgot vagy viselkedést ellenőrizzen.
Példa egy jó automatizált teszt leírására (koncepcionálisan):

Teszt neve: TC_LOGIN_001_Valid_Credentials_Login_Success
Előfeltételek: A felhasználó nincs bejelentkezve. A regisztrált felhasználó ("testuser", "password123") létezik a rendszerben.
Lépések:
Navigáljon a bejelentkezési oldalra.
Adja meg a "Felhasználónév" mezőbe: "testuser".
Adja meg a "Jelszó" mezőbe: "password123".
Kattintson a "Bejelentkezés" gombra.
Várt eredmény:
A felhasználó sikeresen bejelentkezik.
A felhasználó a főoldalra (dashboard) navigálódik.
A főoldalon megjelenik az "Üdvözöljük, testuser!" üzenet.
Utófeltételek (Teardown): Jelentkeztesse ki a felhasználót (ha a következő teszt ezt igényli).
Ez a teszt gyors, független (ha a felhasználói állapotot kezeli), megismételhető, önellenőrző (az asserciók a várt eredményt ellenőrzik), és időben megírható.

✅ Mi a Selenium, Selenium IDE és Selenium WebDriver?
Selenium: Egy nyílt forráskódú, hordozható szoftver tesztelési keretrendszer webalkalmazásokhoz. Lehetővé teszi a webböngészők műveleteinek automatizálását. Nem egyetlen eszköz, hanem egy szoftvercsomag, amely különböző eszközöket tartalmaz.
Fő célja: Weboldalak funkcionális tesztelésének automatizálása.
Támogatott böngészők: Chrome, Firefox, Safari, Edge, stb.
Támogatott programozási nyelvek: Java, C#, Python, Ruby, JavaScript, Kotlin.
Selenium IDE (Integrated Development Environment):
Egy böngészőbővítmény (Chrome, Firefox), amely lehetővé teszi a tesztesetek rögzítését és visszajátszását ("record and playback").
Célközönség: Kezdők, akik ismerkednek az automatizálással, vagy gyors prototípusokat szeretnének készíteni.
Funkciók: Tesztesetek rögzítése, szerkesztése, futtatása, egyszerű vezérlési szerkezetek (if, while), tesztesetek exportálása különböző programozási nyelvekre (pl. Java, Python WebDriver kódként).
Korlátok: Kevésbé alkalmas komplex tesztekhez, nehezebb a karbantartása nagyobb projektekben, korlátozottabb funkcionalitás a WebDriverhez képest (pl. nincs fejlett hibakezelés, adatvezérelt tesztelés nehézkes).
Selenium WebDriver:
A Selenium központi komponense, egy API (Application Programming Interface) és protokoll, amely lehetővé teszi a programozási nyelvek számára, hogy közvetlenül kommunikáljanak a webböngészőkkel.
Működés: Minden böngészőhöz tartozik egy specifikus "driver" (pl. ChromeDriver, GeckoDriver Firefoxhoz), amely egyfajta hídként működik a teszt szkript és a böngésző között. A WebDriver parancsokat küld a böngésző driverének, ami végrehajtja azokat a böngészőben.
Előnyök: Nagyobb rugalmasság és kontroll, támogatja a komplex tesztelési logikát, programozási nyelvek teljes ereje kihasználható (ciklusok, feltételek, kivételkezelés, OOP stb.), integrálható más tesztelési keretrendszerekkel (pl. TestNG, JUnit, PyTest) és CI/CD eszközökkel.
Használat: Ez az ipari szabvány a webes UI automatizáláshoz.
Összefoglalva:

Selenium: Az ernyőfogalom, a teljes projekt.
Selenium IDE: Egy egyszerű eszköz gyors tesztrögzítésre és lejátszásra.
Selenium WebDriver: Egy erőteljes API programozott böngésző-automatizáláshoz, a Selenium motorja.
✅ Hogyan lehet azonosítani a webes elemeket?
A Selenium WebDriver különböző lokátor stratégiákat kínál a webelemek (pl. gombok, szövegmezők, linkek) azonosítására a HTML DOM-ban (Document Object Model). A leggyakoribbak:

ID:
By.id("element_id")
Előny: Az ID-knak egyedinek kell lenniük az oldalon, ezért ez a leggyorsabb és legmegbízhatóbb lokátor. Ha van egyedi ID, ezt érdemes először választani.
Name:
By.name("element_name")
Előny: Gyakran használják űrlap elemeknél. Lehet, hogy nem egyedi.
Class Name:
By.className("element_class_name")
Előny: Hasznos, ha az elemek közös stílusosztályt használnak. Ha egy elemnek több osztálya van, csak egyet kell megadni. Ha az osztálynév szóközt tartalmaz, ez a stratégia nem fog működni (ilyenkor CSS Selector-t kell használni).
Tag Name:
By.tagName("html_tag_name") (pl. div, a, input)
Előny: Hasznos, ha egy adott típusú elemet keresünk (pl. az összes linket az oldalon). Ritkán egyedi önmagában.
Link Text:
By.linkText("teljes_link_szöveg")
Előny: Csak <a> (anchor) tagekhez használható. A link teljes, látható szövegével azonosít.
Partial Link Text:
By.partialLinkText("részleges_link_szöveg")
Előny: Szintén csak <a> tagekhez. Akkor hasznos, ha a link szövege dinamikusan változik, vagy csak egy részét ismerjük.
CSS Selector:
By.cssSelector("css_selector_kifejezés")
Előny: Nagyon erőteljes és rugalmas. Komplexebb azonosítási logikát tesz lehetővé (pl. attribútumok, hierarchia, relatív pozíciók alapján). Gyorsabb, mint az XPath a legtöbb modern böngészőben.
Példák: input[type='submit'], #username, .error-message, div > a
XPath (XML Path Language):
By.xpath("xpath_kifejezés")
Előny: A legrugalmasabb lokátor stratégia. Képes navigálni a DOM struktúrában (fel, le, testvérek), elemeket szöveges tartalmuk alapján megtalálni, és olyan elemeket is elérni, amelyeknek nincs egyedi ID-ja vagy neve.
Hátrány: Általában lassabb, mint a CSS Selector. Az XPath kifejezések törékenyebbek lehetnek, ha a DOM struktúra gyakran változik.
Példák: //input[@id='username'], //button[text()='Login'], //div[@class='container']/a[1]
Legjobb gyakorlatok lokátorok választásához:

ID: Ha van, mindig ezt használd.
Name: Jó alternatíva, ha nincs ID.
CSS Selector: Gyors, erőteljes, és jól olvasható komplexebb esetekben is.
XPath: Végső megoldásként, ha más nem működik, vagy nagyon komplex DOM navigációra van szükség (pl. szöveges tartalom alapján keresés, szülő elem elérése).
Kerüld a generált vagy nagyon általános lokátorokat (pl. //div[3]/span[2]), mert ezek könnyen eltörnek a UI változásakor.
Törekedj egyedi és stabil lokátorok használatára.
✅ Hogyan lehet várni az elemekre, és mi lehet a probléma? Gyűjtsd össze a lehetséges hibákat és okokat!
A modern webalkalmazások dinamikusan töltik be a tartalmat (pl. AJAX hívásokkal). Ezért a Selenium szkripteknek gyakran várniuk kell arra, hogy egy elem megjelenjen, kattinthatóvá váljon, vagy egy bizonyos állapotba kerüljön, mielőtt interakcióba lépnének vele. Ha a szkript megpróbál interakcióba lépni egy még nem létező vagy nem interaktív elemmel, az hibához vezet (pl. NoSuchElementException, ElementNotInteractableException).

Várakozási stratégiák a Seleniumban:

Implicit Várakozás (Implicit Wait):
driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10)); (Java példa)
Működés: Globális beállítás a WebDriver számára. Ha egy elemet nem talál azonnal, a WebDriver egy megadott ideig (pl. 10 másodperc) újra és újra megpróbálja megtalálni, mielőtt NoSuchElementException-t dobna.
Hatáskör: A WebDriver session teljes élettartamára érvényes, minden findElement és findElements hívásra hat.
Probléma:
Nem vár az elem állapotára (pl. láthatóság, kattinthatóság), csak a DOM-ban való jelenlétére.
Lelassíthatja a teszteket, ha sok elemre kell feleslegesen várni.
Elrejtheti a valódi teljesítményproblémákat.
Nem ajánlott explicit várakozással keverni, mert kiszámíthatatlan viselkedést okozhat.
Explicit Várakozás (Explicit Wait):
WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));
WebElement element = wait.until(ExpectedConditions.visibilityOfElementLocated(By.id("myElement"))); (Java példa)
Működés: Egy adott kódrészletre vonatkozik. A WebDriver egy meghatározott maximális ideig vár egy bizonyos feltétel (ExpectedCondition) teljesülésére, mielőtt TimeoutException-t dobna. Rendszeres időközönként (polling interval, alapértelmezetten 500 ms) ellenőrzi a feltételt.
Feltételek (ExpectedConditions): Sok előre definiált feltétel létezik, pl.:
visibilityOfElementLocated(By locator): Az elem jelen van a DOM-ban és látható.
elementToBeClickable(By locator): Az elem látható és engedélyezett (kattintható).
presenceOfElementLocated(By locator): Az elem jelen van a DOM-ban (nem feltétlenül látható).
invisibilityOfElementLocated(By locator): Az elem láthatatlanná válik.
textToBePresentInElementLocated(By locator, String text): A megadott szöveg megjelenik az elemben.
alertIsPresent(): Felugró ablak jelenik meg.
Előny: Sokkal rugalmasabb és pontosabb, mint az implicit várakozás. Csak ott vár, ahol szükséges, és specifikus állapotokra. Ez a javasolt várakozási mechanizmus.
Fluent Várakozás (Fluent Wait):
Wait<WebDriver> wait = new FluentWait<>(driver)
.withTimeout(Duration.ofSeconds(30))
.pollingEvery(Duration.ofSeconds(5))
.ignoring(NoSuchElementException.class);
WebElement foo = wait.until(driver -> driver.findElement(By.id("foo"))); (Java példa)
Működés: Az explicit várakozás egy fejlettebb formája, amely nagyobb konfigurációs szabadságot ad:
Beállítható a maximális várakozási idő.
Beállítható a polling intervallum (milyen sűrűn ellenőrizze a feltételt).
Megadható, hogy mely kivételeket hagyja figyelmen kívül várakozás közben (pl. NoSuchElementException).
Előny: Nagyon rugalmas, finomhangolható várakozás dinamikus elemekre.
Thread.sleep() (NEM AJÁNLOTT):
Thread.sleep(5000); // Vár 5 másodpercet (Java példa)
Működés: A végrehajtást feltétel nélkül felfüggeszti a megadott ideig.
Probléma (Miért nem ajánlott):
Nem determinisztikus: Nem veszi figyelembe, hogy az elem mikor válik elérhetővé. Ha az elem hamarabb elérhető, feleslegesen várunk. Ha később, a teszt még mindig elbukhat.
Lassú: Jelentősen megnöveli a tesztek futási idejét.
Törékeny: Ha a rendszer teljesítménye változik, a fix várakozási idők már nem lesznek elegendőek vagy túl hosszúak lesznek.
Rossz gyakorlat: Általában azt jelzi, hogy a tesztelő nem érti a dinamikus várakozási mechanizmusokat. Csak nagyon ritka, indokolt esetben (pl. debuggolás) vagy speciális szinkronizációs problémáknál szabadna használni, de akkor is csak óvatosan.
Lehetséges problémák, hibák és okok a várakozással kapcsolatban:

NoSuchElementException: Az elem nem található a DOM-ban a megadott várakozási időn belül.
Okok: Rossz lokátor, az elem még nem töltődött be, az elem egy iframe-ben van (kontextust kell váltani), az oldal még navigál.
TimeoutException: Az explicit vagy fluent várakozás során a megadott feltétel nem teljesült a maximális várakozási időn belül.
Okok: Az elem nem érte el a várt állapotot (pl. nem lett látható, kattintható), a feltétel hibás, a várakozási idő túl rövid.
ElementNotInteractableException / ElementClickInterceptedException: Az elem megtalálható a DOM-ban, de nem lehet vele interakcióba lépni (pl. kattintani, szöveget beírni).
Okok: Az elem nem látható (pl. display: none;), le van tiltva (disabled attribútum), egy másik elem elfedi (pl. felugró ablak, overlay), még nem teljesen töltődött be vagy animálódik.
StaleElementReferenceException: Az elemre való hivatkozás elavult. Ez akkor fordul elő, ha az elemet megtaláltuk, de azóta a DOM megváltozott (pl. újratöltődött az oldal, vagy az elem egy része frissült AJAX által), és az eredeti referencia már nem érvényes.
Megoldás: Az elemet újra meg kell keresni a DOM-ban, mielőtt interakcióba lépnénk vele. Gyakran segít, ha az interakciót és az elemkeresést egy try-catch blokkba tesszük, és hiba esetén újrapróbáljuk.
"Pelyhes" tesztek (Flaky Tests): A tesztek néha sikeresek, néha sikertelenek megfelelő várakozási stratégia hiánya miatt.
Túl hosszú várakozási idők: Ha az implicit vagy explicit várakozási idők túl hosszúra vannak állítva, az feleslegesen lassítja a teszteket, még akkor is, ha az elemek hamarabb elérhetővé válnak.
Implicit és explicit várakozások keverése: Ez kiszámíthatatlan várakozási időkhöz vezethet, ezért kerülendő. Általában az explicit várakozás preferált.
Megoldások és legjobb gyakorlatok:

Használj explicit várakozást (WebDriverWait, FluentWait) ExpectedConditions-szal.
Válassz megfelelő ExpectedCondition-t az adott helyzetre.
Kerüld a Thread.sleep() használatát.
Ne keverd az implicit és explicit várakozásokat. Ha explicit várakozást használsz, az implicit várakozást érdemes 0-ra állítani vagy nem használni.
Használj stabil lokátorokat.
StaleElementReferenceException esetén próbáld meg újra megtalálni az elemet.
Győződj meg róla, hogy a megfelelő frame-ben vagy ablakban keresed az elemet.
✅ Hasonlítsd össze a POM és a Keyword Driven Testing megközelítéseket!
Jellemző	Page Object Model (POM)	Keyword Driven Testing (KDT)
Alapkoncepció	Minden weboldalhoz vagy annak jelentős komponenséhez egy külön osztály (Page Object) tartozik. Ez az osztály tartalmazza az oldalon található elemek lokátorait és az azokon végezhető műveleteket (metódusokat).	A teszteseteket kulcsszavak (keywords) sorozataként definiáljuk. Minden kulcsszó egy vagy több konkrét műveletet hajt végre az alkalmazáson.
Absztrakció szintje	Magas. Elrejti a lokátorok és a Selenium WebDriver hívások részleteit a teszt szkriptek elől. A tesztek az üzleti logikára fókuszálnak.	Nagyon magas. A tesztelőknek nem kell programozniuk, csak ismerniük kell a kulcsszavakat és azok paramétereit. A kulcsszavak implementációja el van rejtve.
Tesztek írása	A teszt szkriptek a Page Object osztályok metódusait hívják meg, ami olvashatóbbá és üzleti szintűvé teszi őket. (Pl. loginPage.enterUsername("user").enterPassword("pass").clickLoginButton();)	A teszteseteket általában táblázatos formában (pl. Excel, CSV) hozzák létre, ahol minden sor egy lépést (kulcsszó + paraméterek) ír le.
Kód újrafelhasználás	Magas. Az oldalspecifikus logika (elemek, műveletek) a Page Object osztályokban van, így több teszt is felhasználhatja őket.	Magas. A kulcsszavakat (amelyek a műveleteket implementálják) többször fel lehet használni különböző tesztesetekben.
Karbantarthatóság	Jó. Ha egy UI elem lokátora vagy egy művelet logikája megváltozik az oldalon, csak a megfelelő Page Object osztályban kell módosítani, a teszt szkriptek érintetlenül maradhatnak.	Jó. Ha egy művelet implementációja változik, csak a kulcsszóhoz tartozó kódot kell frissíteni. Ha új funkcionalitás kerül be, új kulcsszavakat kell létrehozni.
Technikai tudásigény	A Page Object osztályok létrehozásához és karbantartásához programozási ismeretek (pl. Java, Python) és Selenium tudás szükséges. A tesztesetek írásához kevesebb technikai tudás is elég lehet, ha a POM jól van felépítve.	A kulcsszavak implementálásához programozási és automatizálási eszköz (pl. Selenium) ismerete szükséges. A tesztesetek (kulcsszavak használatával történő) összeállításához minimális technikai tudás is elegendő.
Eszközök	Nincs specifikus eszközigénye, a Seleniummal és egy programozási nyelvvel valósítható meg. Tervezési minta.	Gyakran speciális keretrendszerek vagy eszközök támogatják (pl. Robot Framework, QTP/UFT keyword view, egyedi fejlesztésű keretrendszerek).
Előnyök	Olvashatóbb, karbantarthatóbb tesztek. Kódduplikáció csökkentése. Jobb tesztstruktúra.	Lehetővé teszi a nem programozó tesztelők számára is az automatizált tesztek készítését. Magas szintű újrafelhasználhatóság. Könnyen érthető tesztlépések.
Hátrányok	Kezdetben több időt vehet igénybe a Page Object osztályok felépítése.	A keretrendszer felépítése és a kulcsszavak implementálása kezdetben bonyolult és időigényes lehet. Kevésbé rugalmas, mint a tisztán kód alapú megközelítés bizonyos komplex esetekben.
Mikor hasznos?	Közepes és nagyméretű projekteknél, ahol a UI várhatóan változik, és fontos a karbantarthatóság. Gyakori a Seleniummal együtt.	Nagyobb projekteknél, ahol vegyes technikai tudású csapat dolgozik, és a tesztelési logika jól lebontható diszkrét műveletekre.

Exportálás Táblázatok-fájlba
Összefoglalva:

A POM egy tervezési minta, amely a weboldalak struktúráját képezi le osztályokba, hogy a tesztkód tisztább és karbantarthatóbb legyen. A tesztek még mindig kódban íródnak, de magasabb absztrakciós szinten.
A Keyword Driven Testing egy teszttervezési és automatizálási megközelítés, ahol a tesztesetek kulcsszavakból állnak, és ezeket a kulcsszavakat egy mögöttes kód implementálja. Ez lehetővé teszi, hogy a teszteket akár programozási ismeretek nélkül is össze lehessen állítani.
A két megközelítés nem zárja ki egymást; egy KDT keretrendszer használhat POM-ot a kulcsszavak implementációjának részeként a UI interakciókhoz.

✅ Mi a különbség a TDD és BDD között?
Jellemző	Test-Driven Development (TDD)	Behavior-Driven Development (BDD)
Fókusz	A szoftverkomponensek (egységek, modulok) helyes működésére, belső minőségére. "Hogyan építsük meg helyesen?"	A szoftver elvárt viselkedésére összpontosít, a felhasználó vagy üzleti érdekelt szemszögéből. "A helyes dolgot építjük?"
Ciklus	1. Írj egy (sikertelen) tesztet. 2. Írj annyi kódot, hogy a teszt sikeres legyen. 3. Refaktorálj. (Red-Green-Refactor)	1. Írj egy viselkedési specifikációt (feature fájlt). 2. Implementáld a lépésdefiníciókat (ezek lehetnek sikertelen tesztek). 3. Írj annyi kódot, hogy a specifikáció teljesüljön. 4. Refaktorálj.
Ki írja a teszteket?	Főként fejlesztők.	Együttműködve: üzleti elemzők, terméktulajdonosok, tesztelők és fejlesztők (a "Három Amigó").
Nyelvezet	Programozási nyelvhez kötött tesztelési keretrendszerek (pl. JUnit, NUnit, PyTest). A tesztek kódban íródnak.	Természetes nyelven (vagy ahhoz közeli, strukturált formában, pl. Gherkin - Given/When/Then) írt viselkedési specifikációk. Ezeket fordítják le futtatható tesztekké.
Célközönség a tesztekhez	Fejlesztők.	Az egész csapat, beleértve a nem technikai szereplőket is. A specifikációk "élő dokumentációként" is szolgálnak.
Tesztelési szint	Elsősorban egységtesztelés (unit testing), de alkalmazható integrációs tesztelésre is.	Elsősorban elfogadási tesztelés (acceptance testing) és rendszertesztelés, de használható magasabb szintű integrációs tesztekhez is.
Eszközök (példák)	JUnit (Java), NUnit (.NET), PyTest (Python), RSpec (Ruby).	Cucumber (Java, Ruby, JS, stb.), SpecFlow (.NET), Behave (Python), JBehave (Java).
Granularitás	Finomabb szemcsézettségű, egy-egy függvényre vagy metódusra fókuszál.	Durvább szemcsézettségű, egy-egy felhasználói funkcióra vagy üzleti szabályra fókuszál.
Cél	Kódminőség javítása, hibák korai felderítése, karbantartható kód létrehozása, fejlesztői magabiztosság növelése.	Közös megértés kialakítása a követelményekről, a szoftver üzleti értékének biztosítása, kommunikáció javítása a csapaton belül.

Exportálás Táblázatok-fájlba
Kapcsolat:
BDD tekinthető a TDD egy továbbfejlesztésének vagy kiterjesztésének. A BDD a TDD "Red-Green-Refactor" ciklusát használja, de a teszteket üzleti viselkedés köré szervezi, és hangsúlyozza az együttműködést és a közös nyelvet. BDD alatt gyakran TDD-t alkalmaznak az egyes lépésdefiníciók implementálásakor.

Röviden:

TDD: Fejlesztői gyakorlat, amely a kód egységeinek helyes implementációjára fókuszál tesztek vezérlésével.
BDD: Együttműködési folyamat, amely a szoftver elvárt viselkedésére fókuszál, természetes nyelven írt specifikációkon keresztül, elősegítve a közös megértést.
✅ Mi az API tesztelés és miért hasznos?
API tesztelés (Application Programming Interface Testing):
Olyan szoftvertesztelési típus, amely közvetlenül az API-kat teszteli, és része az integrációs tesztelésnek, hogy ellenőrizze az API-k funkcionalitását, megbízhatóságát, teljesítményét és biztonságát. Az API tesztelés a szoftverarchitektúra üzleti logikájának rétegére összpontosít, anélkül, hogy a felhasználói felületet (UI) érintené. A tesztek során a szoftver requesteket (kéréseket) küld az API végpontoknak, majd validálja a response-okat (válaszokat) a funkcionalitás, adatok, státuszkódok és teljesítmény alapján.

Miért hasznos az API tesztelés?

Korai hibafelismerés: Mivel az API-k az alkalmazás logikájának magját képezik, az itt talált hibák korábban és olcsóbban javíthatók, mintha csak a UI tesztelés során derülnének ki.
Gyorsabb tesztfuttatás: Az API tesztek általában sokkal gyorsabbak, mint a UI tesztek, mivel nem kell megvárni a UI elemek betöltődését és renderelését. Ez gyorsabb visszajelzést tesz lehetővé a fejlesztőknek.
Nagyobb stabilitás: Az API-k interfészei általában stabilabbak, mint a felhasználói felületek, amelyek gyakrabban változhatnak. Ezért az API tesztek kevésbé törékenyek és kevesebb karbantartást igényelnek.
Nyelv- és platformfüggetlenség: Az API-k általában szabványos protokollokat (pl. HTTP/HTTPS) és adatcsere formátumokat (pl. JSON, XML) használnak, így bármilyen nyelvvel vagy platformmal tesztelhetők, amely képes ezeket kezelni.
Költséghatékonyság: A gyorsabb futás, a kevesebb karbantartás és a korai hibafelismerés miatt az API tesztelés hosszú távon költséghatékonyabb lehet, mint kizárólag a UI tesztekre támaszkodni.
Jobb tesztfedettség: Lehetővé teszi az üzleti logika olyan részeinek tesztelését is, amelyek a UI-n keresztül nehezen vagy egyáltalán nem érhetők el.
Biztonsági tesztelés: Az API végpontok tesztelhetők sebezhetőségekre, mint például authentikációs és autorizációs problémák, adatkezelési hibák stb.
Integrációs tesztelés alapja: Az API-k összekötik a különböző szoftverkomponenseket és -rendszereket. Az API tesztelés kulcsfontosságú annak ellenőrzésében, hogy ezek az integrációk megfelelően működnek-e.
Automatizálás CI/CD folyamatokban: Gyorsaságuk és megbízhatóságuk miatt az API tesztek könnyen integrálhatók a folyamatos integrációs és folyamatos szállítási (CI/CD) pipeline-okba, így biztosítva a szoftver minőségét minden buildnél.
Terheléses tesztelés: Az API-k teljesítménye és skálázhatósága tesztelhető anélkül, hogy a UI réteg szűk keresztmetszetet képezne.
✅ Mi az adatvezérelt tesztelés és miért hasznos?
Adatvezérelt tesztelés (Data-Driven Testing - DDT):
Egy szoftvertesztelési módszertan, amelyben a tesztadatokat külső forrásból (pl. CSV fájl, Excel táblázat, adatbázis, JSON/XML fájl) olvassuk be, és ugyanazt a tesztlogikát (teszt szkriptet) hajtjuk végre többször, különböző bemeneti adatkészletekkel. A teszt szkript és a tesztadatok elkülönülnek egymástól.

Hogyan működik:

A tesztlogikát (a végrehajtandó lépéseket) egyetlen teszt szkriptben vagy függvényben definiáljuk.
A tesztadatokat (bemeneti értékek és várt kimenetek) egy külső adatforrásban tároljuk. Minden sor ebben az adatforrásban általában egy teszt iterációnak felel meg.
A tesztelési keretrendszer vagy szkript beolvassa az adatokat az adatforrásból.
A teszt szkript ciklikusan lefut, minden iterációban az adatforrás következő adatkészletét használva.
Minden egyes iteráció eredményét külön rögzítik.
Miért hasznos az adatvezérelt tesztelés?

Kód újrafelhasználás: Ugyanazt a teszt szkriptet használhatjuk számos különböző adatértékkel, csökkentve a redundáns tesztkód mennyiségét.
Jobb tesztfedettség: Könnyen tesztelhetünk sokféle bemeneti kombinációt és szélső esetet anélkül, hogy minden egyes esethez külön teszt szkriptet kellene írni. Ez növeli a tesztelt forgatókönyvek számát.
Könebb karbantartás:
Ha a tesztlogika változik, csak egy helyen (a központi teszt szkriptben) kell módosítani.
Ha a tesztadatok változnak, vagy új teszteseteket (adatkészleteket) kell hozzáadni, azt a külső adatforrásban tehetjük meg a tesztkód érintése nélkül.
Átláthatóság és érthetőség: A tesztadatok elkülönítése a kódtól átláthatóbbá teszi, hogy milyen adatokkal történik a tesztelés. Nem technikai szakemberek (pl. üzleti elemzők) is könnyebben áttekinthetik vagy akár szerkeszthetik a tesztadatokat.
Skálázhatóság: Könnyen bővíthető új tesztesetekkel egyszerűen új adatsorok hozzáadásával a külső fájlhoz.
Kevesebb tesztkód: Jelentősen csökkenti a megírandó tesztkód mennyiségét, mivel egyetlen szkript több forgatókönyvet is lefedhet.
Hatékonyság: Gyorsabbá teszi a tesztesetek létrehozását és futtatását, különösen, ha sok hasonló tesztesetet kell végrehajtani különböző adatokkal.
Hibák jobb izolálása: Ha egy teszt egy adott adatkészlettel hibát jelez, könnyebb azonosítani, hogy melyik bemeneti kombináció okozta a problémát.
Példa: Egy bejelentkezési funkció tesztelése adatvezérelt módon:

Teszt szkript (logika):
Nyisd meg a bejelentkezési oldalt.
Írd be a felhasználónevet a felhasználónév mezőbe.
Írd be a jelszót a jelszó mezőbe.
Kattints a bejelentkezés gombra.
Ellenőrizd a várt eredményt (pl. sikeres bejelentkezés üzenet, hibaüzenet).
Adatforrás (pl. CSV fájl):
Kódrészlet

Felhasznalonev,Jelszo,VartEredmenyLeiras
validUser,validPass,SikeresBejelentkezes
invalidUser,validPass,HibauzenetMegjelenik
validUser,invalidPass,HibauzenetMegjelenik
,validPass,HibauzenetMegjelenik
validUser,,HibauzenetMegjelenik
A teszt szkript minden sorra lefut a CSV fájlból, felhasználva az adott sorban lévő adatokat.