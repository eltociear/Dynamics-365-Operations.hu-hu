---
title: Értékesítési rendelések megerősítése
description: Ez az eljárás bemutatja, hogyan kell az értékesítési rendeléseket megerősíteni.
author: omulvad
manager: AnnBe
ms.date: 06/26/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SalesTableListPage, SalesTable, SalesEditLines,  SrsReportViewerForm, CustConfirmJournal, SysQueryForm, SysQueryFieldLookUp, SysLookup, SalesParmIdLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: f9274a90ffbf6e5703d3ed97a8b974227b25c2a0
ms.sourcegitcommit: 62d66f98d4bbf916e19184506b90055bb68d219f
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/28/2019
ms.locfileid: "1924378"
---
# <a name="confirm-sales-orders"></a>Értékesítési rendelések megerősítése

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan kell az értékesítési rendeléseket megerősíteni. Megjelenik, hogyan lehet megerősíteni egyetlen rendelést, illetve egyszerre több rendelést. Ezeket a feladatokat jellemzően egy értékesítési rendelés feldolgozó végzi el. Ezt a folyamatot az USMF bemutatócéggel vagy saját adataival is használhatja. Mielőtt elkezdené, ellenőrizze, hogy van-e ugyanannak a vevőnek több nyitott értékesítési rendelése. Ha USMF-et használ, használhatja az US-027 vevőt.


## <a name="confirm-a-single-sales-order"></a>Egy értékesítési rendelés megerősítése
1. Ugorjon az **Navigációs lap > Modulok > Értékesítés és marketing > Értékesítési rendelések > Minden értékesítési rendelés** pontra.
2. A listában keresse meg és válassza ki a jóváhagyni kívánt rendelést.
3. Kattintson a hivatkozásra az értékesítési rendelés számán a kiválasztott rendelés megnyitásához.
4. A **Művelet panelen** kattintson az **Értékesítés** elemre.
5. Kattintson az **Értékesítési rendelés** megerősítése gombra.
6. Bontsa ki a **Paraméterek** szakaszt. Ellenőrizze, hogy a **Feladás** értéke „Igen” értékre van-e állítva.  
7. Állítsa a **Nyomtatás megerősítése** pontot „Igen” értékre. A **Hitelkeret ellenőrzése** mező megadja a vevő fennmaradó hitelkeretének kiszámításához használt módszert. Alapértelmezésben ez a Kinnlevőségek paraméterei oldalról van átmásolva. Ha szeretné kihagyni a hitelkeret-ellenőrzést egy adott értékesítési rendelés megerősítésekor, állítsa „Nincs” értékre a **Hitelkeret-ellenőrzés** elemet. Azonban tartsa szem előtt, hogy még akkor is, ha ez a mező beállítása „Nincs”, a hitelkeret-ellenőrzés akkor is megtörténik, ha a **Kötelező hitelkeret-korlát** beállítást kiválasztotta a vevői alapadatokban. 
8. Kattintson az **OK** gombra.
9. Kattintson az **Igen** gombra.
10. Zárja be a lapot.
11. A **Művelet** ablaktáblában kattintson a **Beállítások** elemre.
12. Kattintson a **Nézetváltás** elemre.
13. Kattintson a **Fejlécnézet** gombra. Ha egy rendelést megerősít, a **Dokumentumállapot** „Visszaigazolás” értékű lesz. 
14. A **Művelet panelen** kattintson az **Értékesítés** elemre.
15. Kattintson az **Értékesítési rendelés** visszaigazolására.
16. Zárja be a lapot.

## <a name="confirm-multiple-sales-orders-at-once"></a>Több értékesítési rendelés egyszerre történő megerősítése
1. Ugorjon az **Értékesítés és marketing > Értékesítési rendelések > Értékesítés megerősítése > Értékesítési rendelés-visszaigazolás** elemre.
2. Kattintson a **Kiválasztás** lehetőségre.
3. A **Tartomány** lap listáján keresse meg és válassza ki a rekordot, amely a **Vevőfiók** mezőre hivatkozik.
4. A **Kritériumok** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
5. A listában keresse meg és válassza ki a vevőfiókot, amelyben a tömegesen jóváhagyandó több rendelés található. Az USMF használata esetén választhatja az „US-027” számlát.  
6. Kattintson az **OK** gombra.
    - Az **Áttekintés** lapon a lekérdezési feltételeknek megfelelő rendelések listája jelenik meg. Ezek a visszaigazolásban fognak szerepelni.  
    - Az **Összegző frissítés** mező a **Paraméterek** szakaszban meghatározza azt a paramétert, amellyel több rendelés összegzése történik egy visszaigazoló dokumentumba. Alapértelmezés szerint az opció a **Kinnlevőségek paraméterei** oldal **Összesítő frissítés beállítás alapértékeiből** lesz átmásolva.  
7. Az **Összegzés frissítése a következőhöz** mezőben válassza ki a Rendelés elemet. Az összesítő frissítések létrehozásához szükséges minimális paraméterek a **Számlafiók** és a **Pénznem**. Ez azt jelenti, hogy olyan összesítő frissítések nem megengedettek, amelyeknek eltérő a számlafiókjuk és a pénznemük. Az **Összesítő frissítések paramétereinek** oldalán beállíthatók további paraméterek is, amely a **Kinnlevőségek paraméterei** oldalról érhető el. 
8. Az **Értékesítési rendelés** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
9. A listában válassza ki a rendelésszámot, amely az összesítő rendelés lesz.
10. Kattintson az **Elrendezés** elemre.
11. Kattintson az **OK** gombra.
12. Kattintson az **OK** gombra.

