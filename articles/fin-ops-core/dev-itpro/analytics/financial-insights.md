---
title: Financial Insights
description: A Financial Insights a Microsoft Power BI szolgáltatást használja kulcsfontosságú pénzügyi mutatók (KPI), diagramok és pénzügyi kimutatások összefogására.
author: kweekley
manager: AnnBe
ms.date: 05/22/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 106233
ms.assetid: 517e6a88-e7a1-4398-9971-b22fa83306ba
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: 7.2999999999999998
ms.openlocfilehash: 596a067611ac4477f4469dbbc370c971e0f7a35d
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2181772"
---
# <a name="financial-insights"></a>Financial Insights

[!include [banner](../includes/banner.md)]

A **Financial Insights** a Microsoft Power BI szolgáltatást használja kulcsfontosságú pénzügyi mutatók (KPI), diagramok és pénzügyi kimutatások összefogására. A Power BI be van ágyazva az alkalmazásba. A **Financial Insights** lényege az analitikus jelentéskészítés. A szervezeten belüli személyek megtekinthetnek, kutatást végezhetnek, ismereteket szerezhetnek és műveleteket hajthatnak végre. 

A **Financial Insights** kombinálja az adatokat a főkönyvből és az analitikus naplókból, hogy teljesebb képet adjon a szervezet pénzügyi helyzetéről.

> [!NOTE]
> Ez a dokumentum az alábbi Power BI terminológiát használja:
> 
> - **Jelentés** – Egyetlen .pbix fájl, amelybe az összes fül összes vizuális eleme elmentésre kerül.
> - **Oldal** – Egyetlen .pbix fájl egy füle. Minden egyes oldal egy vagy több vizuális elemet tartalmazhat.
> - **Vizuális elem** – Egyetlen adatforrás, például karton, KPI, diagram, grafikon, mátrix vagy pénzügyi kimutatás. Az olyan oldal, amelyen pénzügyi kimutatás szerepel vizuális elemként, nem tartalmazhat más vizuális elemeket a jelentésben szereplő adatok mérete miatt.

Jelenleg a **Financial Insights** az aktív jogi személy vagy az összes jogi személy adatainak megtekintésére szolgál. A jövőbeli kiadásokban a munkaterület úgy fog fejlődni, hogy a Power BI segítségével módosíthat és létrehozhat majd vizuális elemeket.

A **Pénzügyi igazgató-áttekintés** munkaterület ugyanazokat a vizuális elemeket jeleníti meg, mint a **Financial Insights**, de középpontjában a meglévő jelentések adatainak megtekintése és szűrése áll. A jövőbeni kiadásokban új vizuális elemeket adhat hozzá a **Financial Insights** munkaterülethez. Az új vizuális elemek olyan munkaterületeken is elérhetők lehetnek, amelyek más szerepkörökre koncentrálnak, például a projektmenedzserekre vagy a kötelezettségek kezelőire. A **Pénzügyi igazgató áttekintés** a munkaterület továbbra is minden jogi személynél megjeleníti az adatokat, függetlenül azoktól a jogi személyektől, amelyekhez a szerepkör hozzáfér.

## <a name="dynamics-365-finance-setup"></a>Dynamics 365 Finance beállítása
**Főkönyv**

A megfelelő alapértelmezés szerinti fő számlák kitöltésére a **Mérleg** pénzügyi kimutatásban és a **Financial Insights** alkalmazáson belüli különböző **Eredménykimutatás** pénzügyi kimutatásokban a fő számla típusa és a főszámla-kategóriák használatosak.

A **Fő számlák** lapon meg kell adnia a fő számlát, hogy hozzárendelje az alábbi típusok egyikét:

- Bevétel
- Expense
- Eszközök
- Kötelezettségek
- Saját tőke

