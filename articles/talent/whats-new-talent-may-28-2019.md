---
title: Új vagy módosult elemek a Dynamics 365 for Talent szolgáltatásban (2019. május 28.)
description: Ez a témakör a Microsoft Dynamics 365 for Talent új vagy módosított szolgáltatásait írja le.
author: Darinkramer
manager: AnnBe
ms.date: 05/28/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: anbichse
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2019-05-28
ms.dyn365.ops.version: Talent
ms.openlocfilehash: c99e0f3637a8d958e31a046eaad6faa57ce3e1e7
ms.sourcegitcommit: 1bf6a8b2f872394a4f242f9ff13c67e8e1ae8f65
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/03/2019
ms.locfileid: "1856281"
---
# <a name="whats-new-or-changed-in-dynamics-365-for-talent-may-28-2019"></a>Új vagy módosult elemek a Dynamics 365 for Talent szolgáltatásban (2019. május 28.)

[!include [banner](includes/banner.md)]

Ez a témakör a Dynamics 365 for Talent új vagy módosított szolgáltatásait írja le.

## <a name="changes-in-attract"></a>Változások az Attract-ben
Ebben a verzióban kisebb hibajavítások találhatók a Dynamics 365 Talent: Attract alkalmazáshoz.

## <a name="coming-soon-in-attract"></a>Hamarosan az Attract alkalmazásban

### <a name="job-approvals-on-home-page"></a>Feladatok jóváhagyása a kezdőképernyőn

A jóváhagyások az irányítópult **Jóváhagyások** szakaszában jelennek meg. A jóváhagyók megtekinthetik a rájuk váró jóváhagyásokat az **Önhöz rendelt** szakaszban, amely megjeleníti a feladat azonosítóját, nevét, egyéb jóváhagyóit és a hozzárendelés dátumát. Azoknak a felhasználóknak, akik a jóváhagyásra elküldenek egy feladatot, megtekinthetik az **Ön által küldött kérések** szakaszban, ahol azokat a jóváhagyókat jelenítik meg, akiknek továbbra is jóvá kell hagynia a feladatot.

## <a name="changes-in-onboard"></a>Változások az Onboard alkalmazásban
Ebben a verzióban kisebb hibajavítások találhatók a Dynamics 365 Talent: Onboard alkalmazáshoz.

## <a name="changes-in-core-hr"></a>A Core HR módosításai
A szakaszban ismertetett módosítások a 8.1.2319-ös buildre vonatkoznak.

### <a name="common-data-service-entity-support-for-custom-fields"></a>Common Data Service entitás-támogatás egyéni mezőkhöz

Ebben a kiadásban a következő Common Data Service-entitások most támogatják az egyéni mezőket: Juttatási számítások részletei, Munkanaptár ünnepsorai és Foglalkoztatás.

### <a name="copy-position-now-includes-payroll-details"></a>A pozíció másolása most tartalmazza a bérlista adatait
Ha a **Pozíció másolása** lehetőséget használja, és az össze beállítást kiválasztja, akkor a bérlistaadatokat is tartalmazza a másolati információ. 

## <a name="in-preview-in-core-hr"></a>Előzetes a Core HR szolgáltatásban

### <a name="restrict-the-leave-types-in-time-off-requests"></a>A szabadság típusának korlátozása a távolléti kérelmekben

A szervezetek számos különböző típusú szabadságot tudnak nyújtani az alkalmazottak számára. Előfordulhat, hogy a szabadságtípusoknak egy része nem küldhető el távollétként az alkalmazottak által, és ezeket az Emberi erőforrás (HR) kezeli. Ebben a kiadásban konfigurálhatja, hogy az alkalmazottak milyen szabadságtípusokból küldhetnek távolléti kérelmeket. 

### <a name="new-page-to-validate-position-hierarchy-data"></a>Új oldal a beosztás-hierarchia adatainak ellenőrzéséhez

A HR és a rendszergazdák most ellenőrizni tudják a vezetői hierarchiát a véletlenül importált körkörös hivatkozások tekintetében. Ezt az új lapot a **Szervezeti adminisztráció > Hivatkozások > Beosztások > Beosztáshierarchia ellenőrzése** helyről érheti el.

### <a name="specify-reason-codes-on-leave-types"></a>Okkódok meghatározása a távollét típusaihoz

A szervezeteknek kiegészítő információkra lehet szüksége a szabadságkérelmekkel kapcsolatban. Immár megadhat okkódokat egy adott távolléttípushoz, és megengedheti az alkalmazottak számára okkód választását szabadságkérelmükhöz.

### <a name="require-reason-codes-for-specific-leave-types-on-time-off-requests"></a>Okkódok kérése adott szabadságtípusokhoz a távollétkérelmek során

Előfordulhat, hogy a szervezetek okkódok beállítását kérik, bizonyos távolléttípusokhoz, amikor a munkavállalók távolléti kérelmeket nyújtanak be. Ez a követelmény a vállalat szabályzata vagy a törvényi követelmények miatt állhat fenn. Meghatározhatja, mely szabadságtípusokhoz szükséges okkód, és alkalmazottaktól megkövetelheti okkód megadását a szabadságtípushoz a távollétkérelmekhez.

### <a name="provide-a-leave-and-absence-transaction-list-for-hr"></a>Egy szabadság és a távolléti tranzakciólista átadása a HR-nek

Az alkalmazotti szabadidő követésének képessége és a szabadidő kiszámításának ismerete azon túl. hogy segít a HR-nek alkalmazott kérdések megválaszolásában, pontos szabadságmegítéléseket biztosít a munkavállalóknak. A HR új betekintést kap a tranzakciókhoz (támogatások, könyvelések, kiigazítások és kérelmek) így a HR munkatársai láthatják a távollétegyenlegek okait.