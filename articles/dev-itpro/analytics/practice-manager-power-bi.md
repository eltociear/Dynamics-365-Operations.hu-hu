---
title: "Gyakorlatvezető Power BI tartalom"
description: "Ez a témakör azt ismerteti, mit tartalmaz a Gyakorlatvezető Power BI-tartalom modul. Leírja, hogy hogyan kell hozzáférni a tartalomban szereplő jelentésekhez, és információkat nyújt a tartalom összeállításához használt entitásokkal és adatmodellekkel kapcsolatban."
author: KimANelson
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations, UnifiedOperations
ms.assetid: 
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 99e5b5087cc72c01ff3e92d0b2b3a6279385eb19
ms.contentlocale: hu-hu
ms.lasthandoff: 09/29/2017

---

# <a name="practice-manager-power-bi-content"></a>Gyakorlatvezető Power BI tartalom

[!include[banner](../includes/banner.md)]

Ez a témakör azt ismerteti, mit tartalmaz a **Gyakorlatvezető** Microsoft Power BI-tartalom modul. Leírja, hogy hogyan kell hozzáférni Power BI-jelentésekhez, és információkat nyújt a tartalom összeállításához használt entitásokkal és adatmodellekkel kapcsolatban.

## <a name="overview"></a>Áttekintés

A **Gyakorlatvezető** Power BI-tartalom gyakorlatvezetők és projektvezetők számára készült. Olyan fontos mutatókat biztosít, amelyek a szervezetnél futó projektekkel kapcsolatosak. Az irányítópult áttekintést nyújt a projektekről és a kapcsolódó ügyfelekről. A jelentésszintű szűrők segítségével jelentés készíthető a meghatározott jogi személyekhez. Ez a Power BI-tartalom adatokat kér le a projektkönyvelés összetett méréseitől.

A **Gyakorlatvezető** Power BI-tartalom öt jelentésoldalt tartalmaz: egy áttekintő oldalt és négy olyan oldalt, amely a projekt költségeinek, bevételeinek, jelenérték-kezelésének és órainak mutatóira vonatkozó részleteket tartalmaz, amelyek különböző dimenziók szerint vannak lebontva.

A tartalom minden összege a rendszer pénznemében jelenik meg. Beállíthatja az rendszer alapértelmezett pénznemét a **Rendszerparaméterek** oldalon.

## <a name="accessing-the-power-bi-content"></a>Power BI-tartalom elérése
Amennyiben a Microsoft Dynamics 365 for Finance and Operations Enterprise edition (2017. július) rendszert használja, a **Gyakorlatvezető** Power BI-tartalom a **Projektvezetés** munkaterületen jelenik meg.

## <a name="reports-that-are-included-in-the-power-bi-content"></a>A Power BI-tartalomhoz tartozó jelentések

A következő táblázat ismerteti a **Gyakorlatvezető** Power BI-tartalom egyes jelentésoldalain található mutatókat.

| Jelentéslap       | Mutatók |
|-------------------|---------|
| Projektek áttekintése | <ul><li>Létrehozott projektek</li><li>Becsült projektek</li><li>Folyamatban lévő projektek</li><li>Projektek száma szakasz szerint</li><li>Projektek száma város szerint</li><li>Tényleges bevétel vevő szerint</li><li>Költségvetés – bruttó nyereség projekt szerint</li><li>Jelenérték-kezelés áttekintése</li></ul> |
| Költség              | <ul><li>Tényleges és költségvetési költség havonta</li><li>Tényleges és költségvetési költség évente</li><li>Tényleges és költségvetési költség kategóriánként</li><li>Tényleges költség tranzakciótípus szerint</li></ul> |
| Bevétel           | <ul><li>Tényleges bevétel hónap szerint</li><li>Tényleges bevétel irányítószám szerint</li><li>Tényleges és költségvetési bevétel kategória szerint</li><li>Tényleges bevétel vevői iparág szerint</li></ul> |
| EVM               | Költség- és ütemezésteljesítmény-index projekt szerint |
| óra             | <ul><li>Tényleges számlázható hasznos órák és tényleges számlázható haszontalan órák és költségvetési órák</li><li>Tényleges számlázható hasznos órák és tényleges számlázható haszontalan órák projekt szerint</li><li>Tényleges számlázható hasznos órák és tényleges számlázható haszontalan órák erőforrás szerint</li><li>Tényleges számlázható órák aránya projekt szerint.</li><li>Tényleges számlázható órák aránya erőforrás szerint.</li></ul> |

