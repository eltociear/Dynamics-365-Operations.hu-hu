---
title: "Költségkönyvelési elemzés Power BI-tartalom"
description: "Ez a témakör a Költségkönyvelési elemzés Power BI-tartalom modul tartalmát ismerteti. Leírja, hogy hogyan kell hozzáférni Power BI-jelentésekhez, és információkat nyújt a tartalom összeállításához használt entitásokkal és adatmodellekkel kapcsolatban."
author: AndersGirke
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 270274
ms.assetid: b74549df-35d5-4f2f-b3c7-405b0d38ea78
ms.search.region: Global
ms.author: aevengir
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: 1d19276331a4278f44ad14292ed434c49b74d727
ms.contentlocale: hu-hu
ms.lasthandoff: 06/13/2017

---

# <a name="cost-accounting-analysis-power-bi-content"></a>Költségkönyvelési elemzés Power BI-tartalom

[!include[banner](../includes/banner.md)]

Ez a témakör a **Költségkönyvelési elemzés** Microsoft Power BI-tartalom modul tartalmát ismerteti. Leírja, hogy hogyan kell hozzáférni Power BI-jelentésekhez, és információkat nyújt a tartalom összeállításához használt entitásokkal és adatmodellekkel kapcsolatban.

## <a name="overview"></a>Áttekintés

A **Költségkönyvelési elemzés** Power BI-tartalom költségellenőrök, illetve olyan személyek részére készült, aki a szervezetük költségellenőrzéséért felelősek. Kulcsfontosságú mérőszámokat foglal magában, például költség, nagyság, illetve költségszorzó és tényleges költség, tervezett költség és rugalmas tervezett költség alapján. A **Költségkönyvelés** modul tranzakciós adatait használja, és összesítő nézetet biztosít a teljes szervezet költségeiről egyetlen kimutatási pénznemben. A vezetők szűrhetik az adatokat költségobjektumok szerint szervezeti egységeik költségkontrollja számára akkor is, ha a szervezet több jogi személyből állhat. 

Mvel a **Költségkönyvelési elemzés** tartalom kiemeli a tényleges és tervezett költségek közötti eltéréseket, a vezetők értesítésülhetnek a működési egységeiknél fellépő pozitív és negatív tendenciákról. A vezetők az egyes költségtényezők költségtényező-hierarchiájáig leáshatnak. A vezetők ily módon részletes bepillantást nyerhetnek a költségeltérések megtörténtének módjába, majd eredményes intézkedéseket tehetnek. 

A **Költségkönyvelési elemzés** tartalom segítségével a költségkönyvelők elemezhetik a költségek átfolyását a teljes szervezet költségobjektumain. 

A Költségkönyveléssel kapcsolatos további tudnivalókért lásd: [Költségkönyvelési honlap](/dynamics365/unified-operations/financials/cost-accounting/cost-accounting-home-page). 

A Költségkönyvelésben hozzáférési szintű biztonság beállításával és ezt a Power BI sorszintű biztonságával kombinálva az összes költségobjektum-tulajdonos számára hozzáférést biztosíthat a **Költségkönyvelési elemzés** Power BI-tartalomhoz. Így a képi megjelenítések összes adatának szűrése a Költségkönyvelésben vezérelt hozzáférési szint alapján történik. Ha többet szeretne megtudni a hozzáférési szintű biztonságról és a sorszintű biztonságról, lásd: [Biztonság beállítása költségkönyvelési tartalomhoz a Power BI-ban](setup-security-cost-accounting-content-pack.md).

