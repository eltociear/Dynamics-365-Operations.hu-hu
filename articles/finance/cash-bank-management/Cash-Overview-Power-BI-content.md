---
title: Készpénzáttekintés Power BI tartalom
description: Ez a témakör a Készpénzáttekintés Power BI-tartalmat ismerteti. Leírja, hogy hogyan kell hozzáférni a tartalomcsomagban szereplő jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához előzőleg használt entitásokkal és adatmodellekkel kapcsolatban.
author: saraschi2
manager: AnnBe
ms.date: 06/25/2019
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankTreasurerWorkspace
audience: Application User
ms.reviewer: roschlom
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: 7621ca961288af81966e0ac883c6525f89960654
ms.sourcegitcommit: bbb64b3475eef155b3f9d1bdc440545da8a7182f
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2553140"
---
# <a name="cash-overview-power-bi-content"></a>Készpénzáttekintés Power BI tartalom

[!include [banner](../includes/banner.md)]

Ez a témakör a **Készpénzáttekintés** Microsoft Power BI-tartalmat ismerteti. Leírja, hogy hogyan kell hozzáférni a tartalomcsomagban szereplő jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához előzőleg használt entitásokkal és adatmodellekkel kapcsolatban.

## <a name="overview"></a>Áttekintés

A **Készpénzáttekintés** Power BI-tartalom azon személyeknek szól, akik a szervezetük készpénzéért felelősek. A **Készpénzáttekintés** Power BI-tartalom áttekintést nyújt a pénzforgalmáról. Emellett előrejelzéseket kínál, melyek segíthetnek, hogy jobb döntéseket hozzon, és ezáltal javíthassa a pénzforgalom állapotát. A készpénzt jogi személy, pénznem és bankszámla szerint elemezheti, hogy jobban megértse a többleteket és hiányokat.

## <a name="setup-needed-to-view-power-bi-content"></a>A Power BI-tartalom megtekintéséhez beállítás szükséges

A következő beállításokat el kell végezni ahhoz, hogy az adatok megjelenjenek a **Készpénz-áttekintés** és **Banki menedzsment** Power BI megjelenítésekben.