Az összes ilyen jelentésben szereplő diagramot és a lapot ki lehet szűrni és rögzíteni lehet az irányítópulton. A szűréssel és a Power BI-n történő rögzítéssel kapcsolatos információkért lépjen az [Irányírópult létrehozása és konfigurálása](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-4-2-create-configure-dashboards/) lehetőségre. Használhatja a Mögöttes adatok exportálása funkciót is azoknak a mögöttes adatoknak az exportálásához, amelyeknek összegzése egy ábrán látható.

## <a name="extending-the-power-bi-content"></a>Power BI-tartalom kibővítése
A Microsoft Dynamics Lifecycle Services (LCS) szolgáltatásban található tartalomcsomagok révén nagyszerű elemzési lehetőségeket nyújthat azoknak a személyeknek, akik nem jelentkeztek be a Microsoft Dynamics 365 szolgáltatásba. A tartalmi csomagokat módosíthatja, hogy más jelentéseket vagy megjelenítéseket tartalmazzanak, majd közzéteheti őket elemzés céljából a Power BI.com bérlőn. 

A **Gyakorlatvezető** Power BI-tartalmat az LCS Megosztott eszközök könyvtárában találja. A tartalom letöltésére és szervezeténél való megvalósítására vonatkozó további információért lásd: [Power BI-tartalom az LCS megoldásban a Microsofttól és a partnerektől](power-bi-content-microsoft-partners.md). Ha meg szeretne tekinteni egy demót, amely bemutatja a Power BI-tartalmak megvalósítását, lásd a [Power BI-tartalom a Microsofttól és az Ön partnereitől a Dynamics Lifecycle Services szolgáltatásban](https://mix.office.com/watch/9puyb1b2xs1w) című részt (Office Mix).

Ügyeljen arra, hogy azt a **Gyakorlatvezető** tartalmat töltse le, amely a Dynamics 365 ön által használt verziójára vonatkozik.

## <a name="understanding-the-data-model-and-entities"></a>Adatmodell, illetve entitások ismertetése

A **Gyakorlatvezető** Power BI-tartalom jelentési oldalainak feltöltésére a következő adatok szolgálnak. Ezeket az adatokat az Entitástárban lebonyolított összesített mérések jelenítik meg. Az entitástár a Microsoft analitikai célokra optimalizált SQL-szerveradatbázisa. További tudnivalókért lásd: [Az entitástár és a Power BI integrációjának áttekintése](power-bi-integration-entity-store.md).

A következő szakaszok leírják az egyes entitások által használt összesített mértékeket.

### <a name="entity-projectaccountingcubeactualhourutilization"></a>Entitás: ProjectAccountingCube_ActualHourUtilization
**Adatforrás:** ProjEmplTrans

| Fő összesítő mérték      | Mező                              | Leírás | 
|--------------------------------|------------------------------------|-------------|
| Tényleges számlázható hasznos órák száma | Sum(ActualUtilizationBillableRate) | A ténylegesen számlázható felhasznált órák száma. |
| Tényleges számlázható haszontalan idő   | Sum(ActualBurdenBillableRate)      | Összes tényleges haszontalan idő aránya. |

### <a name="entity-projectaccountingcubeactuals"></a>Entitás: ProjectAccountingCube_Actuals
**Adatforrás:** ProjTransPosting

| Fő összesítő mérték | Mező              | Leírás | 
|---------------------------|--------------------|-------------|
| Tényleges bevétel            | Sum(ActualRevenue) | Az összes tranzakció összes feladott bevétele. |   
| Tényleges költség               | Sum(ActualCost)    | Az összes tranzakciótípus összes feladott költsége. |

### <a name="entity-projectaccountingcubecustomer"></a>Entitás: ProjectAccountingCube_Customer
**Adatforrás:** CustTable

| Fő összesítő mérték | Mező                                            | Leírás | 
|---------------------------|--------------------------------------------------|-------------|
| Projektek száma        | COUNTA(ProjectAccountingCube_Projects[PROJECTS]) | Elérhető projektek száma. |


### <a name="entity-projectaccountingcubeforecasts"></a>Entitás: ProjectAccountingCube_Forecasts
**Adatforrás:** ProjTransBudget

| Fő összesítő mérték | Mező                  | Leírás | 
|---------------------------|------------------------|-------------|
| Előirányzott költség               | Sum(BudgetCost)        | Az összes tranzakciótípus összes előrejelzett költsége. |
| Tényleges bevétel            | Sum(BudgetRevenue)     | A megvalósult/számlázott bevétel előrejelzett összege.  |
| Előirányzott bruttó nyereség       | Sum(BudgetGrossMargin) | Különbség az összes előrejelzett bevétel összege és az összes előrejelzett költség összege között. |

### <a name="entity-projectaccountingcubeprojectplancostsview"></a>Entitás: ProjectAccountingCube_ProjectPlanCostsView
**Adatforrás:** Projekt

| Fő összesítő mérték | Mező                    | Leírás | 
|---------------------------|--------------------------|-------------|
| Tervezett költség              | Sum(SumOfTotalCostPrice) | Tervezett feladatokkal rendelkező projekttranzakció-típus becsléseinek teljes önköltségi ára. |

### <a name="entity-projectaccountingcubeprojects"></a>Entitás: ProjectAccountingCube_Projects
**Adatforrás:** Projekt

| Fő összesítő mérték    | Mező | Leírás | 
|------------------------------|-------|-------------|
| Költségteljesítmény-index       | ProjectAccountingCube_Projects[Earned value] / ProjectAccountingCube_Projects[A végrehajtott feladatok összes tényleges költsége] | Az összes bevétel osztva az összes tényleges költséggel. |
| Teljesítményindex ütemezése   | ProjectAccountingCube_Projects[Earned value] / ProjectAccountingCube_Projects[A végrehajtott feladatok összes tervezett költsége] | Az összes bevétel osztva az összes tervezett költséggel. |
| A már befejezett munka százaléka. | Befejezett munka százaléka = ProjectAccountingCube_Projects[A végrehajtott feladatok összes tényleges költsége] / (ProjectAccountingCube_Projects[A végrehajtott feladatok összes tényleges költsége] + ProjectAccountingCube_Projects[Projekt összes tervezett költsége] - ProjectAccountingCube_Projects[A végrehajtott feladatok összes tervezett költsége]) | A végrehajtott munka összesített százaléka a végrehajtott feladat tényleges költsége és a projekt tervezett költsége alapján. |
| Tényleges számlázható órák aránya  | ProjectAccountingCube_Projects[Projekt összes ténylegesen számlázható hasznos ideje] / (ProjectAccountingCube_Projects[Projekt összes ténylegesen számlázható hasznos ideje] + ProjectAccountingCube_Projects[Projekt összes ténylegesen számlázható haszontalan ideje]) | Tényleges számlázható órák összesen a hasznos órák és a haszontalan idő alapján. |
| Jelenérték                 | ProjectAccountingCube_Projects[Projekt összes tervezett költsége] * ProjectAccountingCube_Projects[A már befejezett munka százaléka] | Összes tervezett költség szorozva a végrehajtott munka százalékával. |

### <a name="entity-projectaccountingcubetotalestimatedcosts"></a>Entitás: ProjectAccountingCube_TotalEstimatedCosts 
**Adatforrás:** ProjTable

| Fő összesítő mérték       | Mező               | Leírás | 
|---------------------------------|---------------------|-------------|
| Befejeződött tevékenység tervezett költsége | Sum(TotalCostPrice) | Befejeződött feladatokkal rendelkező projekttranzakció-típus becsléseinek teljes önköltségi ára. |