Ne rendeljen semmilyen más főszámla-típust (például **Mérleg** vagy **Eredmény**) a fő számlákhoz. A jelentéstétel nem tudja meghatározni a fő fiók típusát, ha más főfiók-típusok vannak hozzárendelve, mivel ezek nem eléggé részletesek. A fő számla típusát úgy kell meghatározni, hogy a források és a bevétel pozitív összegekként jelenjenek meg a pénzügyi kimutatásokban.

A pénzügyi kimutatásokban való megjelenítéshez és a különféle egyéb vizuális elemekbe - például a KPI-kba - való befoglaláshoz minden fő számlához főszámla-kategóriát kell rendelni. A Főszámla-kategóriákat továbbfejlesztettük, hogy megjelenítési sorrendet tartalmazzanak. A megjelenítési sorrend kifejezetten használatos a **Financial Insights** pénzügyi kimutatásaiban. Új főszámla-kategória hozzáadása vagy szerkesztése után módosítható a **Megjelenítési sorrend** értéke, és ezzel megadható a sorrend, amelyben a főszámla-kategóriák megjelennek a pénzügyi kimutatásokban. Ha számos főszámla-kategória megjelenítési sorrendjét módosítania kell, használhatja a Megnyitás az Excel programban funkciót a módosítások gyors szerkesztéséhez és az alkalmazásban való közzétételéhez.

## <a name="entity-store"></a>Entitástár
A **Financial Insights** adatainak lekérése az Entitástárból történik (**Rendszerfelügyelet** \> **Beállítás** \> **Entitástár**). Ha megnyitja a **Pénzügyi igazgató áttekintés** vagy **Financial Insights** munkaterület, és a következő figyelmeztető üzenet jelenik meg a vizuális elemekben, frissítenie kell az entitásokat.

![Figyelmeztetés](./media/Cantdisplay.png)

Frissítenie kell a következő entitásokat az adatok a **Financial Insights** és **Pénzügyi igazgató áttekintés** munkaterületeken való megtekintéséhez:

- Pénzügyi jelentéskészítés tranzakcióadatok 2-es verzió (**Megjegyzés:** Ez új a 10.0.1-es verzióban, és az előző entitás helyébe lép.)
- Pénzügyi jelentéskészítés tranzakciós adatai
- CustCollectionsBIMeasurements
- LedgerCovLiquidityMeasurement
- Beszerzés kocka
- Értékesítés kocka

Az előző verzióban a LedgerActivityMeasure és VendPaymentBIMeasure entitás a **Pénzügyi igazgató-áttekintés** munkaterület adataihoz voltak használva. A jelenlegi verzióban azonban már nem használatosak.

Meghatározhat egy ismétlődő köteget, hogy rendszeresen frissítse az entitások adatait. Mivel minden egyes entitás teljes mértékben újraépül a frissítések során, óvatosan válassza ki az entitásfrissítések idejét és gyakoriságát. A pénzügyi kimutatásoknál használt elsődleges entitás a FinancialReportingTransactionData entitás. Ezért dönthet úgy, hogy gyakrabban frissíti ezt az entitást.

## <a name="security"></a>Biztonság
Jelenleg a beágyazott Power BI jelentések adatait nem lehet azon jogi személyekre korlátozni, amelyekhez a felhasználó hozzáfér. Ezért a beágyazott Power BI jelentések felügyelete a biztonsági beállítások feladatköreivel történik. A meghatározott feladatkörök valamennyi jogi személy vagy csak az aktív vállalat adataihoz engedélyezik a hozzáférést. Az alábbi táblázat bemutatja a létező feladatköröket és a szerepköröket, amelyekhez ezek hozzá vannak rendelve. A feladatkörök eltávolíthatók vagy más szerepkörökhöz rendelhetők a szervezet igényei alapján.

