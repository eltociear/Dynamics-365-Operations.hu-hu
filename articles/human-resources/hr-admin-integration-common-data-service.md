---
title: Common Data Service-integráció konfigurálása
description: A Common Data Service és a Microsoft Dynamics 365 Human Resources egy példánya között be- és kikacsolhatja az integrációt. Ezenkívül megtekintheti a szinkronizálási adatokat, törölheti a nyomonkövetési adatokat, valamint újraszinkronizálhat egy entitást a két környezet közötti adatproblémák elhárítása érdekében.
author: andreabichsel
manager: AnnBe
ms.date: 02/03/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-human-resources
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Human Resources
ms.custom: 7521
ms.assetid: ''
ms.search.region: Global
ms.author: anbichse
ms.search.validFrom: 2020-02-03
ms.dyn365.ops.version: Human Resources
ms.openlocfilehash: 042daf3fdf7a906086af726472da050467d217e3
ms.sourcegitcommit: 40163705a134c9874fd33be80c7ae59ccce22c21
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/03/2020
ms.locfileid: "3009252"
---
# <a name="configure-common-data-service-integration"></a>Common Data Service-integráció konfigurálása

A Common Data Service és a Microsoft Dynamics 365 Human Resources egy példánya között be- és kikacsolhatja az integrációt. Ezenkívül megtekintheti a szinkronizálási adatokat, törölheti a nyomonkövetési adatokat, valamint újraszinkronizálhat egy entitást a két környezet közötti adatproblémák elhárítása érdekében.

Ha kikapcsolja az integrációt, a felhasználók módosíthatják az emberi erőforrásokat vagy a Common Data Service megoldást, de ezek a módosítások nem szinkronizálhatók a két környezet között.

Alapértelmezés szerint a Human Resources és a Common Data Service megoldás közötti integráció kikapcsolt vagy bekapcsolt állapotban van a környezetekben lévő bemutatóadatok jelenlététől függően:

- **Kikapcsolva** olyan új környezetek számára, amelyek nem tartalmaznak bemutatóadatokat
- **Bekapcsolva** olyan új környezetek számára, amelyek tartalmaznak bemutatóadatokat

A bemutatóadatokat tartalmazó új környezetek a létesítéskor megkezdik az adatok szinkronizálását.

Előfordulhat, hogy a következő helyzetekben ki szeretné kapcsolni az integrációt:

- Az adatokat az adatkezelési keretrendszeren keresztül tölti ki, és az adatokat többször kell importálni, hogy a megfelelő állapotba kerüljenek.

- Probléma adódott az adatokkal a Human Resources vagy a Common Data Service programok valamelyikében. Ha kikapcsolta az integrációt, akkor úgy törölhet egy rekordot az egyik környezetből, hogy az a másikban megmarad. Amikor újra bekapcsolja az integrációt, az a rekord, amelynek környezetében nem történt törlés, újra visszaszinkronizálódik abba a környezetbe, ahonnan törölte azt. A szinkronizálás azután kezdődik, hogy a **Common Data Service-integráció nem fogadott kérelemszinkronizálási** kötegelt feladatot futtatja.

> [!WARNING]
> Az adatintegráció kikapcsolásakor ügyeljen arra, hogy ne szerkessze mindkét környezetben ugyanazt a rekordot. Az integráció visszakapcsolásakor az utoljára szerkesztett rekordot szinkronizálja a rendszer. Ezért ha nem ugyanazokat a változtatásokat hajtotta végre a rekordon mindkét környezetben, adatvesztés léphet fel.

## <a name="access-the-common-data-service-integration-page"></a>A Common Data Service-integráció oldal elérése

1. Abban a Human Resources példányban, ahol megtekinteni vagy konfigurálni szeretné a Common Data Service rendszerrel való integrációs beállításokat, válassza ki a **Rendszerfelügyelet** csempét.

    [![Rendszerfelügyelet csempe](./media/hr-select-system-administration.png)](./media/hr-select-system-administration.png)

2. Válassza ki a **Hivatkozások** lapot.

    [![Hivatkozások lap](./media/hr-system-administration-links.png)](./media/hr-system-administration-links.png)

3. Az **Integrációk** menüpontban válassza a **Common Data Service konfigurációja** elemet.

    [![Common Data Service konfigurációs hivatkozása](./media/hr-select-common-data-service-configuration.png)](./media/hr-select-common-data-service-configuration.png)

## <a name="turn-data-integration-between-human-resources-and-common-data-service-on-or-off"></a>Adatintegráció be- vagy kikapcsolása a Human Resources és a Common Data Service között

