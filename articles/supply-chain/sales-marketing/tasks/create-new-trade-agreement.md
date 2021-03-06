---
title: Új kereskedelmi szerződés létrehozása
description: Ez az eljárás bemutatja, hogyan hozhat létre egy kereskedelmi megállapodást, amelyben regisztrálhat egy új termékeladási árat, amelyben egy adott vevővel megállapodott.
author: omulvad
manager: AnnBe
ms.date: 06/25/2019
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 58ad2a5571138f1a82b021af63cdae9d567b92d8
ms.sourcegitcommit: 8b4b6a9226d4e5f66498ab2a5b4160e26dd112af
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 08/01/2019
ms.locfileid: "1835587"
---
# <a name="create-a-new-trade-agreement"></a>Új kereskedelmi szerződés létrehozása

[!include [task guide banner](../../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogyan hozhat létre egy kereskedelmi megállapodást, amelyben regisztrálhat egy új termékeladási árat, amelyben egy adott vevővel megállapodott. Ezt a folyamatot az USMF bemutatócéggel vagy saját adataival is futtathatja. Saját adatok használatakor az útmutató használatának megkezdése előtt győződjön meg róla, hogy a Kereskedelmi megállapodások napló neve létezik, ahol az Alapértelmezett viszony az "Ár (eladási)".


## <a name="create-and-post-a-new-trade-agreement-journal"></a>Hozzon létre és tegyen közzé egy új kereskedelmi megállapodási naplót
1. Ugorjon a **Navigációs lap > Modulok >Értékesítés és marketing > Árak és engedmények > Kereskedelmi megállapodási naplók** elemre.
2. Kattintson az **Új** elemre.
3. A **Név** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
4. Keresse meg és jelölje ki a kívánt rekordot a listán.
5. A **Művelet panelen** kattintson a **Sorok** elemre.
6. A **Fiókkód** mezőben válassza ki a „Tábla” lehetőséget.
    
    Ebben a példában egy konkrét vevő árát frissíti, ami azt jelenti, hogy meg kell adnia egy Táblát. Ha a termék listaárát frissítené, az „Összeset” kellene kiválasztania, úgy, hogy az új ár legyen érvényes az összes vevőre. Ha különböző árakat különböztet meg az egyes vevői szegmensek között, akkor válassza a Csoportot. A Csoport kiválasztásához be kell állítania a Vevői árcsoportokat.  

7. A **Fiókválasztás** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
8. Keresse meg és jelölje ki a kívánt rekordot a listán.
9. A **Cikk-kód** mezőben válassza ki a „Tábla” lehetőséget.
    
    Ha "Ár (eladási)" típusú kereskedelmi megállapodást ír be, akkor csak a "Tábla" elemet válassza ki a **Cikk-kód** mezőben. Ennek oka az, hogy az ár abszolút érték, és nem lehet azonos egy termékcsoport összes termékére.
    
10. A **Cikk-viszony** mezőben kattintson a legördítő nyílra a keresőlista megnyitásához.
11. A listában válassza ki a szerződésben szerepeltetni kívánt terméket. Jegyezze meg, hogy mely termék van kijelölve.  
12. Adja meg a minimum mennyiséget a **Kezdőérték** mezőben.
    - Ha a vevőnek egy minimális mennyiséget kell rendelnie, mielőtt új ár igényelhetne, akkor meg kell adnia a mennyiséget itt.  
    - Adjon meg egy értéket a **Címzett** mezőben, hogy megadja a maximális mennyiséget, amely felett a megállapodási ár nem lesz érvényes. Ha több mennyiségi szünet alapján ajánl árakat és engedményeket, adja meg az egyes mennyiségi határértékeket egy minimális és maximális mennyiségként a **Kezdő** és a **Befejező** mezőkben.
13. Az **Összeg devizában mezőben** adjon meg egy árat.
14. A **Részletek** szakaszban, a **Kezdő dátum** mezőben adjon meg egy dátumot, amelytől kezdve érvényes lesz a szerződés.
15. Kattintson a **Mentés** gombra.
16. Kattintson az **Érvényesítés** gombra.
17. Kattintson a **Kijelölt sorok érvényesítése** pontra.
18. Kattintson az **OK** gombra.
19. Kattintson a **Bejegyzés** lehetőségre.
20. Kattintson az **OK** gombra.

## <a name="view-trade-agreements-for-a-product"></a>Termékkel kapcsolatos kereskedelmi megállapodások megtekintése
1. Kattintson ide: **Navigációs ablaktábla > Modulok > Termékinformációk kezelése > Termékek > Kiadott termékek**.
2. A listában keresse meg és válassza ki a terméket, amelynek éppen frissítette az árát.
3. A **Művelet panelen** kattintson az **Értékesítés** elemre.
4. Kattintson a **Kereskedelmi megállapodások megtekintése** pontra.
    
    Tekintse át az imént létrehozott ármegállapodás részletes adatait.    

5. Zárja be a lapot.

## <a name="additional-resources"></a>További erőforrások
### <a name="community-blogs"></a>Közösségi blogok
- [Értékesítési árak a Dynamics 365 for Finance and Operations szolgáltatásban](https://financefunction.tech/2018/11/14/sales-prices-in-dynamics-365-for-finance-and-operations/#sales_price_in_trade_agreements)