| Feladatkör                                    | Szerepkörök | Leírás |
|-----------------------------------------|-------|------------|
| Pénzügyi igazgatói áttekintés munkaterület megjelenítése             | Pénzügyi igazgató | Ez a feladatkör a Pénzügyi igazgató áttekintés munkaterülethez biztosít hozzáférést. Alapértelmezés szerint az aktív vállalat szolgál szűrőként. Viszont minden jogi személyt hozzáadhat függetlenül attól, hogy a felhasználó hozzáfér-e a többi jogi személyhez. |
| Jelenlegi vállalat pénzügyi információinak megtekintése | <ul><li>Könyvelő</li><li>Főkönyvelő</li><li>Számviteli felügyelő</li><li>Könyvvizsgáló</li><li>Költségvetés-kezelő</li><li>Vezérigazgató</li><li>Pénzügyi igazgató</li><li>Pénzügyi ellenőr</li></ul> | Ez a feladatkör hozzáférést biztosít a Financial Insights alkalmazáshoz. Alapértelmezés szerint az aktív vállalat szolgál szűrőként. Nem adhat hozzá más jogi személyeket. |
| Vállalatközi pénzügyi információk megtekintése   | A Microsoft Dynamics 365 for Finance and Operations, Enterprise edition 7.3-as verziójában ez a kötelességhez nem rendelt szerepkört. A következő kiadásban ez a feladatkör a pénzügyi igazgatói szerepkörhöz kerül hozzárendelésre. | Ez a feladatkör a Pénzügyi igazgató áttekintés munkaterület menüpontjához biztosít hozzáférést. Alapértelmezés szerint az aktív vállalat szolgál szűrőként. Viszont minden jogi személyt hozzáadhat függetlenül attól, hogy a felhasználó hozzáfér-e a többi jogi személyhez. |


## <a name="financial-reporting-vs-finanical-insights"></a>Pénzügyi jelentések és Pénzügyi statisztikák
Noha a **Pénzügyi statisztikák** tartalmaznak pénzügyi kimutatásokat, nem helyettesítik az alkalmazás funkcióját. A **Pénzügyi statisztikák** alapértelmezett pénzügyi kimutatásai korlátozottak, és nem tartalmazzák a pénzügyi kimutatások valamennyi típusát. Pénzügyi jelentéskészítő modul továbbra is elsődleges eszköz a jogszabályban meghatározott pénzügyi kimutatások megtervezéséhez, létrehozásához és előállításához.

A következő összehasonlító táblázattal különbséget tehet a két lehetőség között:


|                                                          | Pénzügyi jelentéskészítés                                               | Financial Insights |
|----------------------------------------------------------|-------------------------------------------------------------------|--------------------|
| **Alapértelmezett jelentések szerkesztése**                                 | Igen                                                               | Nincs |
| **Új jelentések készítése**                                   | Igen                                                               | Nincs |
| **Jelentések nyomtatása**                                        | Igen                                                               | Nincs |
| **Exportálás az Excel programba**                                      | Igen                                                               | A korlátozott nyers adatokat exportál az Excel programba, nem formázott jelentést |
| **Jelentéskészítési hierarchia / szervezeti hierarchia támogatása**   | Igen                                                               | Nincs |
| **Jelentés analitikus adatokról**                             | Igen a Korlátozott csak szállítóra, vevőre                              | Igen: szállító, vevő, vevői és szállítói csoportok, vevői és szállítói címek stb. |
| **Jelentési pénznem**                                   | Igen: könyvelési pénznem és a fordítás jelentési pénznemre       | Nem: Csak a könyvelési pénznem |
| **Biztonság**                                             | Igen, a Finance és a jelentési fa biztonsága alapján | Korlátozott: jelentések megtekintése minden vállalatnál (Finance and Operations biztonságtól függetlenül) vagy csak az aktív vállalatnál |
| **Támogatás különböző számlatükrökhöz és pénzügyi évekhez** | Igen                                                               | Nincs |
| **jelentés külső adatokról**                              | Nincs                                                                | Nincs |
| **Konszolidációk támogatása**                               | Igen                                                               | Korlátozott: jelentés több vállalatról is, de csak a könyvelési pénznem használatával |

Az eredeti **Pénzügyi igazgató áttekintés** munkaterületből származó felhasználói felületen kívül új KPI-k, diagramok és pénzügyi kimutatások is elérhetők. A következő pénzügyi kimutatások állnak rendelkezésre:

