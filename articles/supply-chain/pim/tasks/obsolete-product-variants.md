---
title: Elavult termékváltozatok keresése
description: Ez az eljárás bemutatja, hogyan lehet megkeresni az elavult kiadott termékeket vagy termékváltozatokat, és hogyan lehet termékéletciklus-állapotot társítani az elavult termékekhez.
author: cvocph
manager: AnnBe
ms.date: 12/05/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: conradv
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4641d24cfa24722f5411da8943bfe4095a9546a4
ms.sourcegitcommit: 9d4c7edd0ae2053c37c7d81cdd180b16bf3a9d3b
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 05/15/2019
ms.locfileid: "1567630"
---
# <a name="find-obsolete-product-variants"></a>Elavult termékváltozatok keresése 

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan lehet megkeresni az elavult kiadott termékeket vagy termékváltozatokat, és hogyan lehet termékéletciklus-állapotot társítani az elavult termékekhez. Előfeltétel: Meg kell határozni legalább egy, tervezéshez inaktív termékéletciklus-állapotot a jelen feladat-útmutató lejátszásához.


## <a name="run-a-simulation"></a>Szimuláció futtatása
1. Ugorjon a Termékinformációk kezelése > Időszakos feladatok > Elavult termékek életciklus-állapotának módosítása lehetőségre.
2. Az Új termékéletciklus-állapot mezőben adjon meg vagy válasszon ki egy értéket.
3. A Szimuláció futtatása termékadatok frissítése nélkül mezőben válassza az Igen lehetőséget.
4. Az Ennyi napon belül létrehozott termékek kizárása mezőbe írjon be egy számot.
5. A Tranzakciókban használt termékek kizárása (napokban megadva) mezőbe írjon be egy számot.
6. Bontsa ki a Szerepeltetni kívánt rekordok szakaszt.
7. Kattintson a Szűrő parancsra.
8. A listában jelölje meg a kiválasztott sort.
9. Érték beírása a Feltétel mezőbe.
10. Kattintson az OK gombra.
11. Kattintson az OK gombra.

> [!NOTE]
> Ajánlott a kötegelt szimuláció futtatása, ha jelentős számú termékekre keres. Ezenkívül győződjön meg arról, hogy a szimulációt ne a vállalat a leginkább aktív munkaidejében futtassa.  

## <a name="review-the-simulation-results"></a>A szimuláció eredményeinek áttekintése
1. Ugorjon a Termékinformációk kezelése > Lekérdezések és jelentések > Termékéletciklus-állapot karbantartási előzményei lehetőségre.
   
> [!NOTE]
> Ezen az oldalon áttekintheti a szimulációs eredményeket, és kiértékelheti, hogy hány termékhez és termékváltozathoz lesz új termékéletciklus-állapot társítva, ha a frissítést szimuláció nélkül futtatjuk.  

## <a name="run-the-update-of-the-product-lifecycle-state-for-obsolete-products"></a>Futtassa az Elavult termékek életciklus-állapota frissítését
1. Zárja be a lapot.
2. Ugorjon a Termékinformációk kezelése > Időszakos feladatok > Elavult termékek életciklus-állapotának módosítása lehetőségre.
3. Bontsa ki a Szerepeltetni kívánt rekordok szakaszt.

> [!NOTE]
> Vegye figyelembe, hogy az utolsó kijelölés mentése megtörtént.  

4. A Szimuláció futtatása termékadatok frissítése nélkül mezőben válassza a Nem lehetőséget.
5. Bontsa ki a Futtatás a háttérben szakaszt.

> [!NOTE]
> Attól függően, hogy hány termék és termékváltozat érintett, fontolja meg a feladat kötegben történő futtatását. Győződjön meg arról, hogy ne futtasson nagy frissítési feladatokat a vállalat leginkább aktív munkaidejében.  

6. Kattintson az OK gombra.
7. Ugorjon a Termékinformációk kezelése > Lekérdezések és jelentések > Termékéletciklus-állapot karbantartási előzményei lehetőségre.

> [!NOTE]
> Tekintse át a módosított kiadott termékeket és termékváltozatokat.  

8. Keresse meg és jelölje ki a kívánt rekordot a listán.

