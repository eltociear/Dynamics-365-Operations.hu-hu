---
title: Tényleges viszonyítva a költségvetéshez Power BI tartalom
description: Ez a témakör a Tényleges viszonyítva a költségvetéshez Power BI-tartalmat ismerteti. Leírja, hogy hogyan kell hozzáférni a tartalomcsomagban szereplő jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához előzőleg használt entitásokkal és adatmodellekkel kapcsolatban.
author: ryansandness
manager: AnnBe
ms.date: 12/18/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BudgetTrackingWorkspace
audience: Application user, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: ryansand
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: July 2017 update
ms.openlocfilehash: a577ab24aaf86c1f7a22953e03f397a2e8213c78
ms.sourcegitcommit: 3ba95d50b8262fa0f43d4faad76adac4d05eb3ea
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 09/27/2019
ms.locfileid: "2184393"
---
# <a name="actual-vs-budget-power-bi-content"></a>Tényleges viszonyítva a költségvetéshez Power BI tartalom

[!include [banner](../includes/banner.md)]

Ez a témakör a **Tényleges viszonyítva a költségvetéshez** Microsoft Power BI-tartalmat ismerteti. Leírja, hogy hogyan kell hozzáférni a Power BI-jelentésekhez, és információkat nyújt a tartalomcsomag összeállításához előzőleg használt entitásokkal és adatmodellekkel kapcsolatban.

## <a name="overview"></a>Áttekintés

A **Tényleges viszonyítva a költségvetéshez** Power BI-tartalmat azoknak hoztuk létre, akik a valós és a költségvetési teljesítmény összevetéséért felelősek a szervezetnél. A **Tényleges viszonyítva a költségvetéshez** Power BI-tartalom a költségvetés-eltérésekbe nyújt betekintést. Az aktuális év költségvetését elemezheti számlakategória, költségvetési kód, fő számla, fő számla leírása vagy pénzügyi időszak szerint, hogy jobban megérthesse az esetleges eltérések okát.

## <a name="accessing-the-power-bi-content"></a>A Power BI tartalom elérése
A **Tényleges viszonyítva a költségvetéshez** Power BI-tartalom jelentései a **Főkönyvi költségvetések és előrejelzések** és a **Pénzügyi igazgató** munkaterületen jelennek meg.

## <a name="reports-that-are-included-in-the-power-bi-content"></a>Jelentések, amelyek a Power BI-tartalomban szerepelnek
A következő táblázat ismerteti a **Tényleges viszonyítva a költségvetéshez** Power BI-tartalom egyes jelentésoldalain található mutatókat.

| Jelentés                      | Mutatók                                                                             |
|-----------------------------|-------------------------------------------------------------------------------------|
| Költségek – Tényleges - költségvetés | <ul><li>Az idei teljes kiadás</li><li>Költségvetés szerinti idei teljes kiadás</li></ul>  |
| Bevétel - Tényleges és költségvetés  | <ul><li>Az idei teljes bevétel</li><li>Költségvetés szerinti idei teljes bevétel</li><ul>     |
| Kiadás                     | <ul><li>Az idei teljes kiadás</li><li>Költségcél a költségvetési alapján</li><ul> |
| Bevétel                     | <ul><li>Az idei teljes bevétel</li><li>Bevételi cél a költségvetési alapján</li><ul>   |
| Nettó árbevétel                  | <ul><li>Az idei nettó bevétel</li><li>Nettó bevételi cél a költségvetési alapján</li><ul>   |

## <a name="understanding-the-data-model-and-entities"></a>Adatmodell, illetve entitások ismertetése

| Entitás                    | Tartalom                                                                         |
|---------------------------|----------------------------------------------------------------------------------|
| Főkönyvi tevékenységek | Tranzakciós összegek a főkönyvbe                                       |
| Költségvetési tevékenységek         | Tranzakciós összegek a költségvetési jegyzékbe                                      |
| Fő számlák             | Fő számlák a jelentések szűréséhez                                               |
| Pénzügyi naptárak          | Pénzügyi naptárak a jelentések szűréséhez                                            |
| Főkönyvek                   | A jelenlegi főkönyvi jelentés szűréséhez használható főkönyvek              |
| Költségvetési kódok              | Költségvetési kódok a jelentések szűréséhez                                                |
| Jogi személyek            | A jelenlegi jogi személyre vonatkozó jelentés szűréséhez használható jogi személyek |