- Főkönyvi kivonat
- Mérleg
- Eredménykimutatás régiónként
- Eredménykimutatás – Tényleges és tervezett
- Eltéréseket tartalmazó eredménykimutatás
- 12 hónapos trend eredménykimutatás
- Költségek három éves trendje
- Szállítónkénti költségek
- Értékesítés vevőnként

## <a name="edit-visuals"></a>Vizuális elemek szerkesztése
A **Financial Insights** kezdeti kiadásában egyetlen vizuális elem sem szerkeszthető. A jövőbeli kiadásokban a megfelelő biztonsággal rendelkező felhasználók képesek lesznek új vizuális elemeket készíteni, meglévő vizuális elemeket másolni és szerkeszteni. Bár a jelentéseket tartalmazó .pbix fájlok erőforrásokként érhetők el, nem javasoljuk az alapértelmezett jelentések szerkesztését. További módosításokra kerül sor az adatmodellen, az alapértelmezett jelentéseken és a pénzügyi kimutatások létrehozásához használt egyéni pénzügyi kimutatás vizuális elemen. Ezért, hogy kihasználhassa az új funkciók és az adatmodell a következő kiadásban megjelenő módosításait, újra meg kell ismételnie az alapértelmezett jelentéseken a Microsoft Power BI Desktop segítségével elvégzett módosításokat.

## <a name="filtering"></a>Szűrés
A felhasználók a bal oldali **Szűrés** ablaktáblával szűrhetik a jelentést. Ez az ablaktábla ugyanaz, mint ami a Power BI Desktop segítségével érhető el. A szűrésnek különböző szintjei vannak, amelyek közül egyesek esetleg nem állnak rendelkezésre attól függően, hogy mit választott ki az oldalon (lapon), illetve hogy használja-e a részletezési funkciókat:

- **Jelentésszintű szűrők** – Ezek a szűrők az összes oldalon (lapon) található összes vizuális elemre vonatkoznak.
- **Oldalszintű szűrők** – Ezek a szűrők az aktív lapon lévő összes vizuális elemre vonatkoznak. Ezeket a szűrőket a jelentésszintű szűrőkön túlmenően alkalmazza a rendszer.
- **Vizuális elemszintű szűrők** – Ezek a szűrők csak a kiválasztott vizuális elemre vonatkoznak. Ezeket a szűrőket az oldalszintű szűrökön túlmenően alkalmazza a rendszer.
- **Részletező szűrő** – Ez a szűrő olyan „forrás” vizuális elemből szűr, amelyet a jelenlegi vizuális elemre alkalmazott, amikor a forrás vizuális elemről a jelenlegi vizuális elemre részletezett.

![Szűrő](./media/filter.png)

Egy adott szűrőérték eltávolításához válassza a mellette látható radírszimbólumot. Ne az X kiválasztásával távolítsa el a szűrőt. Ha kiválasztja az X-et, akkor a szűrt mező törlődik a szűrőlehetőségek közül. Ha véletlenül eltávolít egy mezőt a szűrőből, zárja be a munkaterületet, majd nyissa meg újra. Az alapértelmezett szűrőbeállítások újra alkalmazásra kerülnek.

Alapértelmezés szerint amikor először megnyitja a munkaterületeket, az aktív jogi személy használatos jelentésszintű szűrőként. Biztonságuk függvényében a felhasználók esetleg más jogi személyeket is felvehetnek, vagy megváltoztathatják a szűrőben kiválasztott alapértelmezett jogi személyt.