1. Nyissa meg a **Rendszeradminisztráció > Beállítás > Rendszerparaméterek** pontot a **Rendszerpénznem** és a **Rendszerváltási árfolyam** beállításához.
2. Ugrás a **Főkönyv > Beállítás > Főkönyv** részre a **Könyvelési pénznem** és az **Árfolyamtípus** beállításához.
2. Adja meg az árfolyamokat a tranzakció pénznemei és a könyvelési pénznem, a könyvelési pénznem és a rendszer pénzneme, a könyvelési pénznem és a banki pénznemek között. Lépjen ide: **Főkönyv > Pénznemek > Pénznemek árfolyamtípusai**.
3. Pénzforgalmi előrejelzés konfigurálása és futtatása. A Pénzforgalmi előrejelzés beállításával kapcsolatos további tudnivalókat lásd: [Pénzforgalmi előrejelzés](https://docs.microsoft.com/dynamics365/finance/cash-bank-management/cash-flow-forecasting). 
4. Lépjen a **Rendszerfelügyelet > Beállítás > Entitástár** részre a **LedgerCovLiquidityMeasurement** összesítő mérték frissítéséhez.

## <a name="accessing-the-power-bi-content"></a>A Power BI tartalom elérése

A **Készpénzáttekintés** Power BI-tartalom jelentései a **Készpénzáttekintés** és a **Bankszámla kezelése** munkaterületen jelennek meg.

Ha adatokkal együtt szeretné megtekinteni a pénzforgalmi előrejelzések jelentéseit, akkor először futtatnia kell az előrejelzés számítási folyamatát a Készpénz- és bankkezelés terület **Pénzforgalmi előrejelzések kiszámítása** funkciójánál. Ezt végre kell hajtani az előrejelzésben szereplő mindegyik vállalat esetén.  Ezt követően frissítenie kell a LedgerCovLiquidityMeasurement összesített mértéket az **Entitástár** oldalon.  

Bemutató céllal felvehet pénzforgalom-előrejelzési bemutató adatokat a Demóadatok modul **Adatok generálása** oldaláról.  Ez a szkript adatokat szúr be a pénzforgalmi előrejelzés táblázataiba annak érdekében, hogy gyorsan kitöltse azokat a jelentések számára szükséges adatokkal.  Ez a modul csak akkor érhető el, ha a bemutató adatmodellt telepítették a környezetnél. 

## <a name="reports-that-are-included-in-the-power-bi-content"></a>Jelentések, amelyek a Power BI-tartalomban szerepelnek

A következő táblázat ismerteti a **Készpénzáttekintés** Power BI-tartalom egyes jelentésoldalain található mutatókat.

| Jelentés                                | Tartalom |
|---------------------------------------|----------|
| Készpénzáttekintés – minden vállalat         | <ul><li>Pénzbeáramlások és pénzkiáramlások a rendszer pénznemében</li><li>Előre jelzett pénznemegyenlegek</li><li>Összesített egyenleg a rendszer pénznemében</li><li>Egyenleg jogi személy szerint</li><li>Aznapi tényleges és előrejelzett egyenleg a bankszámla pénznemében</li></ul> |
| Készpénzáttekintés – jelenlegi vállalat       | <ul><li>Pénzbeáramlások és pénzkiáramlások a könyvelési pénznemben</li><li>Előre jelzett pénznemegyenlegek</li><li>Összesített egyenleg a könyvelési pénznemben</li><li>Aznapi tényleges és előrejelzett egyenleg a bankszámla pénznemében</li></ul> |
| Pénzforgalmi előrejelzés – összes vállalat    | <ul><li>Pénzbeáramlások és pénzkiáramlások a rendszer pénznemében</li><li>Napi előrejelzés összegzése</li><li>Előrejelzés részletei</li></ul> |
| Pénzforgalmi előrejelzés – pénznem vállalata | <ul><li>Pénzbeáramlások és pénzkiáramlások a könyvelési pénznemben</li><li>Napi előrejelzés összegzése</li><li>Előrejelzés részletei</li></ul> |
| Pénznem előrejelzése                     | <ul><li>Előre jelzett pénznemegyenlegek</li><li>Napi pénznem összegzése</li><li>Előrejelzés részletei</li></ul> |
| Banki egyenlegek                         | <ul><li>Összesített egyenleg a rendszer pénznemében</li><li>Egyenleg jogi személy szerint</li><li>Aznapi tényleges és előrejelzett egyenleg a bankszámla pénznemében</li><li>Egyenleg bankszámla szerint</li><li>Egyenleg pénznemenként</li></ul> |


## <a name="understanding-the-data-model-and-entities"></a>Adatmodell, illetve entitások ismertetése

A következő táblázat megjeleníti azokat az entitásokat, amelyeken a **Készpénzáttekintés** Power BI-tartalom alapul.

| Entitás                                                                          | Tartalom |
|---------------------------------------------------------------------------------|----------|
| LedgerCovLiquidityMeasurement\_Vállalat                                          | Vállalatok a jelentések szűréséhez |
| LedgerCovLiquidityMeasurement\_Dátum                                             | Dátumok a jelentések szűréséhez |
| LedgerCovLiquidityMeasurement\_LedgerCovForecastActual                          | Jelenlegi banki egyenleg és az utolsó előre jelzett banki egyenleg |
| LedgerCovLiquidityMeasurement\_LedgerCovLiquidity                               | Előrejelzett tranzakció részletes adatai |
| LedgerCovLiquidityMeasurement\_LedgerCovLiquidityInflowOutflowBalanceCompany    | Összegzett pénzbevételek, kiadások és egyenlegek az egyes vállalatok könyvelési pénznemében |
| LedgerCovLiquidityMeasurement\_LedgerCovLiquidityInflowOutflowBalanceEnterprise | Összegzett pénzbevételek, kiadások és egyenlegek az összes vállalatnál a rendszer pénznemében |
| LedgerCovLiquidityMeasurement\_LedgerCovLiquidityTransactionCurrency            | Összegzett nettó tranzakciós összeg és devizaegyenleg a tranzakciós pénznem használatával |
