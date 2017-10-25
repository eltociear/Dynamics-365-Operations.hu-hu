---
title: "Kimenő folyamat"
description: "Ez a témakör a Készletkezelés kimenő folyamatairól nyújt áttekintést."
author: perlynne
manager: AnnBe
ms.date: 10/04/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: WMSOrder, WMSShipment, MCRPickingWorkbench, WMSPickingRegistration, CustomFilterGroup
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 274363
ms.assetid: 375807b2-a426-4f1b-bc1f-2fe00fd48413
ms.search.region: global
ms.search.industry: Distribution
ms.author: perlynne
ms.dyn365.ops.intro: AX 7.0.0
ms.search.validFrom: 2016-02-28
ms.translationtype: HT
ms.sourcegitcommit: 9c09a7bd314bb9005eb0b6c69d7cccad1c30cfdb
ms.openlocfilehash: 7b395cab2184f8f9f3f50a7a595c6ed782645323
ms.contentlocale: hu-hu
ms.lasthandoff: 10/04/2017

---

# <a name="outbound-process"></a>Kimenő folyamat

[!include[banner](../includes/banner.md)]

Ez a témakör a Készletkezelés kimenő folyamatairól nyújt áttekintést.

## <a name="output-orders"></a>Kimeneti rendelések

Kimeneti rendelésekkel az értékesítésirendelés-sorok és az átmozgatási rendelés sorai összeköthetők a kitárolási listákat használó kimenő kitárolási folyamatokkal.

Amikor a kitárolási listák értékesítési rendelések vagy átmozgatási rendelések alapján létrejönnek, automatikusan létrejönnek a szállítmányok és a kimeneti rendelések. Minden kitárolási lista egyetlen szállítmányhoz tartozik. Az átmozgatási rendelés szállítmánya vagy az értékesítési rendelés csomagjegyzéke a szállítmányból dolgozható fel. 

A következő ábrán áttekinthető a kimenő rendelések folyamata. 

[![A kimenő rendelési folyamat áttekintése](./media/outbound-order.png)](./media/outbound-order.png)

Kimenő szabályok beállításával meg lehet határozni, hogyan kezelje a program a kimenő folyamatot. Ezeket a szabályokat a szállítmányozási folyamat nagyobb mértékű ellenőrzéshez használhatja. A szabályok segítségével különösen meg lehet szabni, a folyamat mely fázisában lehet szállítmányt küldeni. A következő beállítások határozzák meg, hogy hogyan kezeli a rendszer a kimenő folyamatokat.

## <a name="picking-route-status-for-sales-and-transfer-orders"></a>Kitárolási útvonali állapot értékesítési és átmozgatási rendeléseknél 

Lépjen a **Kinnlévőségszámlák**\>**Beállítás**\>**Kinnlévőségek paraméterei** pontra, majd a **Frissítések** fülön válasszon egy értéket a **Kitárolási útvonal állapota** mezőben.

[![Kitárolási útvonali állapot mező értékesítési rendeléseknél](./media/picking-route-status-sales-order.png)](./media/picking-route-status-sales-order.png)

Ha a **Kitárolási útvonal állapota** mező értéke **Kész**, a kitárolási folyamat automatikusan megtörténik a kitárolási listák létrehozása során. Ha a mező értéke **Aktív**, a kitárolásilista-sorokat kézzel kell frissíteni.

Ugyanez a beállítás vonatkozik az átmozgatási rendelésekre. Lépjen a **Készletkezelés**\>**Beállítása**\>**Készlet- és raktárkezelési paraméterek** elemre, majd az a **Szállítási** fülön válasszon egy értéket a **Kitárolási útvonal állapota** mezőben.

[![Kitárolási útvonali állapot mező átmozgatási rendeléseknél](./media/picking-route-status-transfer-order.png)](./media/picking-route-status-transfer-order.png)

## <a name="end-output-inventory-orders"></a>Kimeneti készletrendelések lezárása

Lépjen a **Készletkezelés** \> **Beállítás** \> **Készlet- és raktárkezelési paraméterek** elemre, majd az **Általános** lapon állítsa be a  **Kimeneti készletrendelés befejezése** lehetőséget.

[![Kimeneti készletrendelési opció lezárása](./media//end-output-inventory-order.png)](./media//end-output-inventory-order.png)

Bizonyos esetekben néhány készleten lévő cikk nem tárolható ki a kitárolási lista folyamatának részeként. Ez az eset például akkor fordulhat elő, ha egy raktári dolgozó csökkenti a mennyiséget a kitárolási sorokban, és feldolgozza a kitárolási listát. Ha a **Kimeneti készletrendelés lezárása** beállítás **Igen** értékre van állítva, ki nem tárolt mennyiségekről visszajelentés készül a rendelés szintjére. Ha a beállítás értéke **Nem**, ki nem tárolt mennyiségek megmaradnak egy nyitott kimeneti rendelés mennyiségeként. Ebben az esetben a mennyiségek a raktárba kiadva maradnak, és hozzá kell adni őket egy új kitárolási listához a **Kimenő megrendelések** funkció részeként.

[![Kimenő megrendelések a Funkciók menüben](./media/open-output-order.png)](./media/open-output-order.png)

[![Funkciók menü a Kimenő megrendelések oldalon](./media/open-output-order-function.png)](./media/open-output-order-function.png)

## <a name="reduce-quantity"></a>Mennyiség csökkentése

A harmadik paraméter, amely a kitárolási listák létrehozása folyamat részeként használható, a **Mennyiség csökkentése** paraméter. E paraméter beállítása együttesen működik a **Foglalás** beállítással, amely a raktárba való kiadás részeként kiváltja a foglalási folyamatot.

[![Mennyiség csökkentése paraméter](./media/reduce-quantity.png)](./media/reduce-quantity.png)

## <a name="example-of-an-outbound-process-for-a-sales-order"></a>Példa értékesítési rendelés kimenő folyamatára

Ebben a példában egy értékesítési rendelést találunk két elemre. A kitárolási lista létrehozása során válassza a **Mennyiség csökkentése** paramétert. Így csak az elérhető aktuális készletet adja ki és hoz létre kitárolási sorokat. A kitárolást jelenteni kell a kitárolási listák regisztrációs folyamatán keresztül (**Kitárolási útvonal állapota** = **Aktív**).

A készlet, amely még nem foglalt, fenntartásra kerül a kitárolási lista létrehozása során. A rendelkezésre nem álló készlet vagy eltávolítható az értékesítési rendelésből, vagy kiadható a raktárnak későbbi kimenő feldolgozásra, amikor készlet elérhető lesz kitárolásra.

[![A kitárolási lista frissítése](./media/update-picking-list.png)](./media/update-picking-list.png)

Amint a kiadási sorok kitárolása a **Kitárolási lista rögzítése** oldalon megtörtént, a társított szállítmány lezárul. Az értékesítési rendelés szállítóleveleinek folyamata ezután inicializálható a kitárolt készlet alapján.

[![Kimenő szállítmányok frissítése](./media/outbound-shipments.png)](./media/outbound-shipments.png)