A **Pénzügyi naptár** szűrőt kell használni, hogy a megfelelő naptár kerüljön felhasználásra a vizuális elemhez. A jelentésszintű szűrő alapértelmezés szerint az aktív jogi személy pénzügyi naptárára van állítva. Ha a szűrőt olyan pénzügyi naptárra állítja át, amelynek más a kezdő vagy befejező dátuma, a kezdeti egyenlegek nem kerülnek be. Emiatt a **Mérleg** pénzügyi kimutatások nem a helyes egyenlegeket fogják megjeleníteni. Ha új pénzügyi naptárt választ ki a szűrőben, oszlopok további csoportja áll rendelkezésre. Az oszlopok minden további csoportja egy másik pénzügyi naptár összegeit mutatja.

A **Feladási réteg** szűrő is szükséges. Alapértelmezés szerint a szűrő beállítása az Aktuális. További feladási rétegeket választhat ki a szűrőben az összesített összegek megjelenítéséhez.

Szűrők érhetők el a **Dátum** és **Pénzügyi év** mezőkhöz is. Általában ezeket a szűrőket az oldal szintjén alkalmazzuk. Alapértelmezés szerint a **Dátum** szűrő egy módosítható relációs dátumot használ. A relációs dátum szűrő el is távolítható, és helyettesíthető a **Pénzügyi év** szűrővel.

## <a name="currency"></a>Pénznem

Az általános főkönyvi adatokra vonatkozó összes vizuális elem a könyvelési pénznemben mutatja az összegeket. Ezért ha a jogi személyre szűr, ügyeljen arra, hogy csak azon jogi személyeket vegye fel, amelyeknél a könyvelési pénznem ugyanaz. Ellenkező esetben az összegző adatok különböző pénznemekben fognak szerepelni.

Az analitikus adatokra vonatkozó vizuális elemek, például **Pénzforgalmi előrejelzés** és **A legjobb 10** vizuális elem a rendszer pénznemében mutatja az összegeket. A rendszer pénzneme és a rendszer árfolyamtípusa a **Rendszerparaméterek** oldalon határozhatók meg.

A **Bankszámla egyenlege** vizuális elem a bankszámlák pénznemében használja az összegeket.

## <a name="dimensions"></a>Dimenziók

Az alapértelmezett pénzügyi kimutatások nem tartalmaznak pénzügyi dimenziót, hanem csak a fő számlára összpontosítanak. A pénzügyi dimenziók támogatása elérhető lesz a jövőbeli kiadásokban, amikor a jelentések szerkeszthetővé válnak. A szervezetek ezután képesek lesznek pénzügyi dimenzióértékekre szűrni.

Egyes pénzügyi kimutatások analitikus tranzakciókon alapuló dimenziókat tartalmaznak. Az új pénzügyi kimutatások célja, hogy lehetővé tegyék a pénzügyi dimenzióként be nem állított dimenziók szűrését. Például az alapértelmezett Szállítónkénti költségek jelentésben a fő számlán túl is bővíthet, és így az egyenlegeket szállító szerinti bontásban is láthatja. A szállító nincs beállítva pénzügyi dimenziónak. Ehelyett a rendszer visszanyúl a kiindulási analitikus tranzakcióhoz a szállító megtalálásához.

A következő dimenziók használatosak az alapértelmezett jelentésekben. E dimenziók egyike sem pénzügyi dimenzió.

- Szállító
- Szállítói csoport
- Vevő
- Vevőcsoport
- Ország/régió
- Állam/tartomány
- Város

> [!IMPORTANT] 
> Ha több szállító vagy vevő tranzakcióit összesíti egy bizonylaton a pénzügyi naplók használatával, az adatok helytelenek lesznek. A jelentések nem tudják meghatározni, hogy melyik szállító vagy vevő kapcsolódik egy adott főkönyvi számlához egy naplóbejegyzésben, mert ezeket az adatokat nem vezetik sehol. Emiatt nem ajánlott több szállítót, vevőt, tárgyi eszközt vagy projektet feltüntetni egy bizonylaton.

## <a name="drill-on-data"></a>Leásás adatokhoz

