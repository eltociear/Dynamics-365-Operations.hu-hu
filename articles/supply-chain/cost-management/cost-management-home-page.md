---
title: Költségkezelés kezdőlap
description: A költségkezeléssel kezelheti a nyersanyagok, a félkésztermékek, késztermékek és a folyamatban lévő eszközök értékelését és könyvelését.
author: AndersGirke
manager: AnnBe
ms.date: 04/25/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CostAdminWorkspace, CostAnalysisWorkspace
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: aevengir
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: dd51fa667fd48b7bab64c3566b616631c6f9bcd1
ms.sourcegitcommit: 2460d0da812c45fce67a061386db52e0ae46b0f3
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/30/2019
ms.locfileid: "2249632"
---
# <a name="cost-management-home-page"></a>Költségkezelés kezdőlap

[!include [banner](../includes/banner.md)]

A [költségkezeléssel (videó)](https://www.youtube.com/watch?v=vXzlC-mOBcg&feature=youtu.be) kezelheti a nyersanyagok, a félkésztermékek, késztermékek és a folyamatban lévő eszközök értékelését és könyvelését. Nem más, mint a [Készletkönyvelés](cost-object.md) és a [Gyártási könyvelés](bom-calculations.md) meghatározásának, kezelésének és jelentésének folyamata.

Az alábbi területeken állíthatók be költségirányelvek: 
-  [Előre meghatározott költség](costing-versions.md)
-  [Készletkönyvelés](cost-object.md)
-  [Gyártási könyvelés](bom-calculations.md)
-  [Közvetett költségkönyvelés](costing-sheets.md)
-  [Főkönyvi könyvelés](production-order-cost-analysis.md)

Meghatározhatja például, hogy mely készletértékelési módszert (pl. [FIFO](fifo-physical-value-marking.md), [Súlyozott átlag](weighted-average-physical-value-marking.md), [Elszámolóár](prerequisites-standard-costs.md) vagy [Mozgó átlag](moving-average.md) szeretné alkalmazni a [Cikkmodellcsoport](../inventory/reserve-inventory-quantities.md) termékeinél a Készletkönyvelésnél.

A Készletkönyvelés és Gyártási könyvelés elemeket a **Költségadminisztráció** és a **Költségelemzés** munkaterületekről érheti el. Ezek a munkaterületek átfogó áttekintést nyújtanak a jelenlegi állapotról, a fő teljesítménymutatókról (KPI-kről), valamint az eltérések észleléséről. 

A Gyártási könyvelés segítségével kezelheti a [Feladatrendeléses költségelszámolást](production-order-cost-analysis.md) a gyártási rendeléseknél és a kötegelt rendeléseknél, továbbá a [Visszavezetéses költségelszámolást](backflush-costing.md) a lean gyártásnál.

A [Költségkezelés Power BI-tartalom](../../dev-itpro/analytics/cost-management-content-pack.md) betekintést biztosít a vezetők számára a készletbe és a befejezetlen termelés készletébe, illetve az ezeken belüli, kategóriánkénti költségáramlásba időalapú lebontásban. Az információk pénzügyi kimutatás részletes kiegészítéseként felhasználhatók.

### <a name="additional-resources"></a>További erőforrások

#### <a name="whats-new-and-in-development"></a>Újdonságok és fejlesztés alatt levő megoldások

Keresse fel a [Microsoft Dynamics 365 Ütemterv](https://roadmap.dynamics.com/) oldalt a már kiadott új funkciók és a kidolgozás alatt álló új szolgáltatások megtekintése érdekében. 

#### <a name="white-paper"></a>Útmutató
A [Darabjegyzék-számítás költségszámítási táblázat segítségével](https://mbs.microsoft.com/customersource/northamerica/AX/learning/documentation/white-papers/365operationsbomcalsheet) című rész ismerteti az anyagokat és a gyártást tartalmazó költségszámítási táblázat beállítását, valamint hogy a beállítás hogyan befolyásolja az anyagjegyzék-számítás eredményét. A témakör jobb magyarázata érdekében konkrét forgatókönyveket és adatokat biztosít, melyek bemutatják a különböző beállítások és konfigurációk hatását. Nem várjuk el, hogy kövesse ezeket a forgatókönyveket, mert ez a dokumentum nem nyújt elegendő részletet a konfigurálásukról. Ha azonban megvan az alaptudása, megpróbálhatja lejátszani az alább felsorolt feladatútmutatókat a megjelenésük sorrendjében. A jelen dokumentum elolvasásából szerzett tudása segítségével elkészítheti az anyagjegyzék-számítás elemzését. 

-  [Késztermék létrehozása](tasks/create-finished-product-2016-02.md)
-  [Félkész termék létrehozása](tasks/create-semi-finished-product-2016-02.md)
-  [Nyersanyagok létrehozása](tasks/create-raw-materials-2016-02.md)
-  [Anyagjegyzékek létrehozása](tasks/create-boms-2016-02.md)
-  [Útvonalak létrehozása](tasks/create-routes-2016-02.md)
-  [Anyagjegyzék-számítás elvégzése egyetlen szintű struktúra használatával](tasks/calculate-bom-single-level-structure-2016-02.md)
-  [Anyagjegyzék-számítás elvégzése több szintű struktúra használatával](tasks/calculate-bom-multilevel-structure-2016-02.md)


#### <a name="blogs"></a>Blogok
A [Dynamics AX Manufacturing kutatás-fejlesztési csapatának blogjában](https://blogs.msdn.microsoft.com/axmfg) és a [Supply Chain Management in Dynamics AX kutatás-fejlesztési csapatának blogjában](https://blogs.msdn.microsoft.com/dynamicsaxscm) számos vélemény, hír és egyéb információ található a költségkezelésről. A bejegyezések egy része ugyan a Költségkezelés előző verziójához íródott, de ugyanazon fogalmak érvényesek továbbra is, és az eljárások is hasonlóak az aktuális verzióban.

#### <a name="task-guides"></a>Feladat-útmutatók
További súgó áll rendelkezésére feladat útmutatókon belül. A feladat-útmutatók eléréséhez kattintson bármelyik lapon a Súgó gombjára.

