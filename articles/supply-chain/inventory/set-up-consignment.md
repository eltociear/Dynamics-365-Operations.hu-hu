---
title: Szállítmány beállítása
description: Ez a témakör azt mutatja be, hogyan kell konfigurálni a bejövő bizományosi készlet műveleteit.
author: perlynne
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DirPartyTable, EcoResTrackingDimensionGroup, InventJournalName, InventJournalOwnershipChange, InventOwner, InventTableInventoryDimensionGroups, VendTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 220804
ms.assetid: 88822f78-4de5-462c-a55f-1f766c572719
ms.search.region: Global
ms.author: perlynne
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 04b3fb3038a1373e203ec240a0163cf67de655cc
ms.sourcegitcommit: 57bc7e17682e2edb5e1766496b7a22f4621819dd
ms.translationtype: HT
ms.contentlocale: hu-HU
ms.lasthandoff: 11/18/2019
ms.locfileid: "2813846"
---
# <a name="set-up-consignment"></a>Szállítmány beállítása

[!include [banner](../includes/banner.md)]

Ez a témakör azt mutatja be, hogyan kell konfigurálni a bejövő bizományosi készlet műveleteit.

A bizományosi árukészlet olyan készlet, amely a szállító tulajdonában van, de a tárolása az Ön telephelyén történik. Ha készen áll a felhasználására vagy a készlet használatára, átveszi a készlet tulajdonjogát. Ez a témakör a bizományosi folyamatok engedélyezéséhez szükséges beállításokat ismerteti. A bizományosi folyamatok beállításával kapcsolatos további tudnivalókért lásd: [Bizományosi viszony beállítása](consignment.md).

## <a name="inventory-owners"></a>Készlettulajdonosok
Fizikai bejövő bizományosi készlet rögzítéséhez meg kell határozni a szállító-tulajdonost. Ez a **készlettulajdonos** oldalon történik. Ha bejelöli a **szállítói számlát**, ezzel létrehozza a **Név** és **Tulajdonos** mezők alapértelmezett értékeit. Az a **tulajdonos** mezőben lévő érték látható a szállító számára, ezért érdemes úgy módosítani, hogy a szállítói számla nevei ne legyenek könnyen felismerhetők külső felhasználók számára. A **tulajdonos** mezőt lehet módosítani, de csak addig a pontig, amikor menti a **készlettulajdonos** rekordot. A **Név** mezőt a rendszer automatikusan beírja annak a félnek a neve alapján, akihez a szállítói számla hozzá van rendelve, és ez nem módosítható.

[![készlettulajdonosok](./media/inventory-owners.png)](./media/inventory-owners.png)

## <a name="tracking-dimension-group"></a>Nyomonkövetésidimenzió-csoport
A bizományosi folyamatokban használandó cikkeket társítani kell egy **nyomon követési dimenziócsoporttal**, ahol a **tulajdonos** dimenzió értéke **aktív**. A tulajdonos dimenzió esetében a **leltár** és a **pénzügyi készlet** opció mindig ki van választva. A **fedezeti terv dimenziónként** soha nincs bejelölve.

[![nyomonkövetésidimenzió-csoport](./media/tracking-dimension-group.png)](./media/tracking-dimension-group.png)

## <a name="inventory-ownership-change-journal"></a>Készlet tulajdonosváltozási naplója
A **készlettulajdonos-változási**napló arra szolgál, hogy rögzítse, amikor a bizományosi készlet tulajdonosa a szállítóról a felhasználó jogi személyre változik. Mint bármely készletnapló esetében ezt is azonosítani kell egy készletnapló-névvel. Ezeknek a neveknek a létrehozása a **készletnapló-nevek** lapon történik, és a **naplótípust** **tulajdonos módosítása** értékre kell állítani.

[![készlet tulajdonosváltozási naplója](./media/inventory-ownership-change-journal.png)](./media/inventory-ownership-change-journal.png)

## <a name="vendor-collaboration-in-consignment-processes"></a>Szállítói együttműködés a bizományosi folyamatokban.
Ha az Ön szállítói a szállítói együttműködési felületet használják, ezt arra is felhasználhatják, hogy nyomon kövessék az Ön telephelyén lévő készlet felhasználását. A szállítóknak a szállítói együttműködésben való beállítására vonatkozó további tudnivalókat lásd: [Szállítói portál felhasználói biztonsága](../procurement/configure-security-vendor-portal-users.md).