Különböző leásási szintek érhetők el a Power BI segítségével. Minden szintnek eltérő neve és különböző funkciói vannak. Sorokra és oszlopokra is le lehet ásni. Ez a szakasz a **Főkönyvi kivonat** pénzügyi kimutatást példaként használva mutatja be a különféle lehetőségeket, és megmutatja, hogyan lehet leásni a sorokban. Ugyanez a funkció létezik az oszlopokhoz is. Csak módosítania kell a **Leásás célja** beállítást.

Az alábbi példában a **Főkönyvi kivonat** kimutatás összecsukódik a sorhierarchia legmagasabb szintjére, amely a fő számla típusa.

![Főkönyvi kivonat](./media/trial-balance.png)

Ha a hierarchia következő szintjét, a főszámla-kategóriákat szeretné megtekinteni, állítsa a **Leásás célja** mezőt **Sorok** értékre, és válassza a **Kibontás** gombot (a harmadik gomb a Leásás célja mező után). Most kibontva látja az összes főszámla-kategóriát. Jelenleg a Power BI nem teszi lehetővé, hogy csak egy sort vagy oszlopot bontson ki, de mégis lássa az összes többi sort vagy oszlopot.

![Főkönyvi kivonat](./media/trial-balance2.png)

A fő számlák az összes sorra vonatkozó kibontásához újra használhatja a **Kibontás** gombot. Azonban, ha csak egy sornál szeretne leásni a fő számlákig, először válassza a **Leásás** gombot (az ablak jobb oldalán levő egyetlen lefelé mutató nyíl), majd válassza ki a sort, amelynél le szeretne ásni. Az alábbi ábrán az az eredmény látható, ha az **Értékesítés** sor van kiválasztva a **Leásás** gomb kiválasztása után.

![Főkönyvi kivonat](./media/trial-balance3.png)

Miután egy sornál leásott, több kattintás szükséges ahhoz, hogy visszatérjen a teljes főkönyvi kivonathoz. A **Felásás** gomb (az első gomb a **Leásás** mező után) csak az **Értékesítés** kategória környezetében ás felfelé, a következő ábrán látható módon.

![Főkönyvi kivonat](./media/trial-balance4.png)

Folytathatja a **Felásás** gomb használatát a sorok legmagasabb szintű összegzéséig.

A Power BI egy olyan gombbal is rendelkezik, amely lehetővé teszi, hogy a hierarchiában a következő szintre lépjen (a második gomb a **Leásás célja** mező után). Ennek a gombnak a hatása különbözik a **Kibontás** gombétól (a harmadik gomb a **Leásás célja** mező után), amely a hierarchia kibontására használatos. A hierarchiát kibontva a jelentésben megmarad a hierarchia. Például, amint korábban bemutattuk, ha a fő számla típusára kibontva továbbra is megjelenik a fő számla típusa a jelentésben. Azonban a hierarchiában a következő szintre lépve a jelentés többé nem jeleníti meg a szülőt a hierarchiában, ahogyan az a következő ábrán látható.

![Főkönyvi kivonat](./media/trial-balance5.png)

Az összegzett egyenlegek mögötti tranzakció részleteinek megtekintéséhez kiválaszthat bizonyos összegeket a Financial and Operations alkalmazásba való visszaásáshoz.

A pénzügyi kimutatásokból való visszaásással a Könyvelési források böngészőjébe (ASE), kerül, nem pedig a bizonylati ügyletekhez. Az ASE nem csak a főkönyvben meglévő könyvelési tételeket mutatja meg. Ehelyett az analitikus tranzakció részletes adatait mutatja. Ezért sokkal több részletet kap a kiinduló tranzakcióról, és elemzésre is felhasználhatja. Például láthatja, hogy ki volt a szállító vagy a vevő, mit vásárolt a vevő vagy mit adott el az eladó, és még azt is, hogy milyen a projekt szerepelt a tranzakcióban.

A pénzügyi kimutatásokból a következő szűrők elküldésre kerülnek az ASE-nek, hogy az ASE megjeleníthesse az összesített tranzakciókat:

Kötelezően kitöltendő mezők szűréshez:

- Jogi személy
- Pénzügyi naptár
- Év
- Fő számla azonosítója