## <a name="accessing-the-power-bi-content"></a>Power BI-tartalom elérése
A **Költségkönyvelési elemzés** Power BI-tartalom a Microsoft Dynamics Lifecycle Services (LCS) megosztott eszközök könyvtárban található. A tartalom letöltésére és szervezeténél való megvalósítására vonatkozó további információért lásd: [Power BI-tartalom az LCS megoldásban a Microsofttól és a partnerektől](power-bi-content-microsoft-partners.md). Ha meg szeretne tekinteni egy demót, amely bemutatja a Power BI-tartalmak megvalósítását, lásd a [Power BI-tartalom a Microsofttól és az Ön partnereitől a Dynamics Lifecycle Services szolgáltatásban](https://mix.office.com/watch/9puyb1b2xs1w) című részt (Office Mix).

Mindenképp töltse le azt a **Költségkönyvelési elemzés** Power BI-tartalmat, amelyik a Microsoft Dynamics 365 Ön által használt verziójához készült.

> [!NOTE]
> A KB 4011327 ezen Power BI-tartalom előfeltétele. Az LCS-be való bejelentkezést követően itt férhet hozzá a tudásbázishoz: <https://fix.lcs.dynamics.com/issue/results/?q=kb4011327>.

## <a name="metrics-that-are-included-in-the-power-bi-content"></a>A Power BI-tartalomhoz tartozó metrikák
A tartalom jelentési oldalak készletét tartalmazza. Minden oldal több metrikát tartalmaz, amelyek diagramok, mozaikok, táblázatok formájában jeleníthetők meg. Az alábbi táblázatban a **Költségkönyvelési elemzés** Power BI-tartalom megjelenítési formáinak áttekintése található.

| Jelentéslap                      | Diagram                                                                                                                         | Csempe                                          |
|----------------------------------|-------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------|
| Költségkontroll pénzügyi időszak szerint    | Tényleges költség és tervezett költség költségösszetevő-hierarchiaszint alapján                                                                   | Tényleges költség vs tervezett költség                    |
|                                  | Költségvetés eltérése költségösszetevő-hierarchiaszint alapján                                                                               | Tényleges költségszorzó vs Tervezett költségszorzó          |
|                                  | A 10 legjelentősebb költségvetési eltérés százalékban költségtényezőnként                                                                          | Tényleges nagyság vs Tervezett nagyság          |
| Költségkontroll - folyó év mai napig     | Tényleges költség és Tervezett költség naptári évi időszak szerint                                                                           | Tényleges költség vs tervezett költség                    |
|                                  | Költségvetési eltérés naptári évi időszak szerint                                                                                       | Tényleges költségszorzó vs Tervezett költségszorzó          |
|                                  | A 10 legjelentősebb költségvetési eltérés százalékban költségtényezőnként                                                                          | Tényleges nagyság vs Tervezett nagyság          |
| Költségszorzó pénzügyi év szerint         | Tényleges költségszorzó Költség működése szerint                                                                                             | Tényleges költségszorzó vs Tervezett költségszorzó          |
|                                  | Tényleges költségszorzó, Tervezett költségszorzó-eltérés, Tervezett költségszorzó-százalék és Tervezett költségszorzó költségösszetevő-hierarchiaszint alapján | Tényleges nagyság vs Tervezett nagyság          |
|                                  | Költségvetés eltérése költségösszetevő-hierarchiaszint alapján                                                                               |                                               |
|                                  | A 10 legjelentősebb költségvetési eltérés százalékban költségtényezőnként                                                                          |                                               |
| Rugalmas költségvetés pénzügyi időszak szerint | Tényleges költség, Tervezett költség, Rugalmas tervezett költség költségösszetevő-hierarchiaszint alapján                                             | Tényleges nagyság vs Tervezett nagyság          |
|                                  | Tényleges költség és Rugalmas költségvetési eltérés költségösszetevő-hierarchiaszint alapján                                                  | Tényleges költség vs Rugalmas tervezett költség           |
|                                  | Tényleges költség, Tervezett költség és Rugalmas költség költség működése szerint és költségösszetevő-hierarchiaszint alapján                                  | Tényleges költségszorzó vs Rugalmas tervezett költségszorzó |
| Költségkimutatás pénzügyi időszak szerint  | Tényleges költség költségösszetevő-hierarchiaszint alapján és Költségobjektum-dimenziótagnév                                             |                                               |
|                                  | Tényleges költség Költségobjektum-dimenziótagnév alapján és Költségelem-dimenziótagnév                                       |                                               |

## <a name="understanding-the-data-model-and-entities"></a>Adatmodell, illetve entitások ismertetése
A következő adatokkal tölthetők ki a jelentések oldalau a **Költségkönyvelési elemzés** Power BI-tartalomban. Ezeket az adatokat az Entitástárban lebonyolított összesített mérések jelenítik meg. Az entitástár a Microsoft analitikai célokra optimalizált SQL-szerveradatbázisa. További tudnivalókért lásd: [Az entitástár és a Power BI integrációjának áttekintése](power-bi-integration-entity-store.md). 

A következő fő összesítő mértékek szolgálnak a tartalom alapjaként.

| Entitás                  | Fő összesítő mérték | Adatforrás a Dynamics 365 szolgáltatáshoz      | Mező     | Leírás                                        |
|-------------------------|---------------------------|-----------------------------------|-----------|----------------------------------------------------|
| Költségkönyvelési tételek | SUM (összeg)               | CAMDATAAggregatedCostEntry        | Összeg    | Az összeg a Költségkönyvelési főkönyv pénznemében. |
| Statisztikai bejegyzések     | SUM(Nagyság)            | CAMDATAAggregatedStatisctialEntry | Nagyság |                                                    |

A következő táblázat azt mutatja, hogyan használjuk a fő összesített mértékeket számos számított mérték létrehozására a tartalom adathalmazában.

| Méret                                       | A mérőszám kiszámításának módja                                                                                          |
|-----------------------------------------------|------------------------------------------------------------------------------------------------------------------------|
| Tényleges költség                                   | CALCULATE('Költségkönyvelési tételek'\[Mérték\], 'Tranzakcióverziók'\[ISSOURCEVERSIONBUDGET\_VALUE\] = 0)            |
| Előirányzott költség                                   | CALCULATE('Költségkönyvelési tételek'\[Mérték\], 'Tranzakcióverziók'\[ISSOURCEVERSIONBUDGET\_VALUE\] = 1)            |
| Tervezett költség eltérése                          | \[Tervezett költség\] - \[Tényleges költség\]                                                                                      |
| Költségvetés eltérésének százaléka                    | IF(\[Tervezett költség\] = 0, blank(), \[Költségvetés eltérése\] / \[Tervezett költség\])                                                |
| Tényleges nagyság                              | CALCULATE('Statisztikai bejegyzések'\[FullMagnitude\], 'Tranzakcióverziók'\[ISSOURCEVERSIONBUDGET\_VALUE\] = 0)          |
| Költségvetés nagysága                              | CALCULATE(\[FullMagnitude\], 'Tranzakcióverziók'\[ISSOURCEVERSIONBUDGET\_VALUE\] = 1)                               |
| Statisztikai költségvetéseltérés                   | \[Tervezett nagyság\] - \[Tényleges nagyság\]                                                                            |
| Statisztikai költségvetéseltérés százaléka        | IF(\[Tervezett nagyság\] = 0, blank(), \[Statisztikai költségvetéseltérés\] / \[Tervezett nagyság\])                          |
| Tényleges költségszorzó                              | IF (\[Tényleges nagyság\] = 0, BLANK(), \[Tényleges költség\] / \[Tényleges nagyság\])                                          |
| Költségvetési költségszorzó                              | IF (\[Költségvetés nagysága\] = 0, BLANK(), \[Tervezett költség\] / \[Költségvetés nagysága\])                                          |
| Tervezett költségszorzó eltérése                     | \[Tervezett költségszorzó\] - \[Tényleges költségszorzó\]                                                                            |
| Tervezett költségszorzó százaléka          | IF(\[Tervezett költség\] = 0, blank(), \[Tervezett költségszorzó eltérése\] / \[Tervezett költségszorzó\])                                 |
| Fix tervezett költség                             | CALCULATE(\[Tervezett költség\], 'Költségkönyvelési tételek'\[COSTBEHAVIOR\] = 1)                                              |
| Változó tervezett költség                          | CALCULATE(\[Tervezett költség\], 'Költségkönyvelési tételek'\[COSTBEHAVIOR\] = 2)                                              |
| Fix változó tervezett költség                    | \[Fix tervezett költség\]                                                                                                  |
| Változó rugalmas tervezett költség                 | IF (\[Költségvetés nagysága\] = 0, BLANK(), (\[Változó tervezett költség\] / \[Költségvetés nagysága\]) \* \[Tényleges nagyság\])       |
| Rugalmas tervezett költség                          | \[Fix változó tervezett költség\] + \[Változó rugalmas tervezett költség\]                                                     |
| Rugalmas költségvetési eltérés                      | \[Rugalmas tervezett költség\] - \[Tényleges költség\]                                                                             |
| Rugalmas költségvetési eltérés százaléka           | IF(\[Rugalmas tervezett költség\] = 0, BLANK(), \[Rugalmas költségvetési eltérés\] / \[Rugalmas tervezett költség\])                     |
| Rugalmas tervezett költségszorzó                     | IF (\[Tényleges nagyság\] = 0, BLANK(), \[Rugalmas tervezett költség\] / \[Tényleges nagyság\])                                 |
| Rugalmas tervezett költségszorzó eltérése            | \[Rugalmas tervezett költségszorzó\] - \[Tényleges költségszorzó\]                                                                   |
| Rugalmas tervezett költségszorzó eltérési százaléka | IF(\[Rugalmas tervezett költségszorzó\] = 0, BLANK(), \[Rugalmas tervezett költségszorzó eltérése\] / \[Rugalmas tervezett költségszorzó\]) |

A következő fő dimenziók szolgálnak szűrőként az összesítő mértékek szeletelésére, nagyobb részletességet és mélyebb elemzési betekintések elérését téve lehetővé.

| Entitás                             | Példák attribútumokra                                                                                               |
|------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| Költségkönyvelési főkönyvek            | Költségkönyvelési főkönyv                                                                                               |
| Költség-ellenőrzőegységek                 | Költség-ellenőrzőegység neve                                                                                               |
| Költségösszetevő-dimenziók            | Költségösszetevő-dimenzió neve, Költségösszetevő-dimenziótag neve, Költségösszetevő-dimenziótag leírása          |
| Költségobjektum-dimenziók             | Költségösszetevő-dimenzió neve, Költségösszetevő-dimenziótag neve, Költségösszetevő-dimenziótag leírása              |
| Statisztikai dimenziók             | Statisztikai dimenzió neve, Statisztikai dimenziótag neve, Statisztikai dimenziótag leírása              |
| Költségobjektum dimenzióhierarchiái  | Költségobjektum dimenzióhierarchiájának neve, Költségobjektum dimenzióhierarchiájának szintje, Költségobjektum dimenzióhierarchiájának fája    |
| Költségösszetevő dimenzióhierarchiái | Költségelem dimenzióhierarchiájának neve, Költségelem dimenzióhierarchiájának szintje, Költségelem dimenzióhierarchiájának fája |
| Statisztikai dimenzióhierarchiák  | Statisztikai dimenzióhierarchiája neve, Statisztikai dimenzióhierarchiája szintje, Statisztikai dimenzióhierarchia fája    |
| Tranzakcióverziók               | Verzió neve                                                                                                         |
| Pénzügyi naptárak                   | Naptár, Naptár leírása                                                                                       |
| Pénzügyi évek                       | Naptári év                                                                                                        |
| Pénzügyi időszakok                     | Naptári év időszak                                                                                                 |
