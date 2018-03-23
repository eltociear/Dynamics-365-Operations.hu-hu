---
title: "Szortiment kezelése"
description: "Ez a témakör bemutatja a Microsoft Dynamics 365 for Retail szortimentkezelésének az alapfogalmait, és tartalmaz a megvalósítással kapcsolatos szempontokat a projekt számára."
author: jblucher
manager: AnnBe
ms.date: 3/12/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-365-retail
ms.technology: 
audience: Application user
ms.search.scope: Retail, Operations
ms.search.region: Global
ms.author: jeffbl
ms.search.validFrom: 2017-11-21
ms.dyn365.ops.version: Application update 5
ms.translationtype: HT
ms.sourcegitcommit: 44b0c4e39ac7410d27ce531c898bb8c423af334a
ms.openlocfilehash: 303f86d6a57e039cb51700744697949845239b10
ms.contentlocale: hu-hu
ms.lasthandoff: 03/12/2018

---

# <a name="assortment-management"></a>Szortiment kezelése
[!include[banner](../includes/banner.md)]

## <a name="overview"></a>Áttekintés
A Microsoft Dynamics 365 for Retail *szortimenteket* tartalmaz, amelyekkel csatornákon keresztül kezelhető a termékek elérhetősége. A szortimentek határozzák meg, hogy mely termékek érhetők el bizonyos üzletekben, és egy adott időszakban.

A Retail esetében a szortiment egy vagy több csatorna (vagy szervezeti hierarchiák használatakor csatornák csoportja) hozzárendelése egy vagy több termékhez (vagy termékcsoportokhez, Kategóriahierarchiák használatakor).

A csatornához rendelt közzétett szortimentek határozzák meg a csatorna teljes termékösszetételét. Emiatt több aktív szortimentet is beállíthat csatornánként.

### <a name="basic-assortment-setup"></a>Alapvető szortiment beállítása
A következő példában egy egyedi szortiment van beállítva minden egyes üzlethez. Ebben az esetben csak az 1. termék érhető el az 1. üzletben, és a 2. üzletben csak a 2. termék érhető el.

![Minden egyes termékek elérhető egy üzletben](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure1.png?raw=true "Minden egyes termékek elérhető egy üzletben")

Ahhoz, hogy a 2. termék rendelkezésre álljon az 1. üzletben, hozzáadhatja a terméket az 1. szortimenthez.

![1. szortimenthez hozzáadott 2. termék](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure2.png?raw=true "1. szortimenthez hozzáadott 2. termék")

Másik lehetőségként hozzáadhatja az 1. üzletet a 2. szortimenthez.

![2. szortimenthez hozzáadott 1. üzlet](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure3.png?raw=true "2. szortimenthez hozzáadott 1. üzlet")

### <a name="organization-hierarchies"></a>Szervezeti hierarchiák
Az olyan helyzetekben, ahol több csatorna osztozik ugyanazon a termékszortimenteken, a szortimentek konfigurálhatók a Retail szortimentszervezeti hierarchia használatával. Ha ebből a hierarchiából ad hozzá csomópontokat, a csomópontban és a gyermek csomópontjaiban levő összes csatorna szerepelni fog.

![Szervezeti hierarchia](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure4.png?raw=true "Szervezeti hierarchia")

### <a name="product-categories"></a>Termékkategóriák
Ehhez hasonlóan a termékoldalon is felvehet termékcsoportokat a termék-kategóriahierarchiák használatával. A szortimentek konfigurálását elvégezheti egy vagy több kategóriahierarchia-csomópont hozzáadásával. Ebben az esetben a szortiment tartalmazni fogja az összes terméket a kategória-csomópontból és gyermek csomópontjaiból.

![Termékkategóriák](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure5.png?raw=true "Termékkategóriák")

### <a name="excluded-products-or-categories"></a>Kizárt termékek vagy kategóriák
A termékek és kategóriák szortimentekhez adásán kívül a kihagyás beállítás segítségével megadhatja azokat a termékeket vagy kategóriákat, amelyeket ki kell zárni a szortimentekből. A következő példában szeretné az összes terméket felvenni egy adott kategóriába, kivéve a 2. terméket. Ebben az esetben nem kell meghatározni a szortimentet termékről termékre, vagy további kategória-csomópontokat létrehozni. Ehelyett megadható csak a kategória, de a termék kizárásával.

> [!NOTE]
> Ha egy termék egyszerre ki van zárva és be van véve egy vagy szortimentbe/szortimentből meghatározás szerint, a termék mindig kizártként lesz figyelembe véve.

