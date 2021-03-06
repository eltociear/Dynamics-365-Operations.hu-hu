---
title: Munkaidősablonok készítése
description: A munkaidősablonok határozzák meg az egész hét munkaóráit, és ezek segítségével hozhatók létre munkaidők egy adott időszakra.
author: sorenva
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: OpResLifeCycleManagementWorkspace, WorkTimeTable, WorkTimeCopyDayDialog
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: sorenand
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c82126d64954f8691571b80ab97b198d58a9e2cb
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1837710"
---
# <a name="create-working-time-templates"></a>Munkaidősablonok készítése

[!include [task guide banner](../../includes/task-guide-banner.md)]

A munkaidősablonok határozzák meg az egész hét munkaóráit, és ezek segítségével hozhatók létre munkaidők egy adott időszakra. Ez az eljárás bemutatja, hogyan definiálhat munkaidősablonokat a munkaidő-ütemezési tulajdonságok segítségével a munkaidő-intervallumok kategorizálásához. Ezt a folyamatot az USMF bemutatócégen vagy saját adata használatával is elvégezheti.

1. Ugrás az összes munkaterületek > Erőforrás életciklusa kezelése elemre.
2. Kattintson a Munkaidősablonok lehetőségre.

## <a name="create-working-time-template"></a>Munkaidősablon létrehozása
1. Kattintson az Új lehetőségre.
2. Írjon be egy értéket a Munkidősablon mezőbe.
3. Írjon be egy értéket a Név mezőbe.
4. Bontsa ki a Hétfő szakaszt.
5. Kattintson a Hozzáadás gombra.
6. Az Kezdés mezőben adjon meg egy időpontot.
    * Adja meg az időt, amikor a munka reggel elkezdődik.  
7. A Befejezés mezőben adjon meg egy időpontot.
    * Adja meg a dolgozók ebédszünetének időpontját.  
8. Kattintson a Hozzáadás gombra.
9. Az Kezdés mezőben adjon meg egy időpontot.
    * Adja meg, hogy mikor folytatódik a munka ebéd után.  
10. A Befejezés mezőben adjon meg egy időpontot.
    * A munkanap végének meghatározása.  

## <a name="replicate-working-times-to-all-week-days"></a>Munkaidők átmásolása minden hétköznapra
1. Kattintson a Nap másolása elemre.
    * Másolja át a munkaidők definícióit hétfőről keddre.  
2. Kattintson az OK gombra.
3. Kattintson a Nap másolása elemre.
    * Másolja át a munkaidők definícióit hétfőről szerdára.  
4. Válasszon egy lehetőséget a Befejező hétköznap mezőben.
5. Kattintson az OK gombra.
6. Kattintson a Nap másolása elemre.
    * Másolja át a munkaidők definícióit hétfőről csütörtökre.  
7. Válasszon egy lehetőséget a Befejező hétköznap mezőben.
8. Kattintson az OK gombra.
9. Kattintson a Nap másolása elemre.
    * Másolja át a munkaidők definícióit hétfőről péntekre.  
10. Válasszon egy lehetőséget a Befejező hétköznap mezőben.
11. Kattintson az OK gombra.

## <a name="define-time-slots-for-special-operations"></a>Időközök meghatározása speciális műveletekhez
1. Bontsa ki a Péntek szakaszt.
2. Keresse meg és jelölje ki a kívánt rekordot a listán.
3. A Tulajdonság mezőben adjon meg vagy válasszon ki egy értéket.
4. Keresse meg és jelölje ki a kívánt rekordot a listán.
5. A Tulajdonság mezőben adjon meg vagy válasszon ki egy értéket.

## <a name="mark-weekend-days-as-closed-for-pickup"></a>Hétvégek megjelölése zárt felvételhez
1. Bontsa ki a Szombat szakaszt.
2. A Lezárt felvétel mezőben válassza az Igen lehetőséget.
3. Bontsa ki a Vasárnap szakaszt.
4. A Lezárt felvétel mezőben válassza az Igen lehetőséget.

