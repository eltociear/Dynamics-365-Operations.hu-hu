---
title: Tervezési feladat érvénytelenítése
description: Ez a témakör azt mutatja be, hogyan lehet érvényteleníteni egy olyan aktív tervezési feladatot, amely a Tervezés optimalizálása funkciót használja.
author: ChristianRytt
manager: AnnBe
ms.date: 02/18/2020
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ReqCreatePlanWorkspace
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2019-10-31
ms.dyn365.ops.version: AX 10.0.5
ms.openlocfilehash: 18c5c7b8030fc6adbc548dab750e4f454aebc867
ms.sourcegitcommit: a688c864fc609e35072ad8fd2c01d71f6a5ee7b9
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/20/2020
ms.locfileid: "3076346"
---
# <a name="cancel-a-planning-job"></a>Tervezési feladat visszavonása

[!include [banner](../../includes/banner.md)]
[!include [banner](../../includes/preview-banner.md)]

A Microsoft Dynamics 365 Supply Chain Management rendszerben érvényteleníthetők az olyan aktív tervezési feladatok, amelyek a Tervezés optimalizálása funkciót használják. Ha a párbeszédpanelen a **Mégse** lehetőséget választja, amikor a tervezésoptimalizálási feladat közvetlenül a felhasználói felületről indul el, (nem a háttérben), akkor ez nem törli a tervezési optimalizációs feladatot. Még ha figyelmeztetés jelenik meg, mint a "művelet visszavonva", akkor is a következő lépések végrehajtásával kell megszüntetni egy tervezési feladatot a tervezési optimalizációval.


Aktív tervezési feladat érvénytelenítéséhez hajtsa végre az alábbi lépéseket. 

> [!NOTE]
> Csak egy aktív feladat érvényteleníthető.

1. Lépjen az **Alaptervezés \> Beállítás \> Tervek** részre.
2. Válassza ki a tervezés futtatásához megfelelő tervet.
3. Válassza az **Előzmények** lehetőséget.
4. Válassza ki az érvényteleníteni kívánt tervezési feladatot.
5. Válassza a **Mégse** lehetőséget.

A feladat állapota mindaddig **Megszakítás** lesz, amíg a Tervezés optimalizálása szolgáltatás meg nem erősíti, hogy a feladat érvénytelenítve lett. Ezt követően az állapot **Megszakítva** lesz.

> [!NOTE]
> Az állapot változásainak megjelenítéséhez a **Frissítés** gombra kattintva frissíteni kell az oldalt.

## <a name="additional-resources"></a>További erőforrások

[Tervezési optimalizálás áttekintése](planning-optimization-overview.md)

[Tervezési optimalizálás indítása](get-started.md)

[A tervezésoptimalizálása illeszkedési elemzése](planning-optimization-fit-analysis.md)

[Tervelőzmények és tervezési naplók megtekintése](plan-history-logs.md)

[Szűrők alkalmazása egy tervre](plan-filters.md)