![Kizárt termék](https://github.com/MicrosoftDocs/Dynamics-365-Operations/blob/jblucher-manage-assortments/articles/retail/media/Managing-assortments-figure6.png?raw=true "Kizárt termék")

### <a name="global-and-released-products"></a>Globális és kiadott termékek
A szortimentek globális szinten vannak meghatározva, és több jogi személy csatornáit tartalmazhatják. A szortimentekbe befoglalt termékek és kategóriák is több jogi személyek között vannak megosztva. Azonban a termék előbb ki kell adni, mielőtt ténylegesen értékesített, megrendelt, számlált vagy kapott lehet a csatornában (például a pénztárnál \[POS\]). Ebből következően annak ellenére, hogy két különböző jogi személyhez tartozó üzletek megoszthatják azt a szortimentet, amely tartalmazza ugyanazon termékeket, a termékek csak akkor érhetők el, ha azokat a jogi személyek esetében kiadták.

### <a name="dynamic-and-static-assortments"></a>Dinamikus és statikus szortimentek
Szortimentek megadhatók adott csatornákkal és termékekkel, vagy szervezeti egységek és kategóriákat befoglalásával. Az ezekhez a csoportokhoz hivatkozásokat tartalmazó szortimentek dinamikus szortimentnek számítanak. Ha a definíciója vagy a tartalma módosul ezeknek a csoportoknak, amíg a szortiment aktív állapotban van, a szortiment meghatározása is módosulni fog.

Például egy szortimentet eredetileg úgy határoztak meg és tettek közzé, hogy egy termékkategóriára hivatkozik. Ha további termékeket később hozzáadnak a kategóriához, ezek a termékek automatikusan bekerülnek a meglévő szortiment meghatározásába. Nem kell manuálisan hozzáadni a termékeket a szortimenthez. Hasonlóképpen, ha egy szervezeti egységet hozzáadnak egy másik csomóponthoz, a szervezeti egység szortimentje automatikusan korrigálódik az adott definíció alapján.

### <a name="stopped-products"></a>Leállított termékek 
A kiadott termékek „leállíthatók” az értékesítési folyamatra nézve egy beállítás bekapcsolásával az **Alapértelmezett sorrend** beállításban. Ez a beállítás általában akkor használatos, ha egy termék élettartama végére ért, és egyetlen csatornán sem értékesíthető. A szortimentek figyelem veszik ezt a beállítást, és leállított termékek nem kerülnek be a szortimentekbe, függetlenül a szortiment konfigurációjától.

### <a name="blocked-products"></a>Letiltott termék
A termék értékesítésének leállítása mellett ideiglenesen is letilthatja a termék értékesítését. Ez a beállítás a kiadott termékek **Kiskereskedelem** lapján állítható be. A letiltott termékek továbbra is szortimenthez vannak hozzárendelve, de a pénztár egy üzenet jelenít meg, amely arról tájékoztat, hogy a termék nem értékesíthető.

### <a name="date-effectivity"></a>Dátum érvényessége
A szortimentek napra időzíthetők. Ezért a kiskereskedők beállíthatják, hogy a termékek mikor legyenek elérhetők és nem elérhetők, csatornánként. Meghatározhat és előre közzétehet szortimenteket, és megadhatja a kezdő és záró dátumokat. A termékek automatikusan lesznek elérhetők vagy nem elérhetők a megadott dátumokon.

### <a name="process-assortments-batch-job"></a>Szortiment kötegelt feladat végrehajtása
A Retailben meghatározott szortimenteket az életbe lépés előtt fel kell dolgozni. Ez a feldolgozás a következő okok miatt történik meg:

- A szortimentdefiníciókat denormalizálni kell, hogy a csatornák könnyen feldolgozhassák őket. Az adott csatorna termékkombinációját több szortimenttel lehet megadni, amelyek különböző dátumtartományokra terjednek ki. Ha az adatok egy részét előre kiszámítják a kiszolgálón, a csatorna teljesítménye növekszik.
- A termékek és a csatornák a szortimentben magán a szortimenten kívül is módosulhatnak. A dinamikus szortimenteket, amelyek hivatkozásokat tartalmaznak a kategóriákra vagy szervezeti egységekre, rendszeres időközönként fel kell dolgozni, hogy magukban foglalják vagy kizárják a rekordokat, a jelenlegi hozzárendelés alapján.

## <a name="implementation-considerations"></a>Kivitelezési szempontok
A következő végrehajtási követelményeket figyelembe kell venni a szortimentek tervezése és kezelése során a kiskereskedelmi implementációhoz:

- **Adatok replikációja és az adatbázis mérete** – Miközben a szortimentek segítenek kiszolgálni a termékek elérhetőségének kezelésére vonatkozó üzleti igényt, a csatorna és offline adatbázis méretének kezelésére szolgáló fontos eszközök is. A jól felügyelt szortimentek csökkentik az adatmennyiséget, amelyet fel kell dolgozni és replikálni kell a csatorna és offline adatbázisokba. Segítenek a megőrzendő rekordok számának csökkentésében is. Ha kevesebb rekord van az adatbázisokban, növekszik a teljesítmény, amikor cikkeket ad hozzá egy tranzakcióhoz, keres, és termékeket tallóz.
- **Hatályba lépő/lejáró szortimentek** – Az egyik leghatékonyabb eszközök a termékek számának kezeléséhez a csatorna és offline adatbázisokban a szortimentek érvényesség dátumainak használata. Ha a szezonális termékek vagy az élettartamuk végére érő termékek esetében nyílt (nem lejáró) szortimenteket alkalmaz, az adatbázisokat vég nélkül fognak nőni. Többféle módszer segítségével kezelheti ezt a helyzetet. Például külön szortimenteket tarthat fenn a szezonális termékeknek, és az olyan termékeknek, amelyek mindig rendelkezésre állnak.
- **Értékesítés és visszáru a szortimenteken kívül** – Ez a lehetőség segítséget nyújt a kiskereskedőknek a szortimentek hatékony kezeléséhez úgy, hogy a rendelkezésre álló termékeket az üzlet alapvető termékmixére korlátozzák. Ez a lehetőség azt is lehetővé teszi a kiskereskedők számára, hogy sikeresen kezeljék azokat a helyzeteket, amikor a termék véletlenül kimaradt egy szortimentből, vagy egy terméket a szortiment érvényességi dátumait kívül hoztak vissza.

Ha egy termékadat nem szerepel a csatorna-adatbázisban, a pénztár valós idejű hívást intéz a központhoz, hogy lekérje a szükséges adatokat, és így megtörténhessen a termék értékesítése, visszavitele vagy elhelyezése egy vevői rendelésen. Az ezen a módon lekért termékinformációk csak az adott tranzakció hatóköre során érhetők el. A termék nincs hozzáadva a szortiment definíciójához. Ennek megfelelően a későbbi valós idejű hívások szükség szerint történnek meg.