- Ha be szeretné kapcsolni az integrációt, állítsa be, hogy az **Integráció engedélyezése a Common Data Service rendszerben** beállításának értéke **Igen** legyen.

    > [!NOTE]
    > Amikor bekapcsolja az integrációt, az adatok szinkronizálása az után történik meg, hogy a **Common Data Service-integráció nem fogadott kérelemszinkronizálási** kötegelt feladatot futtatja. Minden adatnak elérhetőnek kell lennie a kötegelt feladat befejezése után.

- Ha ki szeretné kapcsolni az integrációt, állítsa át a beállítást **Nem** értékre.

[![Common Data Service-integráció be- és kikapcsolása](./media/hr-enable-or-disable-common-data-service-integration.png)](./media/hr-enable-or-disable-common-data-service-integration.png)

## <a name="view-data-integration-details"></a>Az adatintegráció részleteinek áttekintése

Az **Adminisztráció** gyorslapon, amely a **Common Data Service-integráció** oldalon található, megtekintheti a rekordok összekapcsolásának módját a Human Resources és a Common Data Service között.

- Egy entitás rekordjainak megtekintéséhez válassza ki az entitást a **CDS-entitás neve** mezőben. A rács a kiválasztott entitáshoz kapcsolódó összes rekordot megjeleníti.

[![Entitás rekordjainak megtekintése](./media/hr-common-data-service-configuration-view-entity.png)](./media/hr-common-data-service-configuration-view-entity.png)

> [!NOTE]
> Jelenleg nem minden Common Data Service-entitás szerepel a listán. Csak olyan entitások jelennek meg, amelyek támogatják az egyéni mezők használatát a rácsban. Az új entitások a Human Resources folyamatos termékkiadásai révén válnak elérhetővé.

A rács a következő mezőket tartalmazza:

- **CDS-entitás neve** – a Common Data Service rendszerben található entitás neve.
- **CDS-entitás referenciája** – a Common Data Service által rekord azonosítására használt azonosító. Ez az érték egyenértékű a Human Resources rendszerben található **RecId**-értékkel. Az azonosítót akkor találja meg, ha megnyitja a Common Data Service-entitást a Microsoft Excel programban.
- **Human Resources-entitás neve** – az az entitás, amely utoljára szinkronizált adatokat a Common Data Service rendszerbe. Az entitás Common Data Service előtaggal vagy egy másik előtaggal rendelkezik.
- **Human Resources-referencia** – az a **RecId**-érték, amely a Human Resources alkalmazásban található rekordhoz van társítva.
- **Törölve a CDS-ből** – az az érték, amely azt jelzi, hogy a rekordot törölték-e a Common Data Service rendszerből.

## <a name="remove-the-association-of-a-record-in-human-resources-from-common-data-service"></a>A Common Data Service rendszerből való rekordtársítás eltávolítása a Human Resources rendszerben

Ha problémák merülnének fel a Human Resources és a Common Data Service közötti adatszinkronizálás során, a nyomon követés törlésével és a nyomonkövetési tábla újraszinkronizálásával feloldhatja őket. Ha eltávolítja a társítást, majd módosítja vagy törli a rekordot a Common Data Service rendszerben, a rendszer a módosításokat nem szinkronizálja a Human Resources alkalmazással. Ha módosításokat hajt végre a Human Resources alkalmazásban, létrejön egy új nyomonkövetési rekord, majd a rekord frissül a Common Data Service rendszerben.

- Ha el szeretne távolítani egy rekordtársítást a Human Resources és a Common Data Service között, válassza ki az entitást a **CDS-entitás neve** mezőben, majd válassza a **Nyomonkövetési adatok törlése** elemet.

[![Nyomonkövetési adatok törlése](./media/hr-common-data-service-configuration-clear-tracking.png)](./media/hr-common-data-service-configuration-clear-tracking.png)

Ha szeretné, hogy a nyomon követés törlése után teljes szinkronizálás fusson az entitáson, tekintse meg a következő eljárást.

## <a name="sync-an-entity-between-human-resources-and-common-data-service"></a>Entitás szinkronizálása a Human Resources és a Common Data Service között

Akkor használja ezt az eljárást, ha a Common Data Service rendszerben végrehajtott módosítások túl sokára jelennek meg a Human Resources alkalmazásban, vagy ha a nyomon követés törlése után újra frissíteni kell a nyomonkövetési táblát.

- Ha teljes szinkronizálást szeretne futtatni egy entitáson a Human Resources és a Common Data Service között, válassza ki az entitást a **CDS-entitás neve**  mezőben, majd válassza a **Szinkronizálás most** parancsot.

[![Teljes szinkronizálás futtatása](./media/hr-common-data-service-configuration-sync-now.png)](./media/hr-common-data-service-configuration-sync-now.png)


