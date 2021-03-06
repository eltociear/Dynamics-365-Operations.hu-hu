---
title: Projekt tényleges adatainak közvetlen szinkronizálása a Project Service Automation alkalmazásból közvetlenül a projektintegrációs naplóba a feladáshoz a Finance and Operations alkalmazásba
description: Ez a témakör bemutatja a sablonokat és a mögöttes feladatokat, amelyek a Microsoft Dynamics 365 Project Service Automation aktuális projektjeinek közvetlenül a Finance and Operations alkalmazásba történő szinkronizálására használatosak.
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 302ac0f456dd8a24dc02948ee657e359f5a9c844
ms.sourcegitcommit: fbc106af09bdadb860677f590464fb93223cbf65
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/06/2019
ms.locfileid: "2770335"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a>Projekt tényleges adatainak közvetlen szinkronizálása a Project Service Automation alkalmazásból közvetlenül a projektintegrációs naplóba a feladáshoz a Finance and Operations alkalmazásba

[!include[banner](../includes/banner.md)]

Ez a témakör bemutatja a sablonokat és a mögöttes feladatokat, amelyek a Dynamics 365 Project Service Automation aktuális projektjeinek közvetlenül a Dynamics 365 Finance szolgáltatásba történő szinkronizálására használatosak.

A sablon szinkronizálja a tranzakciókat a Project Service Automation alkalmazásból a Finance egy előkészítési táblájába. Szinkronizálás befejezése után, importálnia **kell** az adatokat az előkészítő táblából a integrációs naplóba.

> [!NOTE]
> - A projekt tényleges adatok integráció a 8.0.1 vagy újabb verzióiban érhető el.
> - Amennyiben az Enterprise edition 7.3.0-ás verziót használja, a KB 4132657 és KB 4132660 telepítését követően, használhat sablonokat projektfeladatok, kiadási tranzakciókategóriák, becsült órák, becsült kiadások és a tényleges értékek integrálásához, és a funkciók zárolásának beállításához. Ha a könyvelési felosztásokat kell visszaállítania, ajánlott a KB 4131710 telepítése is.
> - Ha a 7.3.0 verziót használja, tranzakciókat hív be a Project Service Automation alkalmazásból, telepítenie kell KB 4345320 frissítést annak érdekében, hogy a díjakat megjelenítse a projektszámlán.
> - Ha időhöz kapcsolódó áfát vagy kiadási tranzakciókat visz be visz be a Project Service Automationbe , telepíteni kell a Project Service Automation Update 7 frissítést. Máskülönben a tényleges adó nem lesz csatolva a kapcsolódó tényleges időhöz vagy a költséghez, és nem lesz szinkronizálva a Finance alkalmazásba. Forduljon a támogatáshoz további információért.

## <a name="data-flow-for-project-service-automation-to-finance"></a>Adatáramlás a Project Service Automation és a Finance között

A Project Service Automation és a Finance közötti integrációs megoldás az adatintegrációs funkciót használja a Project Service Automation és Finance példányok közötti szinkronizáláshoz. Az integrációs sablonok, amelyek elérhetőek az adatintegrációs funkcióval lehetővé teszik a projekt tényleges adatainak áramlását a Project Service Automation alkalmazásból a Finance alkalmazásba.

A következő ábra bemutatja a Project Service Automation és a Finance közötti adatszinkronizálást.