Opcionálisan kitöltendő mezők szűréshez:

- Negyedév
- Hónap
- Időszak

Ha egy sorban nem bont ki elegendő mélységig, a leásás nem működik. Például ha csak a főszámla-kategóriáig bővít, akkor nem lehet leásni az ASE-ig az egyenleg után, mivel a fő számla mezőt kötelező kitölteni az ASE-ben végzett szűréshez.

Ha túlságosan mélyre bővít egy sorban, a pénzügyi kimutatásokra vonatkozó további szűrőket a rendszer nem küldi el az ASE-nek. Emiatt eltérő számok jelenhetnek meg. Például ha az országig vagy régióig bővít lefelé a régiónkénti eredménykimutatás pénzügyi kimutatás sorain, az ország vagy régió nem kerül be szűrőként az ASE-be.

> [!NOTE]
> A pénzügyi kimutatási sorokban és oszlopokban mélyebbre le lehet ásni, mint ameddig az ASE jelenleg a szűrést támogatja. Ezért bizonyos esetekben a ASE-ben megjelenő részletes tranzakciók összege más lesz, mint az az egyenleg, ameddig leásott. Ezt a funkciót a jövőben továbbfejlesztjük.

## <a name="hierarchies"></a>Hierarchiák

Az alapértelmezett pénzügyi kimutatások két hierarchiát használnak az az adatok kibontásához és a bennük való leásáshoz. Az egyik hierarchia a sorokra vonatkozik, a másik pedig az oszlopokra. Mindkét hierarchia előre meg van határozva a pénzügyi kimutatás tervezése során. A legtöbb pénzügyi kimutatásnál a sor hierarchiája a következő **Fő számlatípus** \> **Főszámla-kategóriák** \> **Fő számla**. Egyes jelentéseknél azonban további mezők is vannak, például Ország és Régió. A hierarchia további csomópontjai az egyes tranzakciók analitikus adatain alapulnak.

Az oszlopok esetében a hierarchia a jogi személyekre és a pénzügyi időszakokra koncentrál. A legtöbb pénzügyi kimutatásnál az oszlop hierarchiája a következő: **Jogi személy** \> **Pénzügyi naptár** \> **Pénzügyi év** \> **Negyedév** \> **Időszak**.

Jelenleg a pénzügyi kimutatások nem támogatják az olyan szervezeti hierarchiákat, amelyek lehetővé teszik az adatok összesítését.

## <a name="data-limitations"></a>Adatkorlátozások
A pénzügyi kimutatási vizuális elemeknél a megjeleníthető sorok száma korlátozott. Jelenleg a korlát értéke 30 000. Ha meghaladja ezt a határértéket, akkor a vizuális elem figyelmeztető szimbólummal tájékoztatja a helyzetről.

![Adatkorlátozások](./media/data-limit.png)

A maximális érték túllépése esetén a pénzügyi kimutatásban megjelenő összegek helytelenek lesznek, mert nem minden sor kerül be a vizuális elembe.

### <a name="empty-rows"></a>Üres sorok
Power BI nem támogatja az üres sorok elrejtését és megjelenítését. Ha egy sor nem tartalmaz adatokat, a sor nem jelenik meg a vizuális elemben.


## <a name="additional-resources-for-power-bi"></a>További erőforrások a Power BI szolgáltatáshoz

Az alábbi erőforrásokban található információk nem szükségesek **Pénzügyi igazgató áttekintés** vagy **Financial Insights** munkaterületre vonatkozó beágyazott jelentések éles környezetben történő engedélyezéséhez. Ehelyett hasznosak fejlesztői célokra, és ha saját Power BI jelentéseit szeretné beágyazni.

- <https://blogs.msdn.microsoft.com/dynamicsaxbi/2017/07/29/accessing-analytical-workspaces-on-1box-environment/>

- <https://docs.microsoft.com/dynamics365/unified-operations/dev-itpro/analytics/add-analytics-tab-workspaces>
