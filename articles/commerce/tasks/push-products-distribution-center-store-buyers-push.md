---
title: " Termékek elosztása az elosztási központból az üzletbe a központi elosztás használatával"
description: Ez az eljárás bemutatja, hogy mely lépésekkel hozhat létre és dolgozhat fel egy Központi elosztást, amellyel termékeket oszthat el egyetlen helyről egy vagy több üzletbe.
author: rubencdelgado
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailBuyersPush, InventLocationIdLookup, InventItemIdLookupSimple, RetailReplenishmentTreeLookup
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: rubendel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 62eeb29e348c558e8954f656b89d90792b0c347b
ms.sourcegitcommit: 81a647904dd305c4be2e4b683689f128548a872d
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 02/01/2020
ms.locfileid: "3022761"
---
# <a name="push-products-from-distribution-center-to-store-using-buyers-push"></a> Termékek elosztása az elosztási központból az üzletbe a központi elosztás használatával

[!include[task guide banner](../includes/task-guide-banner.md)]

Ez az eljárás bemutatja, hogy mely lépésekkel hozhat létre és dolgozhat fel egy Központi elosztást, amellyel termékeket oszthat el egyetlen helyről egy vagy több üzletbe. A felhasználó több konfigurációt is definiálhat, majd kérheti a rendszer javaslatát a termékek elosztására, vagy manuálisan megadhatja, hogy a termékek elosztása hová és az egyes üzletekbe milyen mennyiségben történjen. Ez az eljárás nem tartalmazza a Központi elosztás lehetőségben használható adatok (például: feltöltési szabályok, szervezeti hierarchiák, üzletek súlya) beállítását. Ez az eljárás az USRT bemutatócéget használja.

1. Nyissa meg a következőt: Központi elosztás.
2. Kattintson az Új lehetőségre.
3. A Leírás mezőben adjon meg egy értéket.
4. A Hely mezőben adjon meg vagy válasszon ki egy értéket.
5. A Raktár mezőben adjon meg vagy válasszon ki egy raktárt, amelyben termékek aktuális készletei találhatók.
6. Kattintson a Hozzáadás gombra.
7. A listában jelölje meg a kiválasztott sort.
8. A Cikkszám mezőben adjon meg, vagy válasszon ki egy terméket.
9. Kattintson a Hozzáadás gombra.
10. A listában jelölje meg a kiválasztott sort.
11. A Cikkszám mezőben adjon meg, vagy válasszon ki egy termékváltozatot.
    * Termékváltozat megadásakor minden egyes változathoz létrejönnek sorok.  
12. Jelöljön meg egy sort a listán.
13. A Központilag elosztott mennyiség mezőbe írja be, hogy a kiválasztott termékből mennyit kíván elosztani.
14. A További központilag elosztandó mennyiség mezőben adja meg azoknak a termékeknek a mennyiségét, amelyekből rendelkezésre áll elosztható mennyiség.
15. Az Elosztás mezőbe írja be: „Hely súly”.
    * Más elosztási szabályok használatához kiválaszthatja a többi típust is.  
16. Válasszon ki egy értéket a Feltöltési hierarchia mezőben.
17. Válassza az Igen lehetőséget a Szortimentek figyelembevétele mezőben.
18. Kattintson a Mennyiségek kiszámítása gombra, majd ellenőrizze a Raktár szakasz soraihoz adott mennyiségeket.
19. Kattintson a Rendelés létrehozása gombra.
20. Kattintson az Igen gombra.