[![Adatáramlás a Project Service Automation és a Finance and Operations integrációjához](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)

## <a name="project-actuals-from-project-service-automation"></a>Projekt tényleges adatai a Project Service Automation alkalmazásból

### <a name="template-and-tasks"></a>Sablon és feladatok

A rendelkezésre álló sablonok eléréséhez a Microsoft Power Apps adminisztrációs központban válassza a **Projektek** lehetőséget, majd kattintson a jobb felső sarkában **Új projekt** lehetőségre a nyilvános sablonok kiválasztásához.

A következő sablon és alapul szolgáló feladatok használható az aktuális projektfeladatok szinkronizálásához a Project Service Automation és Finance között:

- **Sablon neve az adatintegrációban:** Projekt tényleges adatai (PSA to Fin and Ops)
- **A projekt tevékenységeinek nevei:**

    - Tényadatok
    - TransactionConnections

### <a name="entity-set"></a>Entitás beállítása

| Project Service Automation | Pénzügy                                   |
|----------------------------|----------------------------------------------------------|
| Tényadatok                    | Integrációs entitás a projekt tényleges adataihoz                   |
| Tranzakciók kapcsolatai    | Projekttranzakció-kapcsolatok integrációs entitása |

### <a name="entity-flow"></a>Entitás folyamata

Projekt tényleges adatainak kezelése a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a projektintegrációs naplóba a Finance alkalmazásba. A könyvelés az alapértelmezett pénzügyi dimenziók és a feladási beállítások alapján lesz alkalmazva.

### <a name="prerequisites"></a>Előfeltételek

Tényleges adatok szinkronizálása előtt, a Project Service Automation integrációs paramétereit be kell állítani, és szinkronizálni kell a projekteket, projektfeladatokat és projektköltség-tranzakció kategóriákat.

### <a name="power-query"></a>Power Query

A Microsoft Power Query for Excelt a következőkre kell használnia a projekt tényleges adatai sablonban ezen feladatok elvégzéséhez:

- A Project Service Automation tranzakciótípus átalakítására a megfelelő tranzakciótípusra a Finance alkalmazásban. A Projekt tényleges adatai (Fin és Ops PSA) sablon már definiálta az átalakítást.
- A Finance számlázási típus átalakítása a megfelelő számlázási típusra a Project Service Automation alkalmazásban. A Projekt tényleges adatai (Fin és Ops PSA) sablon már definiálta az átalakítást. A számlázási típus ezután hozzá lesz rendelve a sortulajdonság elemhez a **Project Service Automation integrációs paraméterek** képernyő beállításai alapján.
- Szűrés specifikus erőforrás szervezeti egységekre, amelyek e sablonnal szinkronizálandók.
- Ha a vállalatközi idő vagy tényleges költségek szinkronizálva lesznek a Finance alkalmazásba, át kell alakítani a szerződéses szervezeti egység a megfelelő jogi személy elemre a Finance alkalmazásban. A Projekt tényleges adatai (Fin and Ops PSA) sablonjában van egy feltételes oszlop a bemutató adatok alapján. Az utolsó beszúrt feltételes oszlopot frissítenie kell a megfelelő jogi személyekhez. Ellenkező esetben ez integrációs hibát vagy a helytelen tényleges tranzakciók importálását okozhatja a Finance alkalmazásba.
- Ha idő vagy a tényleges vállalatközi költségek nem lesznek szinkronizálva a Finance alkalmazásba, ki törölnie kell az utolsó beszúrt feltételes oszlopot a sablonból. Ellenkező esetben ez integrációs hibát vagy a helytelen tényleges tranzakciók importálását okozhatja a Finance alkalmazásba.

#### <a name="contract-organizational-unit"></a>Szerződéses szervezeti egység
A beszúrt feltételes oszlop frissítéséhez sablonban kattintson a **Hozzárendelés** nyílra a hozzárendelés megnyitásához. Válassza ki a **Speciális lekérdezés és szűrés** hivatkozást a Power Query megnyitásához.

- Ha az alapértelmezett Microsoft Projekt tényleges adatok (Fin és Ops PSA) sablont használja, a Power Queryben jelölje be a **Beszúrt feltétel** elemet az **Alkalmazott lépések** szakaszban. Az **Funkció** bejegyzésben, cseréje az **USSI** elemet a jogi személy nevére, melyet használni kell, hogy az integrációhoz. Szükség szerint adjon hozzá a további feltételeket a **Funkció** bejegyzéshez, és frissítése a **más** feltételt **USMF** helyett a megfelelő jogi személyre.
- Új sablon létrehozásakor, hozzá kell adnia az oszlopot a vállalatközi idő- és a költségek támogatásához. Válassza a **Feltételes oszlop hozzáadása** elemet, és adjon egy nevet az oszlopnak, például **LegalEntity**. Adjon meg egy feltételt az oszlopnak, ahol, if **msdyn\_contractorganizationalunitid.msdyn\_name** is \<organizational unit\>, then \<enter the legal entity\>; else null.

### <a name="template-mapping-in-data-integration"></a>Sablonleképezés az adatintegrátorban

Az alábbi ábrák egy példát mutatnak a sablonfeladat hozzárendelésére az Adatintegrációban A leképezés mutatja, hogy melyik mezőadatok szinkronizálódnak a Project Service Automation – Finance irányban.

[![Sablon-hozzárendelés](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)

[![Sablon-hozzárendelés](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a>Előkészítési tábla importálása a Project Service Automation integrálását követően

Az importálás előkészítési tábla periodikus folyamatját futtatni a tényleges adatok szinkronizálását követően a Project Service Automation és a Finance között. Ez a folyamat importálja a projekttranzakciókat az előkészítési táblából a Project Service Automation integrációs naplóba, ahol a könyvelés alkalmazva lesz, és fel lehet adni az importált tranzakciókat. Ajánljuk, hogy ez a folyamatot kötegelt módban futtassa, és tetszés szerint beállíthatja, hogy ismétlődő kötegként futtatandó.

## <a name="update-actuals-from-finance"></a>Tényleges adatok frissítése a Finance megoldásból

### <a name="template-and-tasks"></a>Sablon és feladatok

A következő sablon és alapul szolgáló feladatok használhatók a projekttranzakciókhoz feladott bizonylatszámok és áfa szinkronizálásához a Finance és a Project Service Automation között:

- **Sablon neve az adatintegrációban:** Projekt tényleges adatainak frissítése (Fin Ops to PSA)
- **A projekt tevékenységeinek nevei:**

    - Tényadatok 
    - TransactionConnections

### <a name="entity-set"></a>Entitás beállítása

| Pénzügy                                                  | Project Service Automation |
|----------------------------------------------------------|----------------------------|
| Integrációs entitás a projekt tényleges adataihoz                   | Tényadatok                    |
| Projekttranzakció-kapcsolatok integrációs entitása | Tranzakciók kapcsolatai    |

### <a name="entity-flow"></a>Entitás folyamata

Projekt tényleges adatainak kezelése a Project Service Automation alkalmazásban történik, majd ezek szinkronizálva lesznek a projektintegrációs naplóba a Finance alkalmazásba. Miután a tényleges értékek fel lettek adva a Finance alkalmazásba ezek frissülnek a Project Service Automation alkalmazásban a Finance bizonylatszámaival. Ha adók is hozzá lettek adva a Finance alkalmazásban, új tényleges adóértékek lesznek létrehozva a Project Service Automation alkalmazásban.

### <a name="power-query"></a>Power Query

A Microsoft Power Queryt a következőkre kell használnia a projekt tényleges adatai frissítési sablonban ezen feladatok elvégzéséhez:

- A Finance tranzakciótípus átalakítására a megfelelő tranzakciótípusra a Project Service Automatio alkalmazásban. A Projekt tényleges adatai frissítése (Fin Ops és PSA) sablon már definiálta az átalakítást.
- A Project Service Automation számlázási típus átalakítása a megfelelő számlázási típusra a Finance alkalmazásban. A Projekt tényleges adatai frissítése (Fin Ops és PSA) sablon már definiálta az átalakítást.

### <a name="template-mapping-in-data-integration"></a>Sablonleképezés az adatintegrátorban

Az alábbi ábrán példákat láthat sablonfeladatok hozzárendelésére az Adatintegrációban A leképezés mutatja, hogy melyik mezőadatok szinkronizálódnak a Finance – Project Service Automation irányban.

[![Sablon-hozzárendelés](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)

[![Sablon-hozzárendelés](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)
